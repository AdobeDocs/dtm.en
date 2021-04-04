---
description: Descriptions of the fields and options in the Library Management settings in Dynamic Tag Management.
seo-description: Descriptions of the fields and options in the Library Management settings in Dynamic Tag Management.
seo-title: Library management
solution: Experience Cloud
title: Library management
uuid: ffc42599-93e7-40c9-8082-f781858f4056
exl-id: af4c856e-2e81-477c-8e57-5e693459a464
---
# Library management{#library-management}

This article contains descriptions of the fields and options in the Library Management settings in Dynamic Tag Management.

 **[!UICONTROL  *Property*]** > **[!UICONTROL Edit Tool]** > **[!UICONTROL Library Management]**

>[!NOTE]
>
>If more than one Adobe Analytics tool is used in a single web property, each tool must have a unique tracker variable name. Duplicative object variable names between Adobe Analytics tools within a single web property will cause conflicts.

## Page code is already present

This prevents Dynamic Tag Management from installing [!DNL Adobe Analytics] page code if the code is already present on your site.

This feature allows you to use Dynamic Tag Management to add to your existing implementation rather than starting from scratch. Be sure to properly set your tracker variable name when checking this box.

## Load library at <*`Page Top`* or *`Page Bottom`*>

Specifies where and when to load the page code. Regardless of your selection, any rules using the Analytics tool will need to have the same setting.

## Managed by Adobe (Recommended)

Enable Dynamic Tag Management to manage your library.

If you select this option, the following option becomes available:

## Library Version

Select the latest version from the [!UICONTROL Library Version] menu. Dynamic Tag Management notifies you when new versions are available. You can revert to a previous version as necessary.

## Custom

You can configure the library code.

If you select this option, the following options become available:

## Set report suites using custom code below

When this box is checked, Dynamic Tag Management looks for a variable in your custom code called *`s_account`*. This variable should contain a comma-separated list of the report suites to which you want to send data.

## Code Hosted

Choose an option to host the [!DNL s_code]:

* **In DTM**: You can host the [!DNL s_code] within Dynamic Tag Management. Click **[!UICONTROL Edit Code]** to cut and paste the file directly into the editor. 

* **URL**: If you have a good [!DNL s_code] file and are happy with the process of updating it, you can provide the URL to the file here. Dynamic Tag Management then consumes that [!DNL s_code] file for its implementation of [!DNL Adobe Analytics].

## Open Editor

Lets you [insert core AppMeasurement code](../tools-reference/analytics-dtm.md#section_E497974E41454C979A8C90A84E2FE537). This code is populated automatically when using the automatic configuration method described in [Adobe Analytics Settings](../tools-reference/analytics-dtm.md#concept_FBA6679A0B79490F8296437F11E5E4F8).

## Tracker Variable Name

If you want to run two instances of [!DNL Adobe Analytics] in parallel (one within Dynamic Tag Management and one natively), you can rename the main *`s`* object. Renaming the object name avoids collisions.
