---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\GetPasswordSingleSignOnCredentialsPostRequestBody;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new GetPasswordSingleSignOnCredentialsPostRequestBody();
$requestBody->setId('5793aa3b-cca9-4794-679a240f8b58');

$result = $graphServiceClient->servicePrincipals()->byServicePrincipalId('servicePrincipal-id')->getPasswordSingleSignOnCredentials()->post($requestBody)->wait();

```