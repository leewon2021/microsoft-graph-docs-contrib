---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\GovernanceRoleSetting;
use Microsoft\Graph\Generated\Models\GovernanceRuleSetting;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new GovernanceRoleSetting();
$adminEligibleSettingsGovernanceRuleSetting1 = new GovernanceRuleSetting();
$adminEligibleSettingsGovernanceRuleSetting1->setRuleIdentifier('ExpirationRule');
$adminEligibleSettingsGovernanceRuleSetting1->setSetting('{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}');
$adminEligibleSettingsArray []= $adminEligibleSettingsGovernanceRuleSetting1;
$requestBody->setAdminEligibleSettings($adminEligibleSettingsArray);


$result = $graphServiceClient->privilegedAccess()->byPrivilegedAccessId('privilegedAccess-id')->roleSettings()->byGovernanceRoleSettingId('governanceRoleSetting-id')->patch($requestBody)->wait();

```