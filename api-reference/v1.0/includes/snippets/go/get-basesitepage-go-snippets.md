---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



pages, err := graphClient.Sites().BySiteId("site-id").Pages().ByBaseSitePageId("baseSitePage-id").Get(context.Background(), nil)


```