---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\ApplyTagsPostRequestBody;
use Microsoft\Graph\Generated\Models\Tag;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new ApplyTagsPostRequestBody();
$tagsToAddTag1 = new Tag();
$tagsToAddTag1->setId('b4798d14-748d-468e-a1ec-96a2b1d49677');
$tagsToAddArray []= $tagsToAddTag1;
$requestBody->setTagsToAdd($tagsToAddArray);


$graphServiceClient->compliance()->ediscovery()->cases()->byCaseId('case-id')->reviewSets()->byReviewSetId('reviewSet-id')->queries()->byReviewSetQueryId('reviewSetQuery-id')->microsoftGraphEdiscoveryApplyTags()->post($requestBody)->wait();

```