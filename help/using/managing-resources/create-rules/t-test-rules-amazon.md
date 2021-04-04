---
description: Test unpublished rules from your console if you use Akamai hosting.
keywords: Dynamic Tag Management
seo-description: Test unpublished rules from your console if you use Akamai hosting.
seo-title: Test unpublished rules for Akamai hosting
solution: Experience Cloud
title: Test unpublished rules for Akamai hosting
uuid: bafa70f9-b1a4-43a2-93bf-2b20b9d5b3f5
exl-id: d62fe7f5-5aa1-485a-9c8e-9d099df3a9d9
---
# Test unpublished rules for Akamai hosting{#test-unpublished-rules-for-akamai-hosting}

Test unpublished rules from your console if you use Akamai hosting.

The Switcher plugin is often the easiest way to test. See [Search Discovery Plugins](https://docs.adobe.com/content/help/en/dtm/using/resources/plugins/search-discovery-plugins.html) in the Dynamic Tag Management Product Documentation for more information. 

1. Access your web console on your site and type `localStorage.setItem('sdsat_stagingLibrary', true)`.
1. Press **[!UICONTROL Enter]**.
1. Type `_satellite.setDebug(true)`, then press **[!UICONTROL Enter]**.
1. Refresh the page.

   This action loads your staging library and sets the debugger, so that you can see details of all available (published / unpublished) rules firing on the page. 
1. When finished, run `localStorage.setItem('sdsat_stagingLibrary', false)`, then press **[!UICONTROL Enter]**.
