---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\ComplianceChange;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new ComplianceChange();
$requestBody->setOdataType('#microsoft.graph.windowsUpdates.complianceChange');
$requestBody->setIsRevoked(true);

$result = $graphServiceClient->admin()->windows()->updates()->updatePolicies()->byUpdatePolicyId('updatePolicy-id')->complianceChanges()->byComplianceChangeId('complianceChange-id')->patch($requestBody)->wait();

```