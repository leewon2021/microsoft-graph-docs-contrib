---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\BusinessScenario;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new BusinessScenario();
$requestBody->setOwnerAppIds(['44109254-4b2b-7a33-76ee-c890a167b295', '13eb9d8b-1d63-4153-9417-3a69ab200a78', 	]);

$result = $graphServiceClient->solutions()->businessScenarios()->byBusinessScenarioId('businessScenario-id')->patch($requestBody)->wait();

```