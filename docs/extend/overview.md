---
ms.prod: vs-devops-alm
ms.technology: vs-devops-extensions-api
title: Developing extensions for Visual Studio Team Services (VSTS) and Team Foundation Server
description: Overview of creating extensions for Visual Studio Team Services (VSTS)
ms.assetid: bd7bd829-e80e-4234-849f-d4b273605a22
ms.manager: douge
ms.author: elbatk
ms.date: 08/23/2016
ms.topic: get-started-article
---

# Create a custom extension

>[!NOTE]
> This section covers developing custom extensions and service-hooks, to find information on installing extensions from the Marketplace, or buying Visual Studio Subscriptions, visit the [Marketplace documentation](../marketplace/index.md). For information on 


## What are extensions?

Extensions are simple add-ons that can be used to customize and extend your DevOps experience with Team Services. 
They are written with standard technologies - HTML, JavaScript, CSS - and can be developed using your preferred dev tools.
They utilize our [RESTful API Library](https://visualstudio.com/integrate/api/overview.md) in order to easily interact with Team Services and applications/services.
The [Visual Studio Marketplace](https://marketplace.visualstudio.com/VSTS) is where extensions are published, 
where they can be kept privately for you and your team or shared with the millions of developers currently using Team Services. 

## What makes up an extension?
<div align="center" style="padding-top:15px">
<img src="./_img/extension-components.png" style="padding-bottom:20px">
</div>

- A [JSON manifest file](./develop/manifest.md) contains basic info about the extension.
- Discovery assets - the markdown and images that make up your extension's overview and aesthetics in the marketplace. 
- Static files that contain the logic of your extension, including HTML, JS, and CSS files. Static files are only applicable to contribution-based extensions.

All of these are bundled up to make a Team Extensions Service Package (.vsix file) that is published to the marketplace. From the marketplace,
extensions can be installed directly by Team Services users.


## What can you do with extensions?

There are dozens of places where you can add to the Team Services user interface, and we're adding more every sprint. Learn about all of the places where you can add a hub in the [contributions reference](./reference/targets/overview.md).

- [Provide new build and release tasks](./develop/add-build-task.md) that teams can use in their builds.
- Use [dashboard widgets](./develop/add-dashboard-widget.md) to get custom views within Team Services. 
- Extend the [work item form](./develop/add-workitem-extension.md) with new tabs, sections, and actions.
- Create [your own hub](./develop/add-hub.md) to embed new capabilities within our Agile, code, build, and test experiences. 
- Develop [actions](./develop/add-action.md) that can be run on hubs, whether they're ours or ones you've created. 


## Next Steps

### Quickstarts

* [Write your first extension (Add a hub)](./get-started/node.md)

### Reference

* [Extension manifest reference](./develop/manifest.md)
