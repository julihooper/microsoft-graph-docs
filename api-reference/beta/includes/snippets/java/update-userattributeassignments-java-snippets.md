---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;

graphClient.identity().b2cUserFlows("{b2cIdentityUserFlowId}").userAttributeAssignments("{id}")
	.buildRequest()
	.patch(identityUserFlowAttributeAssignment);

```