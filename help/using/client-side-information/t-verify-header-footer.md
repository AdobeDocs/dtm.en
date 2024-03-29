---
description: Verify that your Dynamic Tag Management library is loading properly on your site.
keywords: Dynamic Tag Management
seo-description: Verify that your Dynamic Tag Management library is loading properly on your site.
seo-title: Verify header and footer code
solution: Experience Cloud
title: Verify header and footer code
uuid: e1c3e381-4118-4696-a5f1-4a2dae156517
exl-id: 65d6c59a-2a76-40f8-97e9-d8e00ac49c90
---
# Verify header and footer code{#verify-header-and-footer-code}

Verify that your Dynamic Tag Management library is loading properly on your site.

1. Open your site in your browser.
1. Open the [!UICONTROL Developer Console] by right-clicking and choosing **[!UICONTROL Inspect Element]** > **[!UICONTROL Console]**.
1. Press **[!UICONTROL Enter]**.

   If the code was properly installed, you will see *`true`* display in the console.

   If the code was not properly installed, you will see the reference error:

   `_satellite is not defined`

   If you receive this error, ensure that:

* You have included the full header code on every page of the site in the [!DNL HEAD] section, as close to the `<head>` tag as possible.
* You do not have unexpected characters appearing in the code snippet, potentially as a result of copying and pasting from a formatted document.
