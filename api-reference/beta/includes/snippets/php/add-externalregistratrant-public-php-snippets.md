---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\ExternalMeetingRegistrant;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new ExternalMeetingRegistrant();
$requestBody->setOdataType('#microsoft.graph.externalMeetingRegistrant');
$requestBody->setId('9d96988d-a66a-46ce-aad7-0b245615b297');

$result = $graphServiceClient->me()->onlineMeetings()->byOnlineMeetingId('onlineMeeting-id')->registration()->registrants()->post($requestBody)->wait();

```