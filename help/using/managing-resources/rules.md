---
description: Dynamic Tag Management is a rule-based system. It looks for user interaction and associated data. When the criteria outlined in your rules are met, the rule triggers the tool, script, or HTML you identified.
keywords: Dynamic Tag Management
seo-description: Dynamic Tag Management is a rule-based system. It looks for user interaction and associated data. When the criteria outlined in your rules are met, the rule triggers the tool, script, or HTML you identified.
seo-title: Rules
solution: Experience Cloud
title: Rules
uuid: 7faccf41-e378-4673-a182-e7e7d7a54985
exl-id: 9790ddb0-d41b-4bb3-83a7-6d4256a4e7f0
---
# Rules{#rules}

Dynamic Tag Management is a rule-based system. It looks for user interaction and associated data. When the criteria outlined in your rules are met, the rule triggers the tool, script, or HTML you identified.

![](assets/rules.png)

A rule consists of two parts:

| Part | Description |
|---|---|
|Identifier|The identifier is what you want the rule to look for. The identifier you specify depends on the type of rule.|
|Trigger|Triggers occur after a rule's conditions are met. A rule in Dynamic Tag Management can trigger as many discrete actions as you want. For example, a single rule for an e-commerce Thank You page can trigger your analytics tools and third-party tags from a single rule. There is no need to create separate rules for each tool or tag.|

## Types of rules {#section_3D5763DAA6504934A3FAF90BFC1FAE9D}

There are three types of rules in Dynamic Tag Management as well as several default rules:

**Event-based**

Events are where the majority of interactions on sites take place. You can measure and react to these interactions in real-time, without the need for JavaScript.

Event-based rules are executed when visitors interact with on-page elements.

By leveraging in-page interactions and page-level tagging, you can optimize based on things like social media sharing, video interactions, tabbed interfaces, image galleries, and product sorting and filtering.

