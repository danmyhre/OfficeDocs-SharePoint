---
title: "Plan customizations, solutions, and apps for SharePoint Online"
ms.author: kaarins
author: kaarins
manager: pamgreen
ms.date: 5/25/2018
ms.audience: Admin
ms.topic: conceptual
ms.service: sharepoint-online
localization_priority: Normal
search.appverid:
- SPO160
- MET150
ms.assetid: b7898ebf-69b7-4196-81e3-b04e1a4e7d67
description: "Learn about the range of options available for branding and provisioning SharePoint sites."
---

# Plan customizations, solutions, and apps for SharePoint Online

Branding and customizing SharePoint Online is different than branding and customizing SharePoint Server products. SharePoint Online gets updated with new features on a regular basis and these updates can affect certain types of customizations. However, there are recommended customization and branding techniques available today that can streamline your branding and customization requirements. For example, if you are making structural changes to the master pages it's important to stay up to date with the ongoing product updates applied to SharePoint Online. The easiest way to stay informed is to watch the [Microsoft 365 Roadmap](https://www.microsoft.com/microsoft-365/roadmap) and monitor the [Microsoft 365 Business blog](https://www.microsoft.com/microsoft-365/business).
  
The software updates that Microsoft makes to SharePoint Online happen much faster than SharePoint Server and customizing or unghosting master pages, which are a core part of the product, will result in those customizations being affected by updates. To remedy the situation, those customizations will need to be re-applied to the updated pages. Staying up to date is possible, but needs to happen much more frequently in SharePoint Online.
  
## I'm used to customizing SharePoint Server products, what's different in SharePoint Online?

Methods for customization that work in SharePoint Server won't necessarily work in SharePoint Online. Some of the methods used for customizing and extending SharePoint Server, for example, rely on the fact that the underlying platform is not constantly being updated - as is the case with SharePoint Online. SharePoint Online is continuously being improved, and any files that have been customized or unghosted may be affected by updates. Here are some recommendations for common SharePoint customizations, as compared to private SharePoint deployments vs. the SharePoint Online service.
  
||||
|:-----|:-----|:-----|
|**Type of Customization** <br/> |**SharePoint Server** <br/> |**SharePoint Online** <br/> |
|**Workflow** <br/> |Start with Out of the box workflows  <br/> SharePoint Designer, or Visual Designer  <br/> |[Use Microsoft Flow](/flow) to create automated workflows|
|**Header/Footer** <br/> |SharePoint Designer, with unghosted pages  <br/> |No equivalent, unghosting pages requires ongoing maintenance  <br/> |
|**Content Blocks** <br/> |CBQ (un-throttled)  <br/> |CBQ (throttled)  <br/> |
|**General Branding (colors, logos, etc.)** <br/> |Sandboxed solutions, Customized/unghosted Master Pages  <br/> |Composed looks or inject styles via app model  <br/> |
|**Navigation** <br/> |Start with out of the box tools  <br/> Structural, managed, and search-driven navigation  <br/> |Start with out of the box tools  <br/> [Navigation options for SharePoint Online](/office365/enterprise/navigation-options-for-sharepoint-online) <br/> |
   
## Customizations: simple to complex
<a name="__toc349226253"> </a>

SharePoint Online customizations range from non-technical changes you can apply quickly in the browser using site commands or features to custom app development using developer tools:
  
1. **Customization using the browser** You can use the browser-based settings SharePoint Online to apply simpler customizations like changing title and logo, updating navigation links, applying a new site theme, changing the contents of a page, or changing views for lists and libraries. Browser-based customizations are the easiest customizations to apply, and they require minimal technical expertise. 
    
