---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Beta.Models.Security;

var requestBody = new RetentionLabel
{
	OdataType = "#microsoft.graph.security.retentionLabel",
	RetentionDuration = new RetentionDurationInDays
	{
		OdataType = "microsoft.graph.security.retentionDurationInDays",
		Days = 2555,
	},
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
var result = await graphClient.Security.Labels.RetentionLabels["{retentionLabel-id}"].PatchAsync(requestBody);


```