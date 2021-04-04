---
description: Describes several troubleshooting scenarios and their solutions and provides a list of Frequently Asked Questions (FAQ).
keywords: Dynamic Tag Management
seo-description: Describes several troubleshooting scenarios and their solutions and provides a list of Frequently Asked Questions (FAQ).
seo-title: Troubleshooting
solution: Experience Cloud
title: Troubleshooting
uuid: 134a3b2e-81e9-4703-a17b-ba4dfc0816db
exl-id: 580ae6e2-7110-493f-a21b-85fd1ecf4edd
---
# Troubleshooting{#troubleshooting}

Describes several troubleshooting scenarios and their solutions and provides a list of Frequently Asked Questions (FAQ).

## View the administrator audit log {#section_658B1D32CDA54D9D89A1A4C238CA8D5F}

In addition to the specific troubleshooting categories listed below, company administrators can view, filter, and export a list of all activities that take place within companies and web properties to which they have access. This feature is helpful both for auditing and troubleshooting purposes.

Click **[!UICONTROL Log]** in the left-hand rail to display the audit log.

For example, you can view and filter by:

* Successful logins 
* Account names 
* IP addresses 
* Companies 
* Web properties (and see who created them and when) 
* Roles

You can also export the log data to .csv.

## Implementation issues {#section_4389E23D85A54D4AA2AFB840CFFD0D3C}

**I see a JavaScript error in my console when I load Dynamic Tag Management.**

There’s likely an issue with your Dynamic Tag Management installation. To view the current installation, right click on any page of the site and click **[!UICONTROL View page source]**. Then type CTRL+F to open the search box and type *`satellite`*. This locates the embed snippets of dynamic tag manager. There should be two instances of these snippets on the page. The first should be right before the `</head>` tag. The second should be right before the `</body>` tag.

Example of Header script:

```
<script src=“//assets.adobedtm.com/aaaabbbcccddddeeee1111222233344445555666/satelliteLib-aaaabbbcccddddeeee1111222233344445555666.js”></script> 
</head> 

```

Example of Footer script:

```
<script type="text/javascript">_satellite.pageBottom();</script> 
</body> 

```

**I get this error: Unexpected token: operator (<) (line: X, col: Y).**

You’ve likely chosen the incorrect setup type for your script. Based on the contents of the script, the editor was expecting HTML, but you set the script to JavaScript or vice versa.

For example: if your script contains `<script>` tags, but you set the script up as JavaScript, you will receive this error when you attempt to save the code.

## Rule issues {#section_C5D17FF9E29B4477B23103B214B66EBC}

**My rule does not fire.**

If your event-based rule does not fire, then there is likely an issue with the selector or condition of the rule. Locate the element on your site where the desired event action occurs, right click and select **[!UICONTROL Inspect element]**. Inspect the highlighted script in the box that opens and ensure you are targeting the correct element. Example:

```
Target element: <div class=’pauseButton’ style=’opacity: 1’>
```

Selector Syntax:

* CSS Selector Syntax: `div.pauseButton OR div[class=’pauseButton’]` 
* Manually assign attributes:

    * Element Tag: `div` 
    * Property: `class` 
    * Value: `pauseButton`

**I suspect that my rules are firing in the incorrect order. Where can I find more information about the load order of rules?**

It is important that rules fire in the correct order. Many problems with rules are the result of rules firing in the wrong order. For more information, see [Load Order for Rules](../managing-resources/rules.md#concept_D355ED29DDDF4725AA201DFF0178699C).

**My rule fires inconsistently.**

There are two possible reasons for a rule to fire inconsistently:

* Does the event action incite a link to load? If so, the rule may not have enough time to fire before the new page loads. You need to check the box within the rule identifier indicating **[!UICONTROL Delay link activation]**. This keeps the activated link from loading until the rule has fired. 
* If the event does not incite a new page load, there may be an issue with bubbling. If the event action can occur on a child or parent item, ensure the button indicating **[!UICONTROL Allow events on child elements to bubble]** is checked. This ensures that the rule fires whether or not the user interacts with the child or parent element.

**My third-party or custom script does not trigger when my page load rule fires.**

Verify what type of script you are using and the load option you have chosen for the rule. If you use sequential HTML, your rule must be set to load at Bottom / Top of Page. The script will not work if the rule is set to load Onload or DOM ready.

**My rule is firing, but my data element won’t populate.**

There’s likely a timing issue. Check and see where the rule is loading; if it’s loading at Top of Page or Onload, then the data element is likely not available yet when the rule fires. Try switching the rule to load at Bottom of Page or DOM Ready. If the data element still does not populate, refer to method for the previous question to ensure the data element is available on the page.

**How can I debug a rule?**

You can use the DTM Switch, browser plugin for easy switching of debug mode and staging mode for Dynamic Tag Management users. It is available for both Google Chrome and Mozilla Firefox. For more information, see [DTM Switch Plugins](../managing-resources/plugins/c-dtm-switch-plugins.md#concept_B46CBAE51A7C47029669CF95DA8A1A98).

Watch an Adobe training video that demonstrates how to debug a rule by using the DTM switch plugins:

>[!VIDEO](https://video.tv.adobe.com/v/17169/)

By then end of this video you should be able to:

* Use the DTM debugging plugin

**Why aren't the variables set in the custom code editor in the Adobe Analytics section of my rule executing?**

When executing variables via the Custom Page Code editor in the [!UICONTROL Adobe Analytics] section of a rule, you must set `linkTrackVars` / `linkTrackEvents` as appropriate for these variables to set in the beacon. When adding variables / events via the rule UI, `linkTrackVars` / `linkTrackEvents` is set for you. However, when adding variables / events via the Custom Page Code editor this must be done manually. For example:

```
s.linkTrackVars = "eVar1" 
s.eVar1 = _satellite.getVar('Title Tag');
```

## Tool issues {#section_A52EEA16E9D84203BD88D96309119CC2}

**When I click an internal link on my site, a new window opens when it should not. How do I control the linker link?**

There is likely a code conflict with the linker link feature. Navigate to your analytics tool within your web property and click the settings gear icon next to the tool. Expand the **[!UICONTROL General]** tab of the settings. Under **[!UICONTROL Global Settings]**, you can control the linker link functionality. From here, you can either turn the linker link feature off or you can set it up to activate / not activate on specific element types or selectors.
