---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\GraphServiceClient;
use Microsoft\Graph\Generated\Models\Channel;
use Microsoft\Graph\Generated\Models\ChannelModerationSettings;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new Channel();
$requestBody->setDisplayName('UpdateChannelModeration');
$requestBody->setDescription('Update channel moderation.');
$moderationSettings = new ChannelModerationSettings();
$moderationSettings->setUserNewMessageRestriction(new UserNewMessageRestriction('moderators'));
$moderationSettings->setReplyRestriction(new ReplyRestriction('everyone'));
$moderationSettings->setAllowNewMessageFromBots(true);
$moderationSettings->setAllowNewMessageFromConnectors(true);
$requestBody->setModerationSettings($moderationSettings);

$result = $graphServiceClient->teams()->byTeamId('team-id')->channels()->byChannelId('channel-id')->patch($requestBody)->wait();

```