---
title: Get started as a project admin or organization Owner
titleSuffix:  Azure DevOps
ms.custom: seodec18
description: Learn how to structure a project, manage users, and more to support your software development teams in Azure DevOps
ms.technology: devops-new-user 
ms.assetid: 
ms.author: chcomley
author: chcomley
ms.topic: conceptual
monikerRange: '>= tfs-2013'
ms.date: 06/14/2019
---

# Manage your project

[!INCLUDE [version-vsts-tfs-all-versions](../includes/version-vsts-tfs-all-versions.md)]  

With most Azure DevOps Services, you can start using the service and configure resources as you go. No up-front work is required. Most settings define defaults.  

As an organization Owner or a Project Administrator, there are a few tasks you might want to do to ensure a smooth operational experience. If you need to manage an organization with a large user base, you'll want to consider additional tasks to structure your projects to support multiple teams or software development apps.  


## Add users to your project

::: moniker range="azure-devops"  
Ensure that all members of your organization or group are added to your organization and projects. For small groups, using [Microsoft Accounts](https://account.microsoft.com/account) to add users to your organization and projects works fine.

Larger enterprises may want to consider using Azure Active Directory to manage permissions and user access. To learn more, see [About organization management](../organizations/accounts/organization-management.md).

::: moniker-end  

::: moniker range="< azure-devops"
 
Ensure that all members of your organization or group are added to your organization and project. Larger organizations may want to consider using Azure Active Directory to keep the maintenance of managing permissions and user access. Typically, you should install Azure Active Directory before installing TFS. To learn more, see the following articles.

- [Install Azure Active Directory Domain Services (Level 100)](/windows-server/identity/ad-ds/deploy/install-active-directory-domain-services--level-100-)
- [Step-By-Step: Setting up Azure Active Directory in Windows Server 2016](/archive/blogs/canitpro/step-by-step-setting-up-active-directory-in-windows-server-2016)

::: moniker-end

To delegate the task of managing user access, add a user with Stakeholder or higher access to the [Project Collection Administrators group](../organizations/security/set-project-collection-level-permissions.md).

## Grant or restrict permissions

Access to features and functions is controlled by access-level assignments, permissions, and security groups. To quickly understand the defaults configured for your project, see [Default permissions and access](../organizations/security/permissions-access.md). 

To delegate specific tasks to others, add them to a built-in or custom security group or add them to a specific role. To learn more, see the following articles.

- [Grant or restrict access to select features and functions](../organizations/security/restrict-access.md)  
- [Set permissions at the project level or project collection level](../organizations/security/set-project-collection-level-permissions.md)

To learn more about permissions and security, review the following articles:

- [About security and identity](../organizations/security/about-security-identity.md)  
- [About permissions and groups](../organizations/security/about-permissions.md)  
- [About security roles](../organizations/security/about-security-roles.md)  
- [About access levels](../organizations/security/access-levels.md)  

::: moniker range=">= tfs-2015"

## Share your project vision and support collaboration

::: moniker-end

::: moniker range="azure-devops"  

Each project has a summary page that's useful for sharing information through **README** files. Or, redirect users to a project Wiki. For users who are new to your project, we recommend that you [set up your project summary page](../organizations/projects/project-vision-status.md) or [provision a Wiki](../project/wiki/wiki-create-repo.md). Use these features to share established processes and procedures for your project.

::: moniker-end  

::: moniker range=">= tfs-2015 < azure-devops"  
Each project has a summary page that's useful for sharing information through **README files**. For users who are new to your project, we recommend that you [set up your project summary page](../organizations/projects/project-vision-status.md). Use this feature to share established processes and procedures for your project. 

::: moniker-end

::: moniker range=">= azure-devops-2019"  

## Remove unused services from the user interface

To simplify the web portal user interface, you can disable select services. For example, if you use a project only to log bugs, then disable all services except for **Boards**.

This example shows that **Test Plans** is disabled:

> [!div class="mx-imgBorder"]
> ![Disable a service](media/services/set-service-visibility.png)

::: moniker-end  

::: moniker range=">= tfs-2015"  

## Set code, test, and other policies 

Set policies to support collaboration across your teams, secure your projects, and automatically remove obsolete files. To set policies, review the following articles: 

::: moniker-end  

::: moniker range=">= azure-devops-2019"

- [Change application access policies for your organization](../organizations/accounts/change-application-access-policies.md)
- [Manage branch policies](../repos/git/branch-policies.md)  
- [Add Team Foundation Version Control (TFVC) check-in policies](../repos/tfvc/add-check-policies.md)  
- [Set build and release pipeline retention policies](../pipelines/policies/retention.md) 
- [Set test retention policies](../test/how-long-to-keep-test-results.md) 
::: moniker-end  

::: moniker range=">= tfs-2015 <= tfs-2018"

- [Manage branch policies](../repos/git/branch-policies.md)  
- [Add TFVC check-in policies](../repos/tfvc/add-check-policies.md)  
- [Set build and release pipeline retention policies](../pipelines/policies/retention.md) 
- [Set test retention policies](../test/how-long-to-keep-test-results.md) 
::: moniker-end  


## Define area and iteration paths for work tracking

If you support several products, you can assign work items by feature area by defining [area paths](../organizations/settings/set-area-paths.md). To assign work items to specific time intervals, also known as sprints, you configure [iteration paths](../organizations/settings/set-iteration-paths-sprints.md). To use the Scrum tools&mdash;sprint backlogs, taskboards, and team capacity&mdash;you need to configure several sprints. For an overview, see [About areas and iteration paths](../organizations/settings/about-areas-iterations.md).  


> [!div class="mx-tdBreakAll"] 
> |Iterations| Areas |
> |-------------|----------| 
> |<img src="../organizations/settings/media/areas/areas-iterations-iterations-intro-ts-2016.png" alt="Default iterations, Scrum process" style="border: 1px solid #C3C3C3;" /> | <img src="../organizations/settings/media/areas/areas-iterations-areas-intro-ts-2016.png" alt="A set of sample area paths" style="border: 1px solid #C3C3C3;" /> | 


## Customize work-tracking processes

::: moniker range=">= azure-devops-2019"
  
All work-tracking tools are available immediately after you create a project. Often, one or more users may want to customize the experience to meet one or more business needs. Processes are easily customized through the user interface. However, you may want to establish a methodology for who manages the updates and evaluates requests.

To learn more, see the following articles:

- [About process customization and inherited processes](../organizations/settings/work/inheritance-process-model.md)  
- [Customize a project](../organizations/settings/work/customize-process.md)  
- [Add and manage processes](../organizations/settings/work/manage-process.md)

::: moniker-end  

::: moniker range="<= tfs-2018"

All work-tracking tools are available immediately after you create a project.  Often, one or more users may want to customize the experience to meet one or more business needs. However, you may want to establish a methodology for who manages the updates and evaluates requests.

To learn more, see [On-premises XML process model](../reference/on-premises-xml-process-model.md).

::: moniker-end

## Review and update notifications

A number of notifications are predefined for each project you add. Notifications are based on subscription rules. Subscriptions arise from the following areas:

- [Out-of-the-box or default subscriptions](../notifications/oob-built-in-notifications.md).
- [Team notifications](../notifications/manage-team-group-notifications.md), managed by a team administrator.
- Project notifications, managed by a member of the Project Administrators group.
- [Organization and collection level notifications](../notifications/manage-organization-notifications.md), managed by a member of the Project Collection Administrators group.

If users believe they're getting too many notifications, direct them to [opt out of a subscription](../notifications/manage-your-personal-notifications.md).

> [!div class="mx-imgBorder"]  
> ![Personal notifications](media/services/personal-notifications.png)   


::: moniker range="< azure-devops"  

## Configure an SMTP server

In order for team members to receive notifications, [you must configure an SMTP server](/azure/devops/server/admin/setup-customize-alerts).  

::: moniker-end  

## Add teams to scale your organization

We recommend that you add teams as your organization grows. Each team gets [access to their own set of customizable Agile tools](../organizations/settings/about-teams-and-settings.md).

![Agile tools and team assets](../organizations/settings/media/agile-tools/agile-tools-team-assets-post-2018.png)

To learn more, see the following articles:

- [About projects and scaling your organization](../organizations/projects/about-projects.md)
- [Add a team, move from one default team to several teams](../organizations/settings/add-teams.md)  
- [Add a team administrator](../organizations/settings/add-team-administrator.md)  

::: moniker range=">= tfs-2015"
  
## Install and manage extensions 

An extension is an installable unit that adds new capabilities to your projects. Azure DevOps extensions support the following functions:

- Planning and tracking of work items, sprints, scrums, and so on  
- Build and release flows
- Code testing and tracking
- Collaboration among team members

::: moniker-end

::: moniker range=">= tfs-2017"

For example, to support [code search](../project/search/code-search.md), install the [Code Search extension](https://marketplace.visualstudio.com/items?itemName=ms.vss-code-search).

::: moniker-end  

::: moniker range=">= tfs-2015"  

You want to tell your users about extensions and that they can [request an extension](../marketplace/request-extensions.md). To install and manage extensions, you must be an organization Owner, a member of the Project Collection Administrators group. Or, you can get added to the [Manager role for extensions](../marketplace/how-to/grant-permissions.md).

::: moniker-end

::: moniker range="azure-devops"

## Set up billing

All organizations can add up to five users with Basic access and unlimited users with Stakeholder access. If you need to add more users or pay for additional services or extensions, [set up billing](../organizations/billing/set-up-billing-for-your-organization-vs.md).  

::: moniker-end

## Next steps  

> [!div class="nextstepaction"]
> [Manage projects](../organizations/projects/about-projects.md)

## Related articles

::: moniker range="azure-devops"  

- [Project and team quick reference](../organizations/projects/project-team-quick-reference.md)  
- [Security & identity](../organizations/security/about-security-identity.md)
- [Organization management](../organizations/accounts/organization-management.md)
- [About user, team, project, and organization-level settings](../organizations/settings/about-settings.md)

::: moniker-end

::: moniker range="< azure-devops"  

- [Project and team quick reference](../organizations/projects/project-team-quick-reference.md)  
- [Security & identity](../organizations/security/about-security-identity.md)
- [Organization management](../organizations/accounts/organization-management.md)
- [About user, team, project, and organization-level settings](../organizations/settings/about-settings.md)
- [TFS administration](/azure/devops/server/index)

::: moniker-end