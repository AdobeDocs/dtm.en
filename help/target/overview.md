---
description: Adobe dynamic tag management (DTM) makes it quick and easy to implement Adobe Target on your websites.
keywords: dynamic tag management;Target;integration;implementation
seo-description: Adobe dynamic tag management (DTM) makes it quick and easy to implement Adobe Target on your websites.
seo-title: Best Practices for Implementing Adobe Target using Dynamic Tag Management
solution: Experience Cloud
title: Best Practices for Implementing Adobe Target using Dynamic Tag Management
uuid: 0d2afb6c-df72-4593-8b21-c701badad2e6
exl-id: 79d83d86-6300-4f77-bddf-9c3167195065
---
# Best Practices for Implementing Adobe Target using Dynamic Tag Management{#best-practices-for-implementing-adobe-target-using-dynamic-tag-management}

Adobe Dynamic Tag Management (DTM) makes it quick and easy to implement Adobe Target on your websites.

<!--
<p>V1.2: Updated to include new instructions for importing the Adobe Target library, built-in methods for adding global mbox parameters, instructions on how to retrieve Client Code, and some updated screenshots. </p>
<p>V1.1: Updated mbox.js section to use the new synchronous-loading option in the Target Tool (the Page Load rule workaround is no longer needed); updated mbox parameters section with new sub-section for DTM-placed. mboxes; updated product names to “Target” and “Target Classic Workflow;” added QA, Approve, Deploy section. </p>
-->

**Last Updated: January 27, 2016**

There are many ways to implement [!DNL Target] depending on your industry and business requirements. Work with your DTM or [!DNL Target] consultant to create your implementation strategy and then use this guide to realize it with DTM.

## Prerequisites {#section-01a87fb6a4944ed99bb17ed6404498f6}

Before following the instructions in this guide, we assume that you have met the following prerequisites: 

<table id="table_A79BD150A4294DB09AAD73CBA0E5BA06"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Prerequisite: </th> 
   <th colname="col2" class="entry"> For more information, see: </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> You have access to the DTM interface. </p> </td> 
   <td colname="col2"> <p> <a href="/help/using/getting-started/get-started.md" format="https" scope="external"> Getting Started </a> in the <i>Dynamic Tag Management Product Documentation</i>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>You have configured the relevant DTM property. </p> </td> 
   <td colname="col2"> <p> <a href="https://docs.adobe.com/help/en/dtm/using/admin/web-property.html" format="https" scope="external"> Web Properties </a> in the <i>Dynamic Tag Management Product Documentation</i>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>You have added the DTM embed code to your website. </p> </td> 
   <td colname="col2"> <p> <a href="https://docs.adobe.com/help/en/dtm/using/client-side/deployment.html" format="https" scope="external"> Embed Code and Hosting Options </a> in the <i>Dynamic Tag Management Product Documentation</i>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>You have a basic understanding of the DTM interface, how to configure rules, etc. </p> </td> 
   <td colname="col2"> <p> <a href="https://docs.adobe.com/content/help/en/dtm/using/dtm-home.html" format="https" scope="external"> Dynamic Tag Management Product Documentation </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>You have access to approve and publish DTM code. </p> </td> 
   <td colname="col2"> <p> <a href="https://docs.adobe.com/help/en/dtm/using/admin/users.html" format="https" scope="external"> Users and Permissions </a> in the <i>Dynamic Tag Management Product Documentation</i>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>You have access to the <span class="keyword"> Target </span> interface. </p> </td> 
   <td colname="col2"> <a href="https://docs.adobe.com/content/help/en/target/using/target-home.html" format="https" scope="external"> Adobe Target Product Documentation </a>. </td> 
  </tr> 
 </tbody> 
</table>

Please check with [Customer Care](https://helpx.adobe.com/contact/enterprise-support.ec.html) or refer to the [Additional Resources](additional-resources.md#concept-96eadfea07c544709d599d9d138a6bf5) section of this guide if you need assistance with any of the above prerequisites.
