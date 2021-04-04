---
description: Set up actions that you want the condition to trigger.
keywords: Dynamic Tag Management
seo-description: Set up actions that you want the condition to trigger.
seo-title: Set up actions for the condition to trigger
solution: Experience Cloud
title: Set up actions for the condition to trigger
uuid: 93c89ff1-4b7d-4895-bd75-edb56ea3600b
exl-id: ebcdfaaa-f119-451a-ae90-2ecb4d3c1132
---
# Set up actions to trigger{#set-up-actions-for-the-condition-to-trigger}

Set up actions that you want the condition to trigger.

After setting up the condition, you must set up the actions that you want the condition to trigger. These actions can include [!DNL Analytics] events, third-party tags, and custom scripts. This example describes how to set up scripts or third-party tags.

Beyond integrated tools like [!DNL Adobe Analytics] and Google Analytics, Dynamic Tag Management can trigger any type of JavaScript or inject HTML into your site, in select pages or in specific scenarios.

Each rule can trigger as many scripts or HTML injections as you want.

>[!NOTE]
>
>Because DTM allows you to inject custom code into your page, please take care not to create cross-site scripting (XSS) vulnerabilities (see [OWASP’s guide](https://www.owasp.org/index.php/Cross-site_Scripting_(XSS)) for more info). Using data elements within a script requires particular attention. Always assume data element values might come from an untrusted source.

**To set up actions for the condition to trigger** 

1. Click **[!UICONTROL JavaScript / Third Party Tags]** to add a new script to your rule.

   ![](assets/scripts_actions.png){width="200"}

1. Click **[!UICONTROL Add New Script]**.

   ![](assets/scripts_actions2.png){width="472"}

1. Name the script.
1. Specify how you want the script to trigger, and paste the desired content into the text area. ![](assets/scripts_actions3.png){width="472"}

1. Click **[!UICONTROL Save Code]**, and the script will be added to the queue for the rule. ![](assets/scripts_actions4.png){width="472"}
