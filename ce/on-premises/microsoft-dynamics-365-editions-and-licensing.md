---
title: "Microsoft Dynamics 365 editions and licensing | Microsoft Docs"
ms.custom: ""
ms.date: "10/01/2018"
ms.prod: "crm-2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (on-premises)"
  - "Dynamics CRM 2016"
ms.assetid: 3bd04575-1193-4fe4-92e1-dc0c91a1bebe
caps.latest.revision: 30
author: Mattp123
ms.author: matp
---
# Microsoft Dynamics 365 editions and licensing

[!INCLUDE [cc_applies_to_on-prem-9_0_0](../includes/cc_applies_to_on-prem-9_0_0.md)]

[!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] offers a licensing option that scales from small, to mid-level, to very large deployments.  
  
## Edition and licensing for on-premises deployments  
  
**[!INCLUDE[pn_microsoft_dynamics_crm_2016_server](../includes/pn-microsoft-dynamics-crm-2016-server.md)]**. There is no user limit for this edition. Features include support for multiple organizations, multiple server instances, and separate role-based service installation. Role-based services let you increase performance by installing [!INCLUDE[pn_microsoftcrm_server](../includes/pn-microsoftcrm-server.md)] features on different computers.     
  
### Licensing  
 A [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] deployment operates by using a single product key. However, each [!INCLUDE[pn_microsoftcrm_server](../includes/pn-microsoftcrm-server.md)] in a  deployment requires a server license.   
  
 You can view and upgrade a license by using the `Get-CrmAccessLicense` and `Set-CrmProductKey` [!INCLUDE[pn_PowerShell](../includes/pn-powershell.md)] commands or in [!INCLUDE[pn_deploymentmanager](../includes/pn-deploymentmanager.md)]. [!INCLUDE[pn_deploymentmanager](../includes/pn-deploymentmanager.md)] is a [!INCLUDE[pn_Microsoft_Management_Console](../includes/pn-microsoft-management-console.md)] snap-in that system administrators can use to manage organizations, servers, and licenses for deployments of [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md). 

 For more information about licensing, see [Microsoft Dynamics 365 (On-premises) Licensing Guide](https://mbs.microsoft.com/Files/public/365/Dynamics365EnterpriseEditionOnPremisesLicensingGuide.pdf). 
  
### Client access license types  
 You can view and modify client access license types for each user in the **Users** area of the **Settings** area in the [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] web client. 
 
## See also    
 [Planning Dynamics 365](planning-your-deployment-of-microsoft-dynamics-365.md) </br>  
 [Dynamics 365 system requirements and required technologies](system-requirements-required-technologies.md)

