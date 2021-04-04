---
description: Add header and footer code in Dynamic Tag Management.
keywords: Dynamic Tag Management
seo-description: Add header and footer code in Dynamic Tag Management.
seo-title: Add header and footer code
solution: Experience Cloud
title: Add header and footer code
uuid: f13d5302-3cbc-4b28-9e6a-46184a9770ed
exl-id: 8d7eb39b-86de-4831-bea5-1d82a55eebfd
---
# Add header and footer code{#add-header-and-footer-code}

Add header and footer code in Dynamic Tag Management.

1. Copy the production header code and place it within the [!DNL HEAD] section of your site HTML.

   Place the code as close to the `<head>` tag as possible. This code snippet should be placed on every page of your live production site.

   >[!NOTE]
   >
   >Production embed code reflects only the published items in that [property](../administration/web-property.md#concept_8413810BEAEC4AA48996BE9AFCF141DD). However, embed code for staging reflects all items in the associated property, regardless of the published or unpublished state. To test unpublished items on your production site, locally enable staging in the console by following the instructions in [Test unpublished rules for Akamai hosting](../managing-resources/create-rules/t-test-rules-amazon.md#task_B397167F9E9B4487957AD6CE2AD47259).

1. Copy the production footer code and place it in the [!DNL BODY] section of your site HTML.

   Place the code as close to the `</body>` tag as possible. 
1. Copy the staging header and footer code, then repeat the steps above on your staging site.

   >[!NOTE]
   >
   >The difference between production and staging code snippets is the addition of `-staging` to the filename in the staging version. The footer code remains the same in staging and production.
