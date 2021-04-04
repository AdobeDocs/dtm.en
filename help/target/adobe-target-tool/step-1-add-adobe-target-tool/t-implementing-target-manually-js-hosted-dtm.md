---
description: Information to help you implement Adobe Target manually by hosting the Target JavaScript Library in dynamic tag management.
keywords: dynamic tag management;Target;integration;implementation
seo-description: Information to help you implement Adobe Target manually by hosting the Target JavaScript Library in dynamic tag management.
seo-title: Option 3  Implement Target Manually with the Target JavaScript Library Hosted by DTM
solution: Experience Cloud
title: Option 3  Implement Target Manually with the Target JavaScript Library Hosted by DTM
uuid: 21f47e48-8601-4b74-b59b-7edf9f49a86c
exl-id: 307703c1-fc49-4fb0-8c16-ece355aa6030
---
# Option 3: Implement Target Manually with the Target JavaScript Library Hosted by DTM{#option-implement-target-manually-with-the-target-javascript-library-hosted-by-dtm}

Information to help you implement Adobe Target manually by hosting the Target JavaScript Library in dynamic tag management.

If you prefer to manage the [!DNL mbox.js] file yourself, but host it within [!DNL dynamic tag management]: 

1. On a property's **[!UICONTROL Overview]** page in [!DNL dynamic tag management], click **[!UICONTROL Add a Tool]**.
1. From the **[!UICONTROL Tool Type]** drop-down list, select **[!UICONTROL Adobe Target]**.
1. In the **[!UICONTROL Tool Name]** box, type "Adobe Target."
1. From the **[!UICONTROL Library Retrieval Method]** drop-down list, select **[!UICONTROL Manual]**.
1. Click **[!UICONTROL Create Tool]**.

   ![Step Result](assets/manual_js.png)

1. Specify your [!DNL Target] Client Code on the resulting screen.

   ![Step Result](assets/manual_js_2.png)

   For information on how to obtain your Client Code, see [Step 1: Add the Adobe Target Tool](../../adobe-target-tool/step-1-add-adobe-target-tool/step-1-add-adobe-target-tool.md#concept-f9bfd490b0264f8693810eaed8a68203). 
1. Expand the **[!UICONTROL Library Management]** section of the page, then select the **[!UICONTROL In DTM]** option from the **[!UICONTROL Code Hosted]** drop-down list within the [!DNL Custom] section.
1. Ensure that the **[!UICONTROL Load Adobe Target Library Synchronously]** option is selected.

   ![Step Result](assets/manual_js_3.png)

1. Click **[!UICONTROL Open Editor]**.
1. Paste in the contents of your current [!DNL mbox.js] file.

   Instructions to download the file can be found in [Download mbox.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) in the *Adobe Classic Product Documentation*.

   ![](assets/manual_js_4.png)

1. Click **[!UICONTROL Save and Close]** in the Editor.
1. Click **[!UICONTROL Save Changes]** on the **[!UICONTROL Adobe Target Tool]** page.
