---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\UploadPkcs12PostRequestBody;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new UploadPkcs12PostRequestBody();
$requestBody->setKey('Base64-encoded-pfx-content');
$requestBody->setPassword('password-value');

$result = $graphServiceClient->trustFramework()->keySets()->byTrustFrameworkKeySetId('trustFrameworkKeySet-id')->uploadPkcs12()->post($requestBody)->wait();

```