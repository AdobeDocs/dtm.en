---
description: Historical release notes for Dynamic Tag Management.
keywords: Dynamic Tag Management
seo-description: Historical release notes for Dynamic Tag Management.
seo-title: Previous release notes
solution: Experience Cloud
title: Previous release notes
uuid: 3e92cd1b-83ad-429e-a9a2-0616394a1949
exl-id: 424e68ab-c456-4e51-b21a-16cc55d59e06
---
# Previous release notes{#previous-release-notes}

Historical release notes for Dynamic Tag Management.

 See [Current Release Notes](../whatsnew.md#concept_424EB048942A44F9AFD46E18A08AA563) for the latest release information.

## April 21, 2016 {#section_65017B66787F4873AD700A7E1B7CD744}

The April 21, 2016 Dynamic Tag Management release includes the following changes:

**New Features** 

<table id="table_ABDB182F090A4E22B5402F50AA55BD34"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Experience Cloud navigation and menu changes </p> </td> 
   <td colname="col2"> <p>As part of the Adobe Experience Cloud Spring 2016 release, a new-top level navigation menu displays at the top of all solution interfaces. The new interface lets you: </p> 
    <ul id="ul_1FC6D539533144938C412655B4A6E807"> 
     <li id="li_2ACACDD55B35474E831BAF6460393063"> <p><b>Single-click navigation between solutions: </b>Choose your own default landing page or take advantage of the solution-switcher widget. </p> </li> 
     <li id="li_46AE604DDA104A7691E98C1F826D988E"><b>Improved notifications: </b>Get notified about events (like posts, mentions, assets shared, system updates) happening across your organization navigation widget. </li> 
     <li id="li_0A997CB2292E4C7297466B9101C35F62"> <p><b>Updated Feed: </b>We reimagined the Feed page to become a better platform for cross-channel collaboration between marketers. </p> </li> 
    </ul> <p>See <a href="https://docs.adobe.com/content/help/en/id-service/using/release-notes/notes-2016.html" format="https" scope="external"> What's New in the Adobe Experience Cloud - Spring 2016 </a> in the <i>Experience Cloud and Core Services Product Documentation</i>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## March 30, 2016 {#section_6C1A5B787D0747C6A205CEAD3A19F3EF}

March 30, 2016

The March 30, 2016 Dynamic Tag Management release includes the following changes:

**New Features** 

<table id="table_438F642203C1407692E97F04831AA82B"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>CSS Selector </p> </td> 
   <td colname="col2"> <p>Use the <span class="wintitle"> CSS Selector </span> to quickly and easily select CSS elements to use as triggers for event-based rules without leaving the DTM rule builder. </p> <p>See <a href="../managing-resources/create-rules/t-rules-event-conditions.md#concept_DDF500DCB8214658AEDECDE69ED1D4AF" format="dita" scope="local"> Using the CSS Selector </a>. </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <p>Restrict tool access using user groups </p> </td> 
   <td colname="col2"> <p>Use group membership to restrict the ability for users to create or modify tools and related tool settings in rules. </p> <p> See <a href="../administration/groups.md#task_D08D33C542C444469636CA288B631FB5" format="dita" scope="local"> Create a New Group </a>. </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <p>Restrict login to Experience Cloud </p> </td> 
   <td colname="col2"> <p>Use the <span class="wintitle"> Restrict to Experience Cloud </span> option to force all users in the company to log in to <span class="keyword"> Dynamic Tag Management </span> using <span class="keyword"> Adobe Experience Cloud </span> credentials rather than using the legacy/company login process. </p> <p>See <a href="../administration/users.md#concept_2FA1011890C04E59845E8EB1E2345488" format="dita" scope="local"> Users and permissions </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

## February 4, 2016 {#section_1276153E14E7462F91B3FC11CE883370}

The February 4, 2016 Dynamic Tag Management release includes the following changes:

**Fixes and Enhancements:** 

* Fixed an issue that prevented a rule from firing when using the [!UICONTROL Element Exists] event with the [!UICONTROL Manually Assigned Properties & Attributes] option. (DTM-6681) 

* Fixed an issue that caused the [!UICONTROL Enter Viewport] trigger condition to not be respected by all rules that match the same HTML element. (DTM-7108) 
* Fixed an issue that caused pages to unload with a jQuery undefined error message. (DTM-7116) 
* Fixed an issue that sometimes caused the [!UICONTROL Original] and [!UICONTROL Modified] editor views seen during the approval process to contain mismatched content. (DTM-7180) 

* Fixed an issue that caused an MCID authentication error when working with data elements. (DTM-7233)

## January 14, 2016 {#section_68CCCE27734848F794C828C40E258A06}

The January 14, 2016 Dynamic Tag Management release includes the following changes:

**New Features** 

<table id="table_67315B8232244A44BFF409EF4C49605E"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Admin notifications for property publishes </p> </td> 
   <td colname="col2"> <p>Administrators can now receive an email notification when one of their web properties is published. The email contains the time and name of the property. </p> <p>See <a href="../getting-started/get-started.md#task_BEC6AC7A5DB542CB9B442D318A0E0305" format="dita" scope="local"> Manage Account Settings </a>. </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <p>Relative hostnames </p> </td> 
   <td colname="col2"> <p>You can specify relative hostnames for staging and production library hosting. </p> <p>See <a href="../client-side-information/deployment.md#task_A7B37CB2C89941A4A4D1F9AF06FC493D" format="dita" scope="local"> FTP </a> and <a href="../client-side-information/deployment.md#task_B7A42F3B1D3E4B71B0BADD17C181F22A" format="dita" scope="local"> Library Download </a>. </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <p>Nielsen tool </p> </td> 
   <td colname="col2"> <p>You can enable Nielsen tracking using Dynamic Tag Management by creating the Nielsen tool and configuring the page code either automatically or manually. The automatic method is recommended for most users. </p> <p>See <a href="../tools-reference/nielsen.md#concept_697E539912154172A3BE804DD2401534" format="dita" scope="local"> Add Nielsen Tool </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Fixed an issue when using multiple custom event rules that caused only the first rule to fire. (DTM-7026) 
* Fixed an issue that prevented the main library from loading for certain customers. (DTM-7130) 
* Fixed an issue with Internet Explorer 9 that caused the Nielsen time-spent-on-page counter to remained paused after the browser or browser tab loses and then regains focus. (DTM-7033) 
* In Internet Explorer 8, the non-human detection mechanism in forms malfunctions. Because IE8 is no longer supported this issue will not be fixed. Please upgrade your browser if this is an issue for you. (DTM-7101)

## November 17, 2015 {#section_663B52500EEA43E4866CBAF3004B9C3A}

The November 17, 2015 Dynamic Tag Management release includes the following changes:

**New Features** 

<table id="table_C7FD6C1A3043434BBDAB32FF299A9B46"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>New event types for event-based rules </p> </td> 
   <td colname="col2"> <p>Added the following new event types for event-based rules: </p> 
    <ul id="ul_083C71EFF676438F986658053467CBB5"> 
     <li id="li_0D9995E0EDAE472E81E8070E8182EAE6">Other &gt; time passed </li> 
     <li id="li_72ACA443ECC6411C92E1F3C0DB207B16">Browser &gt; tab focus </li> 
     <li id="li_82A3C177501E4C0797873D9AFD928EF8">Browser &gt; tab blur </li> 
    </ul> <p>For more information, see <a href="../managing-resources/create-rules/t-rules-event-conditions.md#concept_B1C6169D8B354207AEE0E4965E6421B1" format="dita" scope="local"> Event Types </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Fixed an issue that caused Dynamic Tag Management to throw a fatal error on Microsoft Internet Explorer 8. DTM-7022

## September 22, 2015 {#section_43A0700440D64A5CB46EFF80A5FE4404}

The September 22, 2015 Dynamic Tag Management release includes the following changes:

**New Features** 

<table id="table_11D4DC80E91E4F27BC65AE0065AB8860"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Experience Cloud Visitor ID Service Tool </p> </td> 
   <td colname="col2"> <p>The newest library version (1.5.2) will enable improved customer ID support, added support for authenticated state and improved multi-solution integration. </p> <p>The newest version is completely compatible with current deployments of the Experience Cloud Visitor ID Service via DTM. To help all users benefit from this update we will automatically migrate your account to the new Experience Cloud ID Service library. </p> <p>As a result of this migration you will see added functionality to your Experience Cloud Visitor ID Service tool in DTM. We suggest that you test this update in your staging environment before publishing. </p> <p>The DTM team strives to add value for our customers, and we are confident that you will see this realized in the update to the Experience Cloud Visitor ID Service tool. </p> <p>For more information, see <a href="../tools-reference/macid.md#concept_FB6CB6A0E6CC4F10B92371F8671F6B59" format="dita" scope="local"> Marketing Cloud ID Service Settings </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Fixed an issue when editing user groups that caused user groups from other companies to be removed. 
* Fixed a security concern with rules using non-sequential HTML code. Please re-publish your web properties for the fix to take effect.

## September 3, 2015 {#section_95B2708228B44CDAACB9E403D2B6B145}

September 17, 2015

**New Features** 

<table id="table_081A4FF9BE064901805E0F50372E11BA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Group management </p> </td> 
   <td colname="col2"> <p>Group management makes it easy to organize users and control their access levels. Permissions are set at the user group level, so all users in the group inherit the group permissions, including access to properties. </p> <p>For more information, see: </p> <p> 
     <ul id="ul_F0B80B5A6DC64FB0AD540828F8F8656D"> 
      <li id="li_50701AD2B60B4314894D97B885057A2C"> <a href="../administration/groups.md#concept_6494F1EF2400457ABCED8D860951CD36" format="dita" scope="local"> Create and Manage Groups </a> 
       <ul id="ul_889F771E61D842139DCA3D486CAA551E"> 
        <li id="li_F16D38BC8FF1414C899BB4E0028D9D7F"> <a href="../administration/groups.md#task_1A482EF670454416A9664CF668A7CC3B" format="dita" scope="local"> Add Users to Groups </a> </li> 
        <li id="li_CAD81F9C59C145A0A9FE4CFBBC38BDA4"> <a href="../administration/groups.md#task_D08D33C542C444469636CA288B631FB5" format="dita" scope="local"> Create a New Group </a> </li> 
        <li id="li_84EFABCF48D8432DA9B3DB30FADA1B91"> <a href="../administration/groups.md#task_2E0A2D7D793845818C586943C7FA3F7F" format="dita" scope="local"> Edit a Group </a> </li> 
        <li id="li_9195FAE6E51645E5A6FE63B861F74275"> <a href="../administration/groups.md#task_CFAA137ED18D4363B1826DF504CF993F" format="dita" scope="local"> Delete a Group </a> </li> 
       </ul> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Improved the deployment of the satellite library (2-5 times speed increase). Customers with many rules or who are deploying many third-party tags will greatly benefit from these changes. 
* Improved the upload speed to Akamai (up to 5 times faster). 
* Improved the load speed (2 times faster) for all rule listing pages. 
* Fixed an issue that prevented some pages from loading in Internet Explorer (users received a pop-up error message).

## July 8, 2015 {#section_A602779958934D75BD68BEDA861A1DFE}

**New Features and Enhancements** 

<table id="table_24D086E97FE94BF697A35EB4818E6D41"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Event Types </p> </td> 
   <td colname="col2"> <p>New event types let you trigger event-based rules on Single Page Apps: </p> <p>New event types include <span class="wintitle"> "Custom" </span> and " <span class="wintitle"> pushState or hashchange </span>." </p> <p>See <a href="../managing-resources/create-rules/t-rules-event-conditions.md#concept_B1C6169D8B354207AEE0E4965E6421B1" format="dita" scope="local"> Event Types </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Fixed an issue in the Google Universal Analytics tool that prevented users from setting the account ID in data elements. 
* Fixed an issue in the Google Universal Analytics tool that suppressed rule beacons if the [!UICONTROL Page Code is Already Present] check box is selected.

## July 8, 2015 {#section_BBB3D1DF8AFA434188E1F10D139F364A}

The July 8, 2015 Dynamic Tag Management release includes the following changes:

**New Features and Enhancements** 

<table id="table_7CE66B92C8C1407185AB0E42DCB4972F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Event Types </p> </td> 
   <td colname="col2"> <p>New event types let you trigger event-based rules on Single Page Apps: </p> <p>New event types include <span class="wintitle"> "Custom" </span> and " <span class="wintitle"> pushState or hashchange </span>." </p> <p>See <a href="../managing-resources/create-rules/t-rules-event-conditions.md#concept_B1C6169D8B354207AEE0E4965E6421B1" format="dita" scope="local"> Event Types </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Fixed an issue in the Google Universal Analytics tool that prevented users from setting the account ID in data elements. 
* Fixed an issue in the Google Universal Analytics tool that suppressed rule beacons if the [!UICONTROL Page Code is Already Present] check box is selected.

## June 8, 2015 {#section_42BD325419FC40AD9D6AB274A544646F}

The June 8, 2015 Dynamic Tag Management release includes the following changes:

**Fixes and Enhancements:** 

* Fixed an issue in some iOS Safari browsers that produced an error when localStorage options are restricted by a user.

## April 23 2015 {#section_A22902A85E214E2B8372E18C3A42CD93}

The April 23, 2015 Dynamic Tag Management release includes the following changes:

**New Features and Enhancements** 

<table id="table_DD11E40E3B374620911CF73E8D7AC8D1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Data Elements </p> </td> 
   <td colname="col2"> <p>Enhancements to data elements include the following: </p> 
    <ul id="ul_F75AC88ECFEE4D33B52DF15731C40C02"> 
     <li id="li_B24FC472DD47472FBD54C9D80D4039E1"> <p>Users can now copy data elements across web properties and companies. </p> </li> 
     <li id="li_C56FAEE318DA4ED7B1515CFC888142C1"> <p>Users can now bulk copy, activate, deactivate, and delete data elements. </p> </li> 
     <li id="li_F9959DDF3B36412495F90387D0DDA4CA"> <p>Users can now select a <span class="wintitle"> cleanText </span> option when setting a data element. </p> <p>This option causes Dynamic Tag Management to remove beginning and ending whitespace and replace all whitespace in the middle of return values with a single space. This option is useful to normalize data element values for easier matching. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## April 7 2015 {#section_C68605C95266442F96B2C9ED8D7451A0}

**New Features and Enhancements** 

<table id="table_9E69FDEC1ACF454F85222967F813827C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Selective Publish </p> </td> 
   <td colname="col2"> <p>When creating a web property, the <span class="wintitle"> Enable Selective Publish </span> option is set by default. </p> <p>See <a href="../administration/web-property.md#task_AE34E23EC47B4E9C8634782C05D9DC09" format="dita" scope="local"> Create a web property </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Enhancements:** 

* Added localization enhancements for the [!DNL Adobe Analytics] tool UI (Premium, Standard, and Point). 
* Updated the favicon icon that displays in browsers' address bars to match new Adobe branding.

## March 24 2015 {#section_D993CD80D56D4583AB927095E0E9BB84}

**New Features and Enhancements** 

<table id="table_3CA51E873E324FD4B7CF14190F127A77"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <p>Integration with Adobe Analytics Premium </p> </td> 
   <td colname="col2"> <p>If you are an <span class="keyword"> Adobe Analytics Premium </span> customer, Dynamic Tag Management lets you take advantage of advanced features and additional eVars and events. </p> <p> <p>Note:  If you do not use the <span class="wintitle"> Automatic </span> configuration method, Dynamic Tag Management will treat you as an <span class="keyword"> Adobe Analytics Standard </span> account. </p> </p> <p>See <a href="../tools-reference/analytics-dtm.md#concept_FBA6679A0B79490F8296437F11E5E4F8" format="dita" scope="local"> Add Adobe Analytics Tool </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes:** 

* Updated the variable and event interface for the [!DNL Adobe Analytics] tool to allow auto-complete selection and to enable access to additional eVars and events for [!DNL Analytics Premium] accounts. See [Add Adobe Analytics Tool](../tools-reference/analytics-dtm.md#concept_FBA6679A0B79490F8296437F11E5E4F8).  

* Fixed an issue where the [!UICONTROL Store Path] option for FTP library deployments wasn’t updating for production libraries when using nested directories.  
* Updated data elements to support hyphenated names. 
* Fixed an issue where the column indicator in the [!UICONTROL Rules] table displayed for a rule, even if the tool was deleted.  
* Updated the [!UICONTROL Sequential HTML] code option to be available for page-load rules only. This option no longer appears for event-based rules. A notice displays with a [!UICONTROL Sequential HTML] tag on an event-based rule to notify users to change the tag before the rule can be saved.  

* Fixed an issue where the [!UICONTROL Sign in with Adobe ID] login option wasn’t allowing users to sign in as a different user. Users can click [!UICONTROL Sign in with a Different Adobe ID] to log out as the current [!DNL Experience Cloud] user and be redirected to the Adobe login page.

## February 10 2015 {#section_6C569C52357B425D95FE0ACA830852E7}

Fixes:

* Added a deprecation warning message for all company administrators using Amazon hosting for their JavaScript library. 
* Improved the error handling for instances where [!DNL document.write] is not available. 
* Addressed various localization issues to increase the user experience for supported languages. 
* Fixed an issue where the [!UICONTROL Channel] field wasn’t included in rules specifying a `s.tl()` call in [!DNL Adobe Analytics]. 

* Fixed an issue where copied rules weren’t automatically added to the staging library until a change was made to the rules. 
* Fixed an issue where Regex was firing for rules using the “parameters” condition option, even if the parameter wasn’t present.

## January 13 2015 {#section_1413A743D84E4BF29C1691DD1940261D}

Fixes:

* Dynamic Tag Management no longer overrides global variables with the name *`window.t`*. 
* Fixed an issue where Firefox was incorrectly trapping the right-click event handler in the browser and causing click-based rules to fire.

## November 13 2014 {#section_19318A60F7294D1080CFAEED5A1CBCD6}

<table id="table_F710029AC6A4459796FBE37123BC5BB9"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Adobe improved our Dynamic Tag Management integration with <span class="keyword"> Adobe Media Optimizer </span>, including. </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4C7FCE04C76C4ED5A905AC86A91F3410"> 
      <li id="li_2DE6639F266341ACB28C3085D40E23DD">Default delivery of the latest (v3) Media Optimizer tag </li> 
      <li id="li_FD124B85067942E38778009F922841E6">Support for a data-element based SKU </li> 
      <li id="li_BB6976ABFC544641BAB942BD315B6320">Suppression of unneeded beacons </li> 
      <li id="li_F93BBA71B3E5498C9229B0F25575201B">Minor enhancements </li> 
     </ul> </p> <p>See <a href="../tools-reference/media-optimizer.md#concept_1A33BC0F5B6A4709929EC6F876236657" format="dita" scope="local"> Adobe Media Optimizer Settings </a> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Improvements**

* Fixed an issue where rule copying did not work after the release of the [!DNL Adobe Media Optimizer] integration on 10/30/2014.  
* Added the ability to specify name/value pairs for general settings and customer-specified IDs in the Experience Cloud ID tool. 
* Added option for the Experience Cloud ID tool to trigger the initial API call. This call enables support for Adobe solutions that do not currently trigger this call already in your own code. 
* Fixed an issue where the browser version tracked by Dynamic Tag Management for certain versions of Internet Explorer was returned as *`Unknown`* instead of *`Internet Explorer`*.  

* Adobe tools will now be displayed first in the listing of installed tools on a given web property.

## October 30 2014 {#section_3112A307294B43AB98C67EA407654225}

Adobe improved our Dynamic Tag Management integration with [!DNL Adobe Media Optimizer], including:

* Default delivery of the latest (v3) Media Optimizer tag 
* Support for a data-element based SKU 
* Suppression of unneeded beacons 
* Minor enhancements

## October 28 2014 {#section_D901228AACEF4A779FF101994E2D8886}

New features in Dynamic Tag Management released on October 28, 2014:

<!-- 

<p>Hid privacy management xml. </p>

 -->

<table id="table_F87E6CF4603B463EA7B7CD877FA256C9"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Adobe Target integration </p> </td> 
   <td colname="col2"> <p>Updated the <span class="keyword"> Adobe Target </span> tool to enable automatic deployment via Dynamic Tag Management. </p> <p>See <a href="../tools-reference/target.md#concept_90D4021A9B6E409D8101FA1AFADE1215" format="dita" scope="local"> Adobe Target Settings </a> for configuration information. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Enable support for Google Universal Analytics Premium features </p> </td> 
   <td colname="col2"> <p>Added a checkbox for premium Google Universal Analytics features in the tool (General group). This option enables the max dimensions and metrics increase from 20 to 200. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes and Improvements**

* Fixed an issue where the Tracking Server value automatically determined by Dynamic Tag Management for the [!DNL Adobe Analytics] tool sometimes set an incorrect value.  
* Fixed an issue where a restored data element had the name appended with "(Restored)," which caused previous references to that data element to be broken. (The appended value is now added only if restoring the data element would create a naming conflict with an existing data element.) 
* Fixed an issue caused when triggering an event-based rule on a click event. If the click event had a delay link activation on an anchor tag with no HREF, the issue forced the browser to attempt to navigate to a blank HREF location. 
* Fixed an issue where Dynamic Tag Management was no longer saving global variables configured in an Analytics tool when changes to that tool had been rejected and then restored. 
* Implemented significant performance improvements in the library generation process, which should result in a shorter wait for changes to appear in production, especially during peak usage hours. 
* Fixed an issue where company administrators were unable to export their activity log to CSV when there was a large amount of data present. 
* Added the ability to use custom HTML data attributes with CSS selector-based data elements.

## August 21 2014 {#section_82776A5125824EB89EBFFA1ADCB1808F}

Fixes and improvements:

* The help landing for Dynamic Tag Management is now at:

  [https://docs.adobe.com/content/help/en/dtm/using/dtm-home.html](https://docs.adobe.com/content/help/en/dtm/using/dtm-home.html)

  Please update your bookmarks accordingly. 

* Fixed an issue where re-enabling a previously disabled property caused all approved items to be immediately published. A property will now be enabled, but published assets will not be affected until a publish request is explicitly requested by a user with appropriate permissions. 
* Fixed an issue where custom code editors in Dynamic Tag Management were truncating the last few lines of displayed code. 
* Fixed an issue where reverting a tool to a previous version did not revert all settings for that tool. 
* Users can now force a data element's value to be automatically converted to lowercase before it is returned and used. 
* Fixed issue where a race condition in the Dynamic Tag Management engine prevented data from being sent correctly to audience management.

## August 7 2014 {#section_3E4A1A7F537B4E4EBFC34D106BA557C4}

New features: 

<table id="table_37894582D32549959E712BD120D8CA4F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud ID Service </p> </td> 
   <td colname="col2"> <p>You can automate the deployment of the <span class="keyword"> Experience Cloud </span> ID Service using Dynamic Tag Management. </p> <p>See <a href="https://docs.adobe.com/content/help/en/dtm/using/tools/macid.html" format="https" scope="external"> Experience Cloud ID Service </a> in <span class="term"> Dynamic Tag Management Help </span>. </p> </td> 
  </tr> 
 </tbody> 
</table>

Fixes and improvements:

* The help landing for Dynamic Tag Management is now at:

  [https://docs.adobe.com/content/help/en/dtm/using/dtm-home.html](https://docs.adobe.com/content/help/en/dtm/using/dtm-home.html)

  Please update your bookmarks accordingly. 

* Fixed an issue where reverting an [!DNL Analytics] account to a previous version resulted in a 404 error. 
* Fixed an issue where Approvers trying to view details on a previous version, while reviewing an approvable item, were unable to expand the appropriate sections. 
* Added support in [!DNL Adobe Analytics] tool configuration for visitor namespace. 
* Upgraded the code editor used throughout Dynamic Tag Management, which provides additional features, including support for extra-long lines of code. 
* Fixed an issue where events set in the [!DNL Analytics] rule UI were not being sent as part of data collection when the rule was set to use *`s.t()`*. 

* Fixed an issue where the Force Lowercase option was not working in Google Universal Analytics. 
* Fixed an issue where the default value was not returned when specifying a DOM element that did not have the attribute defined as specified in the CSS selector for the data element. 
* Fixed an issue where reverting an [!DNL Analytics] tool to a previous version did not revert all elements of that account, resulting in a mixture of old and new settings for the tool.

## July 24 2014 {#section_E4C035C5DA204B6D9EC559FAA7DC6886}

New features: 

<table id="table_72AEAD70FA57480A9AB73178A01C81D9"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="keyword"> Adobe Analytics </span> account and report suite synchronization. </p> </td> 
   <td colname="col2"> <p>Report suites are automatically synchronized via a <span class="keyword"> Experience Cloud </span> login or Web Services ID. </p> <p>Once the accounts are connected, Dynamic Tag Management pulls the <span class="keyword"> Adobe Analytics </span> report suite IDs and names into the tool configuration interface, allowing for increased speed in tool deployment with less possibility for user errors. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Adobe managed measurement library option. </p> </td> 
   <td colname="col2"> <p>You can let Dynamic Tag Management loads and manage the base library directly. You no longer need to cut and paste library code from the <span class="keyword"> Adobe Analytics </span> administration tools. This feature also makes upgrades to new versions of <span class="keyword"> AppMeasurement </span> easier, because the base code and custom code are stored separately. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Custom Code timing. </p> </td> 
   <td colname="col2"> <p>You can now select whether you want the code in the <span class="keyword"> Adobe Analytics </span> code panel to fire before or after the interface settings for more implementation flexibility. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Interface improvements. </p> </td> 
   <td colname="col2"> <p>The groups ( <span class="wintitle"> General </span>, <span class="wintitle"> Library Management </span>, and so on) on the <span class="wintitle"> Tools </span> page for <a href="../tools-reference/analytics-dtm.md#concept_FBA6679A0B79490F8296437F11E5E4F8" format="dita" scope="local"> Adobe Analytics </a> has been reorganized and streamlined to simplify configuration. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Latest Links**

See [FAQ for Adobe Analytics Release - July 24 2014](../tools-reference/analytics-dtm.md#concept_3C2761855B2D49DEBFAD8E2F7BB78003) for questions and answers.

See [Adobe Analytics Settings](../tools-reference/analytics-dtm.md#concept_FBA6679A0B79490F8296437F11E5E4F8) for configuration information.

## July 10 2014 {#section_7307DD6B68AF4476B68FDFB603EB1A29}

Features and fixes: 

<table id="table_3407164F92994CC6B61C53AC3CE34362"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Audit Log for Administrator </p> </td> 
   <td colname="col2"> <p> 
     <!--https://issues.adobe.com/browse/DTM-4124-->Click <span class="uicontrol"> Log </span> in the left-hand rail to view the <span class="wintitle"> Audit Log </span> page. </p> <p>Company administrators can view, filter, and export a list of all activities that take place within companies and web properties to which they have access. This feature is helpful both for auditing and troubleshooting purposes. </p> <p>For example, you can view and filter by: </p> 
    <ul id="ul_0A061552FD114DB9AC37768F7BF15379"> 
     <li id="li_73BE05A762874D698297471414A184AC">Successful logins </li> 
     <li id="li_4C56B6A981D04BD8A74E3324C3FBCE16">Account names </li> 
     <li id="li_4E400DB82FD94039AAC29A4862586421">IP addresses </li> 
     <li id="li_B102DDE78BB844F1B8E73B84DD34F082">Companies </li> 
     <li id="li_68D7E01FF4984ABFBCA082A1A274190C">Web Properties (and see who created them and when) </li> 
     <li id="li_0D9890DBCA1D4E8EAE960D98E099D0F7">Roles, and more. </li> 
    </ul> <p>You can also export the log data to <span class="filepath"> .csv </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Language Selector </p> </td> 
   <td colname="col2"> <p> 
     <!--https://issues.adobe.com/browse/DTM-4150-->Dynamic Tag Management is now available in the same languages (English, French, Spanish, German, Korean, Portuguese, Japanese, Traditional Chinese, and Simplified Chinese) as the rest of the <span class="keyword"> Experience Cloud </span>. </p> <p>In <span class="wintitle"> Account Settings </span>, click the <span class="uicontrol"> Languages </span> menu to specify the language. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Synchronous loading of the <span class="keyword"> Adobe Target </span> tool. </p> </td> 
   <td colname="col2"> 
    <!--<p>https://issues.adobe.com/browse/DTM-3949</p>--> <p> To enable this feature: </p> 
    <ol id="ol_744EDD6EB086483E94D38C3668DD51BD"> 
     <li id="li_839766A434044B81BBE7393DD8596AC6">Navigate to the <span class="wintitle"> Target </span> tool configuration page. </li> 
     <li id="li_329369BDD8E945EEB5147A4FF4E5F739">Enable <span class="uicontrol"> Load Adobe Target Library synchronously </span>. </li> 
    </ol> <p>Note:  This value is enabled by default for new instances of the <span class="keyword"> Adobe Target </span> tool, and disabled by default for existing instances of the tool. </p> <p>Existing instances of the <span class="keyword"> Adobe Target </span> tool will continue to load asynchronously until you change the setting to <span class="term"> synchronous </span>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes**

* Fixed an issue where disabling and then enabling a property caused the items in the approvals queue to be automatically published by the system when the property was re-enabled. 
* Added a message to the [!UICONTROL Embed] tab for company administrators. This message is a reminder that no code is published to the production environment until someone explicitly clicks **[!UICONTROL Publish]**. This fix was done to help avoid confusion by some users who were seeing *`404 Not Found`* errors on the production library, because they had not yet published. 

* Fixed an issue where duplicate registrations were possible for the same user using a differing case. (For example, [!DNL user@DOMAIN.com] vs [!DNL user@domain.com]). 

* Fixed an [!DNL Adobe Analytics] issue that prevented you from re-adding or editing an *`eVar`* or *`prop`* value after deleting that specific variable or property. 

* Fixed an issue where rejecting an approved or published tool, and then updating that tool, did not cause a new entry to be generated in the approvals queue. 
* Fixed an issue where the [!DNL Adobe Analytics] tool configuration options for *`Always Track`* and *`Never Track`* did not emit the correct values to the library and therefore did not have any effect on data collection. 

* Fixed an issue where entering invalid regular expressions caused a broken interface and required you to reload the page. 
* Google Analytics event tag: Fixed an issue where a *`Fill in all fields`* error appeared on a rule, but you were unable to save the rule or make any additional edits and was required to reload the page.

## May 15 2014 {#section_AD67AC3BCE334DF9A7624EE7F97BDE98}

Fixes and improvements for May 15, 2014:

* Fixed an issue where variables set in custom code were not being set on direct call or event-based rules using [!DNL s.t()]. The code contained within the custom code area for direct call or event-based rules using [!DNL s.t()] was not correctly adding any variables set to the beacon before an image request was being fired. 

* Fixed and issue where the command bar was sticking to the bottom of the [!UICONTROL Approvals] page. The persistent bar with the Edit and Reject commands on the [!UICONTROL Approvals] page was sticking to the bottom of the page rather than following the page view upon scroll. 

* Fixed an issue on the [!UICONTROL Rule List] page, where a newly created rule showed [!DNL Adobe Analytics] in use, even if those rules were not using [!DNL Adobe Analytics]. 

* Fixed layout issues on [!UICONTROL Selective Publish] queue page. We cleaned up the layout so that it is not truncated or stretching beyond the boundary of the content area of the page. 
* Data elements now display in alphabetical order in the Data Element Value criteria of a rule. They have now been alphabetized for easier viewing. 
* The items on the publish history are now paginated to improve performance and user experience. 
* Added password security enhancements. To ensure the security for Dynamic Tag Management accounts, we have implemented a number of enhancements to our authentication system:

    * New passwords must meet specific criteria (minimum 7 characters, at least one number, at least one letter, at least one symbol, not one of the last 5 passwords). 
    * Company admins can now see how long it has been since a user last changed their password. 
    * Company admins can now force users to reset their password. 
    * Users attempting to log in 5 times unsuccessfully will be locked out for 30 minutes to prevent brute force attacks (the user or their company admin can reset the password to re-enable access immediately).

## May 8 2014 {#section_8F8F5385C7B549F59F78CCFB2443237E}

Fixes for May 8, 2014:

* Fixed an issue where *`trackingServer`* value was not being applied consistently. The value for *`s.TrackingServer`* should be used consistently for all types of calls throughout Dynamic Tag Management, and the value should be pulled either from the custom code or from the UI, depending on the configuration of a specific web property. (The UI value takes precedence if set in both locations.) 

* Fixed an issue where properties with a large number of items awaiting approval was causing 500 errors and timeouts. We optimized the queries for the approvals workflow to ensure that properties with a large number of items awaiting approval would load quickly and not result in timeouts, errors, or broken pages. 
* Fixed an issue where pages with an existing object called 's' would cause errors in Dynamic Tag Management. Dynamic Tag Management tries to initialize an 's' object on the page for [!DNL Adobe Analytics] tracking, and this was causing a conflict if [!DNL Analytics] was implemented via Dynamic Tag Management and the *`Page code already exists`* box was not checked. The object is now locally scoped within Dynamic Tag Management, so it will work in any custom code scenarios but will not conflict with any on-page code. 

* We made a number of improvements to the way that hierarchies are managed in [!DNL Adobe Analytics] tools and rules, including ensuring that non-sequential hierarchies could be used together in a tool or rule, and ensuring that the same hierarchy could not be set more than once in a tool or rule.

## April 28 2014 {#section_72C1A347664C43C8A30C4B8AACA400B7}

Fixes for April 28, 2014

* Fixed an issue where direct call and event-based rules that were configured to send a page view (using [!DNL s.t()]) were not executing custom code.

## April 17 2014 {#section_7D43ABB68A4343229D22AFA1FC4DC1FE}

Fixes for April 17, 2014

* Fixed an issue in which an error displayed when you delete data elements that were associated with rules that had already been deleted. 
* Fixed an issue in which deleted data elements were still shown in the menu when you add a condition to a rule based on a data element. 
* Fixed an issue where fields and values for Google Universal Analytics rules were showing as *`modified`* in the Approval view, even if the rules had not been changed. This issue also occurred on new rules. 
* Fixed an issue where the Google Universal Analytics tool configuration allowed you to configure the cookie timeout in milliseconds, even though Google Universal Analytics does not support this. 
* Changed *`AdLens`* to *`Media Optimizer`*. 

* Users can now use the % syntax to view the pop-up list of data elements when sending values to [!DNL Media Optimizer]. 
* Modified styling on tool lists to better accommodate tools with long names, and to improve readability.

## April 8 2014 {#section_C66A861824D748468B1E232F419DE3A4}

Fixes for April 8, 2014

* Fixed the styling on the [!UICONTROL Forgot Password] page to improve appearance. 
* Fixed an issue where approved/published rule conditions were being removed from production library upon deletion in staging. 
* Fixed an issue where the [!UICONTROL Actions] menu on the [!UICONTROL Rule List] page was being cut off at the bottom, if there were less than three rules being displayed. 

* Fixed alignment for the Create Data Element button on the [!UICONTROL Data Elements] page. 
* Fixed alignment for the Create New Schedule button on the [!UICONTROL Scheduling] page. 
* Fixed an issue where long rule names were breaking the [!UICONTROL Selective Publish] page. 
* Fixed an issue where deleting [!UICONTROL Adobe Analytics] variable values would, in certain cases, result in a broken UI that required a page refresh to fix.

## April 3 2014 {#section_9B1C47B7F3E94CEFAA184EBF21C4640B}

Features for April 3, 2014 

<table id="table_4EBB9309D60144EF9BEE0B1CECB774A7"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Google Universal Analytics support. </p> </td> 
   <td colname="col2"> <p> Added native support for <a href="../tools-reference/google-universal-analytics.md#concept_224428EBB8E4466B93328EC5AE87FF04" format="dita" scope="local"> Google Universal Analytics </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Upgrade from Google Analytics to Google Universal Analytics </p> </td> 
   <td colname="col2"> <p> Integrated the Airlock JS library to perform automatic translation of all existing GA calls to Google Universal Analytics. </p> </td> 
  </tr> 
 </tbody> 
</table>

Fixes for April 3, 2014:

* Fixed an issue where clicks were not being tracked in certain scenarios when the **[!UICONTROL Page code is already present]** box was enabled in the [!DNL Adobe Analytics] tool configuration. 

* Fixed an issue where all approvables were being deployed in staging, rather than just the ones that were added or modified. This issue potentially resulted in delays to seeing staging updates. 
* Fixed an issue where *`linkTrackVars`* and *`linkTrackEvents`* were being overwritten by rules, rather than appending to existing values (such as those set in [!DNL s_code]). 

* Fixed an issue where use of special characters (such as brackets) in data element names caused exceptions when you edited the data element. 
* Fixed an issue where a lengthy shared secret for library download bundles caused exceptions (showed as a 500 Server Error). 
* Fixed an issue where the *`cookieLifetime`* variable was being emitted to the library with incorrect capitalization, causing the corresponding setting from the interface to be disregarded when the page was loaded.

## March 11 2014 {#section_23FFF5B7457E4D16B68FCB2FAD803972}

Fixes for the March 11, 2014 release:

* Fixed issue where test files ( [!DNL ftp_test.txt]) were being left on FTP/SFTP servers after upload was complete. This file is now deleted once the upload is complete as it is only used to test the ability to validate user credentials and is not actually needed by Dynamic Tag Management. 
* Fixed issue where custom port for FTP/SFTP was not being saved.

## March 6 2014 {#section_B0BBF310B0384B2CA7C2878374CD0C6A}

Features and fixes for the March 6, 2014 release: 

<table id="table_25F7951BC85D4A52B0BA129366795D31"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Added support for SFTP. </p> </td> 
   <td colname="col2"> <p> Dynamic Tag Management now supports transmitting published files to a client's server via secure FTP (SFTP). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Added support for hierarchy delimiters. </p> </td> 
   <td colname="col2"> <p> A delimiter can now be specified when hierarchies are used in a rule that sends data to <span class="keyword"> Adobe Analytics </span>. (Previously, the behavior was that all hierarchies were comma-delimited, and any other delimiter required use of custom code.) </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes**

* Fixed issue with SVG images in older IE browsers. SVG images that were clicked in older IE browsers (prior to IE version 9) caused errors and would sometimes cause the browser to crash. 
* Fixed issue with custom links in direct call rules. Using custom links in direct call rules would generate a JavaScript error in the browser. 
* Fixed issue with data element rule conditions referencing the wrong name. If a user renamed a data element, and the data element was being referenced in a rule condition, the rule would try to use the most recently specified name for that data element. This issue occurred even if the name change had not yet been published. 
* Fixed issue where elements without an HREF attribute caused errors when clicked. This issue is regarding the "linker link" functionality in the Dynamic Tag Management engine, which attempts to automatically track any clicked elements on the page. Elements without an HREF were generating errors. The "linker link" code now checks that the element is an anchor tag before attempting to track clicks on it.

## February 4 2014 {#section_2922AFC3900442B8A93599278A53E3B9}

Fixes for the February 4 2014 release: 

<table id="table_DA582EE212AC44CAADAB7157753DF38E"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Fixed issue with invalid URLs being accepted in web property configurations. </p> </td> 
   <td colname="col2"> <p> Users were able to enter invalid URLs on a web property. Valid URLs are now required. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Fixed issue with port being stripped from deploy hook URL. </p> </td> 
   <td colname="col2"> <p> The deploy hook URLs containing a non-default port would have the port removed before the HTTP call was made. This issue resulted in deploy hook notifications being sent to the wrong URL. </p> </td> 
  </tr> 
 </tbody> 
</table>

## January 28 2014 {#section_2FF720E76F66441FB2461F6F51254910}

Fixes for the January 28 2014 release: 

<table id="table_BE6F737B192B45709528399817545994"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Fixed an issue with <span class="keyword"> Adobe Analytics </span> variables overwriting one another in the interface. </p> </td> 
   <td colname="col2"> <p>A user attempting to set multiple <span class="keyword"> Adobe Analytics </span> variables would see variables being overwritten unintentionally. (For example, a user sets prop22, then sets prop2. Prop22 disappears and prop2 contains wrong value.) </p> <p>Note:  This issue was visible in the interface but did not affect existing code or data collection. In other words, if you did not see the variable being overwritten before you saved the rule or tool configuration, then you were not affected by this issue. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Fixed an issue with long account IDs causing tools list to be truncated on right side. </p> </td> 
   <td colname="col2"> <p> Having a long account ID for one or more tools on a web property would cause the tools list to be truncated, making it impossible to then edit that tool. </p> </td> 
  </tr> 
 </tbody> 
</table>

## January 21 2014 {#section_94F6A239E28D4D19AEC92FE16D6A5572}

Fixes for the January 21 2014 release: 

<table id="table_4D6405F818C3402D8EAD1F71663607D5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Fixed UI bugs with Scheduling feature. </p> </td> 
   <td colname="col2"> <p> The Scheduling feature had a number of UI bugs relating to element styling, etc. which have now been fixed. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> User can now correctly set global campaign in <span class="keyword"> Adobe Analytics </span> tool. </p> </td> 
   <td colname="col2"> <p> Fixed issue where campaign values set in the <span class="keyword"> Adobe Analytics </span> tool were not being retained when the tool was saved. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Fixed formatting of tool-tips. </p> </td> 
   <td colname="col2"> <p> Fixed display formatting issues relating to tool-tips. </p> </td> 
  </tr> 
 </tbody> 
</table>

## January 16 2014 {#section_80F6D89166164A5180A302C10352576C}

Fixes for the January 16 2014 release: 

<table id="table_9D724C54CCC74048800AA396C7558BD1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Akamai hosting is the default embed option for new web properties. </p> </td> 
   <td colname="col2"> <p> Dynamic Tag Management is migrating from Amazon S3 to Akamai as the primary external hosting option in efforts to provide Dynamic Tag Management customers a more reliable hosting experience. We encourage all current customers utilizing Amazon S3 hosting to transition to Akamai as soon as possible, so that they may take advantage of increased performance due to Akamai's globally distributed network. </p> <p> All <i>new companies</i> created after January 15, 2014 will have Akamai as their external hosting option by default. </p> <p> Companies created prior to January 15, 2014 will be able to choose between Akamai and Amazon S3 until this option is deprecated on December 31, 2014. Any new <i>properties</i> created within Dynamic Tag Management companies that existed prior to January 15, 2014 will also have the option of choosing between Amazon S3 and Akamai. </p> <p>For information about migrating from Amazon S3 to Akamai, see <a href="../client-side-information/deployment.md#concept_722B01555D0441ACBB052BC34DC5B67D" format="dita" scope="local"> Akamai Hosting </a> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Paginated user lists. </p> </td> 
   <td colname="col2"> <p>User lists for companies and web properties are now paginated (if the company or web property has more than 25 users). This change was done to improve both user experience and platform performance. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Company administrators may delete web properties. </p> </td> 
   <td colname="col2"> <p> Use caution when taking this action, because deleting the web property removes all tools, rules, and settings and <b>cannot be undone</b>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Multiple rules containing custom <span class="keyword"> Adobe Analytics </span> code now fire correctly. </p> </td> 
   <td colname="col2"> <p>Previously, if multiple page load rules fire and they all had custom code for <span class="keyword"> Adobe Analytics </span>, only one of the rules would take effect. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Batch deactivation of rules now working. </p> </td> 
   <td colname="col2"> <p>Fixed an issue that was causing batch deactivation of rules to show as having taken effect in the UI, but were not actually deactivated in the library. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Login page reskin. </p> </td> 
   <td colname="col2"> <p> Login via Adobe ID now looks identical to the login page for <span class="filepath"> marketing.adobe.com </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Opt-out of nonessential emails. </p> </td> 
   <td colname="col2"> <p> Users will now see an option on their <span class="wintitle"> Account Settings </span> page to opt out of non-essential emails, such as approval and publish notifications, note creations, and so on. Essential emails, such as invitations to new companies, properties, and password resets are still sent. </p> </td> 
  </tr> 
 </tbody> 
</table>

## November 19 2013 {#section_34D659DD33DA4A979D1A50F09D07C7FE}

The following table provides information about release notes and fixes for this release. 

<table id="table_AD256DE453434852A5802C40FD058456"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Data elements not working correctly in <span class="keyword"> Target </span> rules </td> 
   <td colname="col2"> Fixed an issue where a data element reference in a Target rule was rendering the literal value (e.g. <span class="filepath"> "%FirstName%" </span>) on the request instead of the substituted value returned from the data element. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Invalid regex causing library save to fail </td> 
   <td colname="col2"> Fixed an issue where an invalid regular expression used in rule criteria would cause the library updates to not be successfully saved. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> New property for engine: <span class="filepath"> isStaging </span> </td> 
   <td colname="col2"> Added a new property to the engine ( <span class="filepath"> _satellite.isStaging </span>). This property indicates whether the staging library is the library loaded on the current page. <p> <span class="term"> True </span> indicates staging library loaded. </p> <p> <span class="term"> False </span> indicates production library loaded. </p> </td> 
  </tr> 
 </tbody> 
</table>

## November 12 2013 {#section_27E2F918217B40289D8A8D83B9F7DE5A}

The following table provides information about release notes and fixes for this release. 

<table id="table_DEDC94234D1C4AE39298D614090FF940"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Deleted tools are no longer visible in rules. </td> 
   <td colname="col2"> Fixed an issue where tools that had been deleted were still showing up in the <span class="wintitle"> Rules </span> tab. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Time On Site criteria now allows for conditional operators. </td> 
   <td colname="col2"> Previously, the Time On Site criteria allowed you to specify only an exact number of minutes to match. Time on Site now supports greater than (&lt;) and less than (&gt;) for increased control over time based scenarios. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Adobe Analytics rules may now use events 76 - 100. </td> 
   <td colname="col2"> Previously, the interface showed events 1 - 75. Now, support is available for events 76 - 100 to match the capabilities available in <span class="keyword"> Analytics </span>. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> New <span class="keyword"> Analytics </span> installed tools with no <span class="filepath"> s_code </span> will not show error. </td> 
   <td colname="col2"> <p> Previously, when creating a new <span class="keyword"> Analytics </span> tool instance, if you did not add <span class="filepath"> s_code </span> to the tool, you would see a 403/Forbidden error displayed in the console. This error occurred because Dynamic Tag Management was requesting a file that did not exist. </p> <p>Now whenever an <span class="keyword"> Analytics </span> tool is created, the <span class="filepath"> s_code </span> is pre-populated with helpful comments and a call to the Satellite engine notification system. The result displays a message in the console, which instructs you to install <span class="filepath"> s_code </span> to complete the implementation. </p> </td> 
  </tr> 
 </tbody> 
</table>

## October 30 2013 {#section_0C2E1A15E5134E4AAC4857BE896C3AEA}

The following table provides information about release notes and fixes for this release. 

|  Fixed Issue  | Description  |
|---|---|
|  Interaction required to save a rule.  | A user must click in a field or make a change to a rule before the Save button is activated. Otherwise, to leave a rule without making changes, you must click Cancel.  |
|  Errant text appearing on selective publish UI in Firefox.  | Fixed an issue where text was being displayed (when it shouldn't have been) at the end of each row in the selective publish UI in Firefox only.  |
|  Buttons for approval modal are not centered.  | Centered the Yes/No buttons in the approval confirmation modal window.  |
|  Sidebar collapse icon not appearing correctly in Firefox.  | The icon that appears to the left of the breadcrumbs allowing a user to collapse/expand their sidebar was not displaying correctly in Firefox. It should now be displaying correctly.  |
|  Company admin can see who invited a user.  | Administrators can now see the name of the person who invited a particular user to their company (if the person who invited the user is an Adobe employee, the admin will simply see *`DTM Admin`* in place of the name).  |
|  Adding Target arguments breaks rule formatting.  | Fixed an issue where a user adding arguments to a rule containing an [!DNL Adobe Target] tool would see an incorrectly formatted/broken UI  |

## October 23 2013 {#section_690C73B992F24F51930F4D2351BEBA13}

The following table provides information about release notes and fixes for this release. 

<table id="table_21E65D8BAE8642129A477ED9FAAD2BD4"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Timestamps embedded in the <span class="codeph"> _satellite </span> object for publish and build. </p> </td> 
   <td colname="col2"> <p>Whenever a new version of the library is published, the <span class="codeph"> _satellite </span> object will now contain two new properties: </p> <p> <b>publishDate</b>: The user requested the publish to happen (the same date/time that appears in the History section of the UI). </p> <p> <b>buildDate</b>: The file was created by our server processes. The difference between the two can be used to troubleshoot potentially processing latency issues. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>New tools and data elements can be created with the same name as those of deleted tools and data elements. </p> </td> 
   <td colname="col2"> <p> Previously when a tool or data element was deleted, you could not create a new tool or data element with that same name. Now, after a tool or data element has been deleted, a new one can be created with the same name. </p> <p>If the original is later restored, "(restored)" is appended to the name to avoid naming conflicts. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Left navigation sidebar is now collapsible </p> </td> 
   <td colname="col2"> <p>An icon appears next to the breadcrumb header at the top of the page allowing the user to toggle the left navigation sidebar on and off. The interface remembers the your preference. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Adding <span class="keyword"> Target </span> arguments breaks rule formatting. </p> </td> 
   <td colname="col2"> <p> Fixed an issue where a user adding arguments to a rule containing an <span class="keyword"> Adobe Target </span> tool would see an incorrectly formatted/broken UI. </p> </td> 
  </tr> 
 </tbody> 
</table>

## October 15 2013 {#section_29D2522B00CA46828C1C9B1FD6AE8530}

The following table provides information about release notes and fixes for this release. 

<table id="table_8F30285C7DD24624B922C74DB576B656"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <p> Breadcrumb wrapping incorrectly in Chrome </p> </td> 
   <td> <p> The breadcrumb display at the top of the page was wrapping incorrectly in Chrome on certain types of pages. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Rule page pagination </p> </td> 
   <td> <p> Rule pages will now show only 25 rules per page and will require users to "page through" to see the full list. This is being done both for user experience and for performance reasons (it's less stressful on the server to produce a list of 25 rules vs. several hundred in the case of some of our clients). </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Rule page filtering </p> </td> 
   <td> <p> A user can now filter the rule page by the name of the rule or the name of third party tags contained within a rule. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Tool approvals </p> </td> 
   <td> <p> Tools in Dynamic Tag Management (Analytics, Target, AdLens, Audience Manager, Google Analytics, etc.) are now part of the approval workflow. New tools, modifications to existing tools, or removals of tools will require approval before they are published to production. Users can now add/modify/delete tools (previously users of type "user" were not able to do this). </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Engine shows Analytics instead of SiteCatalyst </p> </td> 
   <td> <p> When looking at debug messages from the Dynamic Tag Management engine, it now says "Adobe Analytics" instead of "SiteCatalyst" for any messages relating to the Analytics product and its associated rules. </p> </td> 
  </tr> 
 </tbody> 
</table>

**See Also**

[Previous Release Notes](../other-resources/release-notes-history-dtm.md#concept_F63E33A02ED04FFEB92D4763A84DEEF0) for historical Dynamic Tag Management release notes.

## September 30 2013 {#section_6377C2B9AA354BB8B5034DFA6D4660E1}

The following table provides information about release notes and fixes for this release. 

<table id="table_38AC407AD8C84605BC648BD5F2AA9131"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fixed Issue </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <p> New properties do not require approval </p> </td> 
   <td> <p> New web properties used to require approval by a superadmin. In order to expedite provisioning of new accounts, we have removed the requirement for this approval so that new properties are automatically approved and instantly available. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> User views dashboard </p> </td> 
   <td> <p> This pertains to the above story about automating new property approval. Superadmins used to have a section called "Pending Activation" on their dashboard; this story was to remove that section since it's no longer needed. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Enable rule copy for all company admins </p> </td> 
   <td> <p> Company admins now have the same ability as superadmins to copy rules across any companies/properties they have access to. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Changing type of data element retains previous values </p> </td> 
   <td> <p> When changing the type of a data element previously, it used to retain some of the old parameters specified by the user. We're now clearing all parameters and ensuring that the library only contains whatever parameters are relevant to the currently selected type. </p> </td> 
  </tr> 
  <tr> 
   <td> <p> company admin resends invitation email </p> </td> 
   <td> <p> Added the ability to click a "Resend" link in the Users tab for a company in case a user didn't receive their invitation e-mail for some reason. (Previously this required revoking the invite and recreating it from scratch) </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Default selector for linker link rule not being emitted to library </p> </td> 
   <td> <p> The "linker link" rule for Google Analytics was not emitting a selector to the library by default, so it was trying to attach linker link functionality to all clicked page elements. We're now correctly defaulting it to "a" (all links). </p> </td> 
  </tr> 
 </tbody> 
</table>
