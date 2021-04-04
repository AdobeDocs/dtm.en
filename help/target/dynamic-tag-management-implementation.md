---
description: Information to help you properly manage the dynamic tag management embed code while implementing Adobe Target.
keywords: dynamic tag management;Target;integration;implementation
seo-description: Information to help you properly manage the dynamic tag management embed code while implementing Adobe Target.
seo-title: Dynamic Tag Management Implementation
solution: Experience Cloud
title: Dynamic Tag Management Implementation
uuid: 8db85ecb-7d34-4bbc-bee8-19f2a38e9a6c
exl-id: 18b7b85b-f157-4979-9313-18b3e42b307f
---
# Dynamic Tag Management Implementation{#dynamic-tag-management-implementation}

Information to help you properly manage the dynamic tag management embed code while implementing Adobe Target.

Place or move rich data objects before the DTM header embed code in order to leverage them most powerfully in your [!DNL Target] implementation. Although your data layer might continue to grow as the rest of the page loads, anything loaded after the header embed code is not available for use in the global Mbox or other [!DNL Target] requests made at the top of the page. This limits your targeting and segmentation capabilities.

Also, if you use JavaScript libraries, such as jQuery, place them above the DTM header embed code so you can leverage them within [!DNL dynamic tag management] and [!DNL Target].

The following illustration shows sample embed code with a data object and JavaScript library properly configured:

![](assets/embed_code_sample.png)
