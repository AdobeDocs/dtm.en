---
description: Information to help you use dynamic tag management data elements in your Target implementation.
keywords: dynamic tag management;Target;integration;implementation
seo-description: Information to help you use dynamic tag management data elements in your Target implementation.
seo-title: Using Data Elements
solution: Experience Cloud
title: Using Data Elements
uuid: dd8ce6d4-91b3-4f4d-88fe-803f0b918e03
exl-id: d70832e6-a555-4b40-ab1d-770b7b8971e1
---
# Using Data Elements{#using-data-elements}

Information to help you use dynamic tag management data elements in your Target implementation.

You can use data elements in the rule-editing interface by using the percent sign (%) syntax. Type a percent sign into the field and you will see a drop-down menu appear with the data elements that you created.

![](assets/percent_sign.png)

You can use data elements in custom scripts by using the `_satellite` object syntax: 

```
_satellite.getVar('data element name');
```
