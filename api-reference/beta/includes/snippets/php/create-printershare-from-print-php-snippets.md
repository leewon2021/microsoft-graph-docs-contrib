---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\PrinterShare;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new PrinterShare();
$requestBody->setName('name-value');
$additionalData = [
	'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}',
];
$requestBody->setAdditionalData($additionalData);

$result = $graphServiceClient->escapedPrint()->shares()->post($requestBody)->wait();

```