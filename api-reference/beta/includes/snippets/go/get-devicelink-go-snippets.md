---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



deviceLinks, err := graphClient.NetworkAccess().Connectivity().RemoteNetworks().ByRemoteNetworkId("remoteNetwork-id").DeviceLinks().ByDeviceLinkId("deviceLink-id").Get(context.Background(), nil)


```