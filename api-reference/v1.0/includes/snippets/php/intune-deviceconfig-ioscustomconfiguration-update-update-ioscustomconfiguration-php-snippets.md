---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\IosCustomConfiguration;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new IosCustomConfiguration();
$requestBody->setOdataType('#microsoft.graph.iosCustomConfiguration');
$requestBody->setDescription('Description value');
$requestBody->setDisplayName('Display Name value');
$requestBody->setVersion(7);
$requestBody->setPayloadName('Payload Name value');
$requestBody->setPayloadFileName('Payload File Name value');
$requestBody->setPayload(\GuzzleHttp\Psr7\Utils::streamFor(base64_decode('cGF5bG9hZA==')));

$result = $graphServiceClient->deviceManagement()->deviceConfigurations()->byDeviceConfigurationId('deviceConfiguration-id')->patch($requestBody)->wait();

```