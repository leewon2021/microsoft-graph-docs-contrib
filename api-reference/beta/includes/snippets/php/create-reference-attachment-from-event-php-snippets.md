---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\ReferenceAttachment;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new ReferenceAttachment();
$requestBody->setOdataType('#microsoft.graph.referenceAttachment');
$requestBody->setName('Personal pictures');
$requestBody->setSourceUrl('https://contoso.com/personal/mario_contoso_net/Documents/Pics');
$requestBody->setProviderType(new ReferenceAttachmentProvider('oneDriveConsumer'));
$requestBody->setPermission(new ReferenceAttachmentPermission('edit'));
$requestBody->setIsFolder(true);

$result = $graphServiceClient->me()->events()->byEventId('event-id')->attachments()->post($requestBody)->wait();

```