See [Event-Based Rules Example](../managing-resources/rules.md#concept_649E7BB6A7B3442C8F32F657BED77D54) for an example of how to set your condition to look for clicks on the various tabs on your product pages.

**Page load**

Let you target by URL, site section, or set up scenarios that are independent of the site structure. For example, a page-load rule can load a survey on the fifth page view or in the seventh minute of a visitor’s session.

Advanced page-load rules let you, for example, target specific user segments in rules.

See [Page Load Rules Example](../managing-resources/rules.md#concept_811F4216145A4E3A91190DFFC9C2D223).

**Direct call**

Designed to bypass Dynamic Tag Management event detection and lookup systems.

Direct call rules are ideal for situations where you want to tell Dynamic Tag Management exactly what is happening. Also, they are ideal when Dynamic Tag Management cannot detect an event in the DOM, such as with Adobe Flash.

See [Creating conditions for Direct Call rules](../managing-resources/create-rules/t-rules-direct-conditions.md#task_85EB8F01775A402BA53B8298F0AADA09) for more information and to watch an EnterpriseTV video about direct-call rules.

**Default rules**

When you activate a property, Dynamic Tag Management includes several default rules.

These rules track common interactions with your site and can help you analyze opportunities throughout your site.

Dynamic Tag Management includes the following default rules:

* **Dead Header:** Tracks any clicks on "dead" (i.e. unlinked) header items.
* **Dead Image:** Tracks any clicks on "dead" (i.e. unlinked) images.
* **Download Link:** Tracks any clicks on downloadable site content.
* **Email Link:** Tracks any clicks on linked emails.
* **Orientation Changed:** Tracks any page orientation change (mobile relevant).
* **Outbound Link:** Tracks any clicks on links driving off site.
* **Telephone Dial:** Tracks any click on a phone number.
* **Zoom Changed:** Tracks any change in page zoom.

## New vs existing rules {#section_0B4B7994A4EF47CDAC89DC6B82A3460B}

You can create a new rule or add your script to an existing rule.

In each rule, you might notice that the screens look very similar: the Conditions section is listed first, then any Installed Tools, and finally the JavaScript / Third Party Tags section.

The reason the sections are listed in this order is that the Conditions (the visitor scenario being tracked) are the first things to think about when planning a new rule or a change to an existing rule.

What is the visitor doing? Where is it happening? When is it happening? If the Conditions are the same, if your scenario is the same, then you can add as many tool actions or variables, and as many third party tags as you would like to an existing rule, if one exists with the Conditions you need. If you have a different set of Conditions, you need to create another rule.

For example, if you have a new conversion pixel or tag to place on your site, and you have some existing rules, think about the scenario that must occur for the rule to execute. Consider whether you have a rule in your web property with the condition you need, to execute the conversion pixel. Suppose that you already have a page-load rule for your purchase confirmation page, and you are loading three conversion pixels in the JavaScript / Third Party Tags section. You can add your new pixel as a new Script in the same section of that rule, without creating a new rule.

If the Conditions are different, then you need to add a new rule.

## Event-based rules example {#concept_649E7BB6A7B3442C8F32F657BED77D54}

An example of how you to use event-based rules in click-tracking for a tabbed interface on a product page.

<!--

rules_event.xml

 -->

When using event-based rules, it helps to have some knowledge of CSS selectors so that you can identify elements on the page.

The [!UICONTROL CSS Selector] lets you quickly and easily select CSS elements to use as triggers for event-based rules without leaving the DTM rule builder. For more information, see [Using the CSS Selector](../managing-resources/create-rules/t-rules-event-conditions.md#concept_DDF500DCB8214658AEDECDE69ED1D4AF).

The following links are useful resources to learn about CSS:

* [CSS Selector Pattern Matching Syntax](https://www.w3.org/TR/CSS2/selector.html#pattern-matching)
* [CSS Selector Reference](https://webplatform.github.io/docs/css/selectors/)

![](assets/create_event_based.png){width="472"}

Set up how to track this click in [!DNL Adobe Analytics].

![](assets/tracking.png){width="472"}

If you also have Google Analytics or any other platforms installed, you can leverage the same rule to configure or send data to as many platforms as you want.

![](assets/google_analytics.png){width="472"}

When using event-based rules, Dynamic Tag Management offers powerful tools to surface data from the page and page elements with which the user interacts.

**DTM Basics: Event-Based Rules, Part One**

>[!VIDEO](https://video.tv.adobe.com/v/17172/)

By then end of this video you should be able to:

* Understand what an event-based rule is
* Explain the event-based rule types
* Create an event-based rule

**DTM Basics: Event-Based Rules, Part Two**

>[!VIDEO](https://video.tv.adobe.com/v/17173/)

By then end of this video you should be able to:

* Understand what an event-based rule is
* Explain the event-based rule types
* Create an event-based rule

**DTM Basics: Event-Based Rules, Part Three**

>[!VIDEO](https://video.tv.adobe.com/v/17174/)

By then end of this video you should be able to:

* Understand what an event-based rule is
* Explain the event-based rule types
* Create an event-based rule

## Page load rules example {#concept_811F4216145A4E3A91190DFFC9C2D223}

You can implement rules that trigger during the course of a page load. For example, you can display a survey after a certain number of page views, or after a specified number of minutes into a session. Page load rules let you target by URL, site section, or set up scenarios that are independent of the site structure.

<!--

rules_page.xml

 -->

**DTM Basics: Page Load Rules, Part One**

>[!VIDEO](https://video.tv.adobe.com/v/17177/)

By then end of this video you should be able to:

* Understand what a page load rule is
* Understand the condition criteria options
* Create a page load rule

**DTM Basics: Page Load Rules, Part Two**

>[!VIDEO](https://video.tv.adobe.com/v/17178/)

By then end of this video you should be able to:

**Google AdWords example**

A marketer would like to trigger a Google AdWords conversion tag when a user fills out a form and arrives on the page `https://www.mysite.com/form/thank-you.html`

Here is how you can set up this scenario in Dynamic Tag Management:

1. Create a new page load rule.

   ![](assets/page_load_rules.png){width="472"}

1. In the rule conditions, specify the page where this rule will be triggered.

   ![](assets/rule_conditions.png){width="472"}

1. Paste the tag your vendor gave you directly into the Third-Party Tags section.

   Because Dynamic Tag Management does not rely on templates, marketers can use any tag within a rule, even in formatted HTML.

   ![](assets/3rdparty_script.png){width="472"}

1. Give your rule a name that describes the user interaction like “Forms: User submits form.”

   You can also add descriptive metadata to your rule.

   This description will help you and others identify this rule if they want to use it for their tags or tools later.

1. Save your rule, and you are ready to test it in a staging environment, request rule approval, and publish to the production site.

   ![](assets/edit_page_load_rule.png){width="472"}

   >[!NOTE]
   >
   >By default, page load rules load at page bottom. This setup works for most scenarios. However, if the rule you are setting up has some dependency on in page content, it might be better to configure the rule to load on DOM ready. Conversely, if you have other rules that rely on the outcome of the rule in question, load the rule at Top of Page or Onload to ensure that it fires first.

## Page load rules - advanced {#section_7F8213A984D6447BA54DE188BA4F17EA}

<!--

rules_page_adv.xml

 -->

This example shows how to deliver an A/B test to users on iPads.

You may want to target specific user segments in your rules. The following example shows how you can deliver an A/B test to a form, using a segment specific to users on iPads who have been on our site for more than fifteen minutes and came to the site through Google search.

1. Create the conditions.

   The following image shows the setting you use for this visitor segment:

   ![](assets/rule_condition_2.png){width="472"}

1. Set up a test on the form using Adobe Target.

   You are not required to modify the page, and there are no mbox containers to place in your markup.

   ![](assets/adobe_target.png){width="472"}

1. Click **[!UICONTROL Save]**, configure your test in Adobe Target and your test is running.

   ![](assets/marketing_cloud_login.png){width="200"}



## Rule conditions and functions {#reference_662A7B7D177C46C98980CD317A7A8861}

Describes all Dynamic Tag Management rule conditions and their functions.

<!--

r_rules_conditions.xml

 -->

## Custom script in a rule condition {#section_9F2E0BD2AC844531840010CF8792A299}

When using custom code in rule conditions for a page load rule, you must use the boolean `return true` when you want the rule to fire.

## Conditions and functions {#section_198A5095854F415C86ABBA9165D53370}

The following table describes condition types, conditions, functions, and applicable notes:

<table id="table_375815C6BDBD4209BF7D72667774512B">
 <thead>
  <tr>
   <th colname="col1" class="entry"> Condition Type </th>
   <th colname="col2" class="entry"> Condition </th>
   <th colname="col3" class="entry"> Function </th>
   <th colname="col4" class="entry"> Notes </th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colname="col1"> <p>URL </p> </td>
   <td colname="col2"> <p>Protocol </p> </td>
   <td colname="col3"> <p>Indicate rule to fire on HTTP or HTTPS. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Subdomain </p> </td>
   <td colname="col3"> <p>Indicate rule to fire or not fire on specified subdomain(s). </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Path </p> </td>
   <td colname="col3"> <p>Indicate rule to fire or not fire on specified URL path(s). </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. The path condition functions based on the <span class="codeph"> _satellite.data.URI</span>, which is inclusive of query params. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Parameter </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if specific URL parameter(s) with specific values are present. </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> <p>Technology </p> </td>
   <td colname="col2"> <p>Cookie Opt-out </p> </td>
   <td colname="col3"> <p>Indicate rule to fire only if user accepts cookies based on presence of <span class="codeph"> sat_track</span> cookie that is set to "true" </p> </td>
   <td colname="col4"> <p>Requires data element setup. Cookie can be given custom name on the <span class="wintitle"> Edit Property</span> page. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Browser </p> </td>
   <td colname="col3"> <p>Indicate rule to fire only in specified browsers. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Operating System </p> </td>
   <td colname="col3"> <p>Indicate rule to fire only in specified operating systems. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Screen Resolution </p> </td>
   <td colname="col3"> <p>Indicate rule to fire within specified screen-resolution ranges. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Window Size </p> </td>
   <td colname="col3"> <p>Indicate rule to fire within specified window-size ranges. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> <p>Engagement </p> </td>
   <td colname="col2"> <p>Traffic Source </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if visit came from specified source. </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Landing Page </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if visit landed on specified page(s). </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>New/Returning Visitor </p> </td>
   <td colname="col3"> <p>Indicate rule to fire only if new/returning visit. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Sessions </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if visitor has had &gt;, =, or &lt; specified number of sessions. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Page Views </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if visitor has had &gt;, =, or &lt; specified number of page views in this session or all sessions. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Time on Site </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if visit persists for specified # of minutes. </p> </td>
   <td colname="col4"> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Registered User </p> </td>
   <td colname="col3"> <p>Indicate rule to fire based on user registration status as indicated in data element. If the indicated data element has a value, then the condition evaluates as "true" (does not include the default value). </p> </td>
   <td colname="col4"> <p>Requires data element setup. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Logged In </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if user is / is not logged in as indicated in data element. If the indicated data element has a value, then the condition evaluates as "true" (does not include the default value). </p> </td>
   <td colname="col4"> <p>Requires data element setup. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Previous Converter </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if user is / is not a previous converter as indicated data element. If the indicated data element has a value, then the condition evaluates as "true" (does not include the default value). </p> </td>
   <td colname="col4"> <p>Requires data element setup. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Cart Item Quantity </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if user has certain number of items in cart as indicated in data element. </p> </td>
   <td colname="col4"> <p>Requires data element setup. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Cart Amount </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if user has certain dollar value in cart as indicated in data element. </p> </td>
   <td colname="col4"> <p>Requires data element setup. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> <p>Data </p> </td>
   <td colname="col2"> <p>Cookie </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if specified cookie with specified value is present. </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Data Element Value </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if specified data element with specified value is present. </p> </td>
   <td colname="col4"> <p>Requires data element setup. Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Variable Set </p> </td>
   <td colname="col3"> <p>Indicate rule to fire if specified JS object with specified value is present. It may be necessary to prefix the object path with the appropriate scope depending on the scenario - 'this.', 'event.', 'target.', 'window.', or 'param.' </p> </td>
   <td colname="col4"> <p>Enable regex on this condition to include multiple scenarios in a single condition. </p> </td>
  </tr>
  <tr>
   <td colname="col1"> </td>
   <td colname="col2"> <p>Custom </p> </td>
   <td colname="col3"> <p>Opens a blank text box to input custom script. </p> </td>
   <td colname="col4"> </td>
  </tr>
 </tbody>
</table>
