---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Identity\ConditionalAccess\Policies\PoliciesRequestBuilderGetRequestConfiguration;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestConfiguration = new PoliciesRequestBuilderGetRequestConfiguration();
$queryParameters = PoliciesRequestBuilderGetRequestConfiguration::createQueryParameters();
$queryParameters->filter = "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'";
$requestConfiguration->queryParameters = $queryParameters;


$result = $graphServiceClient->identity()->conditionalAccess()->policies()->get($requestConfiguration)->wait();

```