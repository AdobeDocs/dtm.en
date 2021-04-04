---
description: Information about creating the Adobe Target tool for deploying Adobe Target in Dynamic Tag Management. You can configure the library automatically (recommended) or manually.
keywords: Dynamic Tag Management
seo-description: Information about creating the Adobe Target tool for deploying Adobe Target in Dynamic Tag Management. You can configure the library automatically (recommended) or manually.
seo-title: Adobe Target tool
solution: Experience Cloud
title: Adobe Target tool
uuid: 06562631-7df3-420d-b787-1ccff774b3b4
exl-id: 497d774e-04d4-497f-a4cb-080aed69e93f
---
# Adobe Target tool

Information about creating the Adobe Target tool for deploying Adobe Target in Dynamic Tag Management. You can configure the library automatically (recommended) or manually.

>[!NOTE]
>
>For best practices, see [Best Practices for Implementing Adobe Target Using Dynamic Tag Management](https://docs.adobe.com/content/help/en/dtm/implementing/overview.html).

*&lt;Web Property Name&gt;* > **[!UICONTROL Overview]** > **[!UICONTROL Add a Tool]** > **[!UICONTROL Adobe Target]**

![](assets/target_tool.png)

## Field descriptions - Add a tool (Adobe Target) {#section_957AFF495DC04E548D0084C0F3063DBF}

The following table describes the fields and options on the [!UICONTROL Add a Tool] page (and the tool edit page) for [!DNL Adobe Target].

* Tool Type
  
  The type of tool, such as [!DNL Adobe Target].

* Tool Name
  
  The name for this tool. This name displays on the [!UICONTROL Overview] tab under [!UICONTROL Installed Tools].

* Library retrieval method
  
  Specifies whether Adobe should manage your [!DNL Adobe Target] code automatically, or whether you would like to provide your own custom code manually.

### Manual configuration method

You can manually manage the [!DNL Adobe Target] code. You can download the [!DNL at.js] or [!DNL mbox.js] file from the Target solution interface as follows:

* Target Standard: **[!UICONTROL Setup]** > **[!UICONTROL Implementation]** > **[!UICONTROL Download at.js]**
* Target Standard: **[!UICONTROL Setup]** > **[!UICONTROL Implementation]** > **[!UICONTROL Download mbox.js]**
* Target Classic: **[!UICONTROL Configuration-]** > **[!UICONTROL mbox.js]** > **[!UICONTROL Download]**

After you download the code locally, copy and paste the code into the editor field in the Library Management section of the tool settings. You have the option of hosting the code at a specific URL as an alternative to manually pasting in the code.

### Automatic Configuration Method

>[!NOTE]
>
>This works for mbox.js only.

Dynamic Tag Management automatically retrieves the latest `mbox.js` code from your [!DNL Adobe Target] account configuration. If you select **[!UICONTROL Automatic]**, you must either be logged in via the Experience Cloud, or you must provide a Client Code value described below.

### Client code retrieval method

(Automatic method) A code unique to your [!DNL Adobe Target] account. It is required for your code to be provided and managed automatically by Adobe. If you chose the Automatic method, you must either be logged in via the Experience Cloud, or provide your Client Code value after selecting **[!UICONTROL Manual]** as the retrieval method.

* Client Code

  (Automatic method) The Client Code value can be retrieved from the [!DNL Adobe Target] solution interface as follows:

    * Target Classic: **[!UICONTROL Configuration]** > **[!UICONTROL mbox.js]** > **[!UICONTROL Edit]** > *copy value for Client*.

    * Target Standard: **[!UICONTROL Setup]** > **[!UICONTROL Implementation]** > **[!UICONTROL Download mbox.js]** > *copy value for Client from within* `mbox.js` *file*.

## Library management - Adobe Target {#concept_DD6234BB44134EE88F7CD67191366CBC}

Descriptions of the fields and options in the Adobe Target Library Management settings in Dynamic Tag Management.

<!--
target_library_management.xml
-->

<!--
<p>TAGS for ditamap </p>
-->

**[!UICONTROL Property]** > **[!UICONTROL Edit Tool]** > **[!UICONTROL Library Management]**

![](assets/target_library.png)

* Load Adobe Target Library synchronously
  This option ensures the `at.js` or `mbox.js` code is loaded synchronously in the `<head>` section. It is generally recommended that you leave this option enabled. It is an [!DNL Adobe Target] best practice to load the code in this way.
* Code Configuration
  **Managed by Adobe:** (`mbox.js` only) This option is equivalent to the Automatic configuration method available when creating the tool. This option loads the `mbox.js` code directly from Adobe.
  This feature optimizes the configuration process when using a manual method, because no more copying or pasting from the [!DNL Adobe Target] admin console is required.
   * You must be logged in via Experience Cloud or have provided the appropriate [Client Code](../tools-reference/target.md#section_957AFF495DC04E548D0084C0F3063DBF) for this option to be available.
   * Clicking **[!UICONTROL Check for Updates]** automatically checks for new versions of the `mbox.js` code within your associated [!DNL Adobe Target] account. If a new version is identified, you have the option to use it or retain the current version.

  **Custom:** You can manually configure the `at.js` or `mbox.js` code. Two methods are available to manually host the code in Dynamic Tag Management:

    * **In DTM:** Click **[!UICONTROL Edit Code]** and paste the code in the editor. If you were using `Managed by Adobe` and switch to `custom`, the editor automatically populates with your `mbox.js` code. You can replace this with the content of the  `at.js` library.
    * **At URL:** If your `at.js` or `mbox.js` is configured as desired, you can provide the URL to the file. Dynamic Tag Management consumes it for use in the [!DNL Adobe Target] tool.

## Global parameters - Adobe Target

Descriptions of the fields and options in the Global Parameters settings in Dynamic Tag Management for an Adobe Target Tool.

<!--
target_global_params.xml
-->

Global parameters let you pass additional data to the global [!DNL Adobe Target] mbox, and also on a per-page basis via page load rules.

The parameters configured in Dynamic Tag Management do not override parameters already defined on the page, but instead appends and sequences to create maximum flexibility and customization on a per page basis.

**[!UICONTROL Property]** > **[!UICONTROL Edit Tool]** > **[!UICONTROL Library Management]**

![](assets/target_global.png)

|Element|Description|
|---|---|
|Name|Indicate the name of the additional parameter(s) you wish to pass to the global mbox.|
|Value|Indicate the value of the additional parameter(s) you want to pass to the global mbox. The value is typically a data element.|

## Mbox rule example for Dynamic Tag Management {#task_2642B010AB204834A2AF7CEACDAC23F7}

An example of how to place wrapping mboxes with built-in flicker handling via Dynamic Tag Management when an Adobe Target tool is installed.

<!--
t_target_example.xml
-->

This functionality currently uses the *`mboxUpdate`* method.

1. Click **[!UICONTROL Property]** > **[!UICONTROL Rules]** > **[!UICONTROL Page Load Rules]** > **[!UICONTROL Create New Rule]**.
1. Name and configure the rule.

   ![Step Info](assets/target_example_1.png)

   Configure the rule so that it fires only on the pages where you want to deploy the mbox.

   >[!NOTE]
   >
   >Adobe recommends load rules triggering mboxes at *`Top of Page`* to ensure the default content is hidden until the mbox response has been received.

   See [Rule Conditions and Functions](../managing-resources/rules.md#reference_662A7B7D177C46C98980CD317A7A8861) for information about available rule criteria.

1. Expand **[!UICONTROL Adobe Target]**.

   ![](assets/target_example_2.png)

   Specify the element to wrap with the mbox using a CSS selector, name the mbox, then configure the timeout if needed. (It is generally recommended to leave this at the default 1500 ms).

1. Configure the parameters you want to add to the [!DNL Target] mbox or to the global [!DNL Target mbox].

   ![Step Result](assets/target_example_3.png)

   In this example, this rule deploys an mbox named `Hero` that wraps a `div` element with an `id` of `hero` and includes an mbox parameter named `Page Name` with a value of `homepage`. It also includes a parameter named `Path` with a value of `home` that it passes to the global mbox.

   ![](assets/target_example_4.png)

   >[!NOTE]
   >
   >You can also use data elements in the parameter UI fields to dynamically populate the value. See [Data Elements](../managing-resources/data-elements.md#concept_8A4591BD0F4241B6925D976482C43CD2) for more information on data elements.