2. **Customizations using supported tools and applications** You can use supported SharePoint tools to perform more extensive customizations. For example, Office applications like Access, Excel, and Visio help you create highly dynamic, data-rich pages on your site. You can use [Microsoft PowerApps](https://powerapps.microsoft.com/) to build no-code solutions.
    
3. **Customizations using remote provisioning** In SharePoint Online, you can use custom CSOM code in apps for SharePoint to provision SharePoint sites and subsites with branding elements. This site provisioning pattern is called remote provisioning. 
    
4. **Customizations using add-ins for SharePoint** The new Cloud App Model in SharePoint Online enables you to add apps to your sites, and is the recommended replacement for Sandboxed solutions going forward. You can use existing third-party apps or build your own. Add apps to a site when you want to customize it with specific functionality or information. For example, you can add apps that perform general tasks like time and expense tracking. Or you can use apps and remote provisioning to apply branding elements to sites. You can also add apps that display news or information from third-party providers, or that connect to social websites. 
    
  - **Third-party apps** Third-party apps are found in the SharePoint Store, which is an Office.com-hosted marketplace accessible from SharePoint Online sites. Select the apps that you want to be available in your organization. Admins can also buy licenses for specific apps for all users in an organization (requires Site Owner permissions or greater). 
    
  - **Custom apps** Your organization can also develop its own apps for SharePoint Online and make them available to users through the App Catalog site. If you know how to build a web application, then you know how to build an app for SharePoint. You can use any language, such as HTML, JavaScript, PHP, or .NET, and your favorite web development tools, including Microsoft Visual Studio. For more information, see [Get started developing apps for SharePoint](/sharepoint/dev/sp-add-ins/get-started-creating-sharepoint-hosted-sharepoint-add-ins).
    
## Can I still develop sandboxed solutions?
<a name="sandboxed"> </a>

Sandboxed solutions have been deprecated in SharePoint Online. Alternative solutions such as remote provisioning offer similar capabilities. Sandboxed solutions carried over as part of a migration will continue to work for a limited period; however, we highly recommend that you replace all sandboxed solutions with alternative functionality such as online apps. In the meantime, be aware that ongoing updates to SharePoint Online may affect some sandboxed solutions.
  
With the introduction of the cloud app model (CAM) and apps for SharePoint, there are now alternatives to older, more established ways of branding and provisioning SharePoint sites.
  
You can perform all types of site branding using apps for SharePoint to provision site branding throughout the enterprise and manage branding at scale: a pattern known as [remote provisioning](/sharepoint/dev/solution-guidance/use-remote-provisioning-to-brand-sharepoint-pages). While SharePoint developers have historically used the SharePoint feature framework, site templates, web templates, and site definitions to provision sites, the remote provisioning pattern shows you how to create custom [SharePoint add-ins](/sharepoint/dev/sp-add-ins/sharepoint-add-ins) that provision site branding and perform other site provisioning tasks. 
  
## Why Add-ins?
<a name="sandboxed"> </a>

Add-ins for SharePoint offer several advantages over sandboxed solutions. They provide users with a way to extend SharePoint sites without creating additional operational burden for admins. Add-ins are also easy for end users to discover and add. Add-ins for SharePoint Online are architected for the cloud, so they better integrate with the respective cloud-based resources in smoother and more flexible ways than sandboxed solutions.
  
See also [SharePoint Add-ins compared with SharePoint solutions](/sharepoint/dev/general-development/sharepoint-add-ins-compared-with-sharepoint-solutions), [SharePoint solution packs](https://www.microsoft.com/en-us/download/details.aspx?id=42030), and the [SharePoint Patterns and Practices on Github](https://github.com/OfficeDev/PnP).
  
## Examples of common SharePoint Online customizations
<a name="__toc349226255"> </a>

To determine the method of customization or development that is appropriate for your organization, think about what you want to customize and what kinds of solutions you want to develop.
  
There are several different ways you can achieve the same outcome on a SharePoint site. For example, if your goal is to create a highly-customized list, you can achieve this by using different List Settings in the browser to configure a list and its views. You might even be able to perform all of the desired customization this way.
  
It is a good practice to first start with browser-based customizations before using supported tools and applications to achieve similar customizations.
  
    
 **I want to change the look and feel or site design**
  
|**First, try browser-based options:**|**Then, try no-code solutions :**|**Then, consider custom code solutions:**|
|:-----|:-----|:-----|
| Use the Site Settings page to:  <br/> [Change the look of your SharePoint site](https://support.office.com/article/06bbadc3-6b04-4a60-9d14-894f6a170818) <br/> [Customize the navigation on your SharePoint site](https://support.office.com/article/3cd61ae7-a9ed-4e1e-bf6d-4655f0bf25ca) <br/> [Choose a theme for your publishing site](https://support.office.com/article/a56da772-55fa-4765-b0a8-32a3b80005d3) <br/>  Apply custom CSS files to the site  <br/>  Change the primary and publishing master pages  <br/> | Use Design Manager to leverage your expertise in HTML, CSS, and JavaScript (available only for publishing sites):  <br/>  Easily design HTML master pages and page layouts in your HTML editor of choice.  <br/>  Convert the HTML file to an ASP.NET master page.  <br/>  Add key functionality to your pages, such as a search box or navigation control, from the Snippet Gallery.  <br/>  Design unique UI experiences for different devises by [creating device channels](/sharepoint/dev/general-development/sharepoint-design-manager-device-channels).  <br/>  For more information about using Design Manager, see [Overview of Design Manager](/sharepoint/dev/general-development/overview-of-design-manager-in-sharepoint).  <br/> | Develop apps for SharePoint that feature App Parts or custom UI actions, such as ribbon or menu commands.  <br/>  Use Visual Studio to:  <br/>  Create custom site pages  <br/>  Create custom ribbon enhancements  <br/>  Create custom dialog box or ribbon controls  <br/>  Deploy custom design solutions as features  <br/> |
   
> [!NOTE]
> If possible, try to customize your site using custom CSS elements and themes rather than custom master pages. Custom master pages will block upgrade to the latest user interface experience when upgrades are rolled out to customers. This may introduce unexpected costs for your organization at upgrade time. 
  
 **I want to customize the appearance of information on sites**
  
|**First, try browser-based options:**|**Then, try no-code solutions:**|**Then, consider custom code solutions:**|
|:-----|:-----|:-----|
| Customize individual pages on the site:  <br/>  Add and edit text, images, video, and other objects  <br/>  Add and customize Web Parts  <br/>  Add and customize new lists and libraries  <br/>  Create custom views and forms for lists and libraries  <br/>  Create and edit content and publishing pages  <br/>  Enable or disable features  <br/> | Add third-party apps for SharePoint to integrate information into sites. See [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43).  <br/>  Use SharePoint Designer to:  <br/>  Add text, images, scripts, and Web Parts to pages  <br/>  Create and customize site and Web Part pages  <br/>  Add custom actions  <br/>  Add Custom navigation  <br/>  Use supported Microsoft Office applications to:  <br/>  Publish workbooks with data, charts, and visualizations using Excel 2013 and Excel Services  <br/>  Publish data visualizations with Visio 2013 and Visio Services  <br/> | Use the Script Editor Web Part to add JavaScript code to site pages.  <br/>  Develop apps for SharePoint that feature App Parts designed to display information  <br/>  Use Visual Studio to:  <br/>  Create custom site pages  <br/>  Create custom Web Parts  <br/> |
   
 **I want to display content from different data sources**
  
|**First, try browser-based options:**|**Then, try no-code solutions:**|**Then, consider custom code solutions:**|
|:-----|:-----|:-----|
| Add Web Parts that retrieve content from external sites or data sources  <br/>  Customize list views and forms from various data sources  <br/> | Use Excel 2013 and Excel Services to display and visualize data from a wide variety of data sources.  <br/>  User Microsot PowerApps to build no-code business solutions.  <br/>  Add third-party apps for SharePoint to integrate information into sites. See [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43).  <br/>  Configure Business Connectivity Services and to connect to data sources such as SQL Azure databases or Windows Communication Foundation web services.  <br/>  | Develop custom apps for SharePoint to integrate and display information.  <br/>  Use Visual Studio to:  <br/>  Create custom list definitions  <br/>  Create custom site pages  <br/>  Create custom Web Parts  <br/>  Create custom dialog box or ribbon controls  <br/> |
   
## Making solutions or apps available to users
<a name="__toc349226256"> </a>

After you finish developing a solution or a custom app, you may need a way to make it available on one or more sites in your organization. Here are some ways you can do that:
  
- If your solution is a customized list or a specialized site or page, you can share a link to that page or site with users.
    
- If you developed a custom SharePoint or Office app, you can make it available by uploading it to the App Catalog site. For more information about making custom apps available, see [Use the App Catalog to make custom business apps available for your SharePoint Online environment](use-app-catalog.md).
    
- If you added a third-party app from the SharePoint Store, you can make it available to all users across the sites in your organization by acquiring licenses for all users in your organization. Or, you can acquire licenses for only those who need to use it, and assign those licenses to the designated users. For more information, see [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43) and [Manage app licenses for a SharePoint Online environment](manage-app-licenses.md).
    
- If you want to change the settings for whether or not site users can acquire apps from the SharePoint Store, see [Configure settings for the SharePoint Store](configure-sharepoint-store-settings.md).
    
- Custom solutions can be made available as well; however, if users are selectively using sandboxed solutions it will be difficult to ensure those sites are refreshed with updated solutions after the SharePoint Online update process affects the site.
    
## Exploring partner solutions and services
<a name="__toc349226257"> </a>

If you are interested in exploring services or applications from Microsoft partners that are available for SharePoint Online, browse Office 365 apps on [Microsoft AppSource](https://go.microsoft.com/fwlink/?linkid=865097). There are also many open source solutions developed by the collective SharePoint Online community, including Microsoft, MVPs, Partners, and Customers on the [Office 365 Developer Patterns and Practices Github site](https://github.com/OfficeDev/PnP).
 

  

