---
description: Use Dynamic Tag Management to add header and footer code that determines the loading of JavaScript and page content on your site. You must install both the header and footer code on every page of your site, regardless of the hosting option used.
keywords: Dynamic Tag Management
seo-description: Use Dynamic Tag Management to add header and footer code that determines the loading of JavaScript and page content on your site. You must install both the header and footer code on every page of your site, regardless of the hosting option used.
seo-title: Header and footer code
solution: Experience Cloud
title: Header and footer code
uuid: 32fe3d1f-586d-42be-823e-52324664d85a
exl-id: 3e6c0258-9989-4420-aec3-ff4105bcf788
---
# Header and footer code{#header-and-footer-code}

Use Dynamic Tag Management to add header and footer code that determines the loading of JavaScript and page content on your site. You must install both the header and footer code on every page of your site, regardless of the hosting option used.

 >[!VIDEO](https://video.tv.adobe.com/v/17171/)

By then end of this video you should be able to:

* Understand the embedding elements 
* Explain the difference between staging and production 
* Not confuse embedding codes with the s.code

Because Dynamic Tag Management includes a snippet of code in both your header and footer, you can run rules at the beginning or end of a page. This ability allows you to implement testing tools and other technologies while retaining control over tracking your pages.

Dynamic Tag Management creates staging and production embed codes you can use to test your changes in your staging environment before pushing changes to your production environment.

>[!IMPORTANT]
>
>For a successful implementation, it is critical that you follow these instructions as they appear in Adobe Help. Specifically, you must place the header code in the `<head>` section of your document templates. Also, you must place the footer code just before the closing `</body>` tag. Placing either of these embed codes elsewhere in your markup, or using asynchronous methods to append the embed codes, or wrapping the embed codes in any way, are *not* a supported implementations of Dynamic Tag Management. The embed codes must be implemented exactly as provided.

An unsupported implementation will yield unexpected results and prevent Customer Care and Engineering from assisting with your implementation.

Because Dynamic Tag Management includes a snippet of code in both your header and footer, you can run rules at the beginning or end of a page. This ability allows you to implement testing tools and other technologies while retaining control over tracking your pages.
