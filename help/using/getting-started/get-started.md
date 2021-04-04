---
description: Information for new users of Dynamic Tag Management.
keywords: Dynamic Tag Management
seo-description: Information for new users of Dynamic Tag Management.
seo-title: Getting started with DTM
solution: Experience Cloud
title: Getting started with DTM
uuid: 93a3054a-0db9-4dbb-9b12-9f69c7696102
exl-id: 768668ab-f4aa-425e-8961-bb222c12afaf
---
# Getting started with DTM{#getting-started-with-dtm}

Information for new users of Dynamic Tag Management.

## Requesting access to Dynamic Tag Management {#section_9E826B582D0F4712ACD5FC9EDEC3BDC2}

Before you start using Dynamic Tag Management, someone from your company must request access. Please contact your Adobe account team and ask for access to Dynamic Tag Management. Your account team will use our internal Provisioning Hub tool to grant access. You should receive your login credentials within one to two business days.

If you have access to the [!DNL Adobe Experience Cloud], you can also request access to Dynamic Tag Management from the [!UICONTROL Tools] menu. 

![](assets/cloud-login.png){width="318px"}

>[!NOTE]
>
>Administrators, see [Getting Started in the Experience Cloud](https://docs.adobe.com/content/help/en/core-services/interface/manage-users-and-products/admin-getting-started.html) if you need access to the Experience Cloud.

## Logging in {#section_88F2816938E94085A30745905D38731A}

Browse to [https://dtm.adobe.com](https://dtm.adobe.com).

## Getting started tasks {#section_43ACA8689DAB4865895EFE47D0667A50}

The steps below help you get up and running with Dynamic Tag Management:

### Create a web property.

Location: Web Properties tab on the Dashboard

A web property is a library of rules and one embed code. A web property can be any grouping of one or more domains and subdomains. You can manage and track these assets similarly. For example, suppose that you have multiple websites based on one template and you want to track the same assets on all of these websites. You can apply one web property to multiple domains.

For general information about web properties and best practices, see [Web Properties](../administration/web-property.md#concept_8413810BEAEC4AA48996BE9AFCF141DD).

To get started, see [Create a web property](../administration/web-property.md#task_AE34E23EC47B4E9C8634782C05D9DC09).

### Configure your hosting options.

Location: Embed tab

Dynamic Tag Management provides a number of options to host the required JavaScript files:

* Akamai 
* Self-hosting: FTP Delivery 
* Self-hosting: Library Download

See [Embed Code and Hosting Options](../client-side-information/deployment.md#concept_09612483C4934E16B20F5E9DA3B7EB7D).

### Add header and footer code to each managed page.

Location: Embed tab

Dynamic Tag Management allows you to precisely time the loading of JavaScript and page content in your page. You can choose to run rules at the beginning or end of a page. This allows you to implement testing tools and other technologies, while retaining full control over tracking your pages.

Adobe provides staging and production embed code so you can test your changes in your staging environment before pushing changes to your production environment.

See [Header and Footer Code](../client-side-information/deployment.md#concept_3F6A0A508F294FCBABEBA1DF540B781B).

### Deploy tools for solutions.

Location: Overview tab

Tools let you quickly integrate [!DNL Adobe Experience Cloud] solutions on your site. Tools go beyond a basic tag, because they provide additional configuration options. A tool corresponds to Adobe solutions like Analytics and Target, as well as Google Analytics. After you add a tool to a property, it is available for inclusion in a rule.

See [Tools (Overview Tab)](../managing-resources/tools.md#concept_19C5BCE1F99E4EACBD4EA2D61F265184).

### Create data elements, and create rules, conditions, and actions.

Location: Rules tab

Data elements are the building blocks for rules. Data elements let you create a data dictionary (or data map) of commonly used items on a page, regardless of where they originate (query strings, URLs, or cookie values) for any object that is contained on your site. You use data elements to build a data layer that can be used in rules for [!DNL Analytics] and other data collection tools.

Rules can be triggered at page load or when a specific event occurs. Dynamic Tag Management provides a powerful conditioning interface that provides granular control of when tags fire.

To get started, you should set up a basic page-load rule with no conditions to collect analytics data on all pages.

For more information, see [Data Elements](../managing-resources/data-elements.md#concept_8A4591BD0F4241B6925D976482C43CD2) and [Rules](../managing-resources/rules.md#concept_2D3F296DD3BD418BAB7A0E2415DD9C92).

### Publish tools and rules to the production server.

After a rule is created, it is funneled through a multi-step approval process before it is published to a production environment.

See [Rules](../managing-resources/rules.md#concept_300552C4F89E418F94A4D755960B44B0). 

## Planning for Dynamic Tag Management {#concept_EC50FC4409014AF1A1C3F1527015849F}

Dynamic Tag Management is an evolution of tag management, designed around the mapping of user interactions to marketing technologies. Your tags and marketing tools are best used when reacting to visitors (or segments of your visitors) and their activity on your site in precise ways. 

<!-- 

success.xml

 -->

By starting with user interactions as the stimulus for marketing tool response, you can know how those interactions result in data collection, testing, or engagement with tools like chat, surveys, and more.

### Planning ahead

To make the most of Dynamic Tag Management, establish a clear vision of how you want to use digital marketing. For help with planning, Adobe offers consulting on best practices. Also, a number of consulting agencies across the globe have extensive experience deploying Dynamic Tag Management and helping transform your organization's productivity, workflows, and sophistication. 

## Browser support {#concept_14C1D3046A1845AC8765584ECD28BD44}

DTM has been tested with the most commonly used browsers. 

<!-- 

browser-support.xml

 -->

The DTM user interface supports the latest version of Safari, Chrome, and Firefox, as well as version 9 and above of Internet Explorer.

The DTM library supports the latest version of Safari, Chrome, and Firefox, as well as version 8 and above of Internet Explorer. 

## Access DTM through Experience Cloud {#task_558CAA9062D646D5BC9252C4D574578F}

These instruction explain how to access DTM companies through the Experience Cloud. 

<!-- 

t_access-dtm-ec.xml

 -->

1. Open the solution picker and click **[!UICONTROL Activation]**.
1. Click **[!UICONTROL Dynamic Tag Management]**.

## Managing users and the publish workflow {#concept_D6E9196B4607429197D07B472A7F0BAC}

Dynamic Tag Management is based on a roles-oriented platform that lets you control the process. 

<!-- 

publish_workflow.xml

 -->

Roles include the following: 

|  Role  | Description  |
|---|---|
|  Users  | Create and test rules.  |
|  Approvers  | Review and approve rules, making approved states of rules publishable.  |
|  Publishers  | Publish rules to the production site. Only approved rules are published.  |
|  Administrators  | Create and manage users, as well as inheriting rights from the three preceding roles.  |

### Publishing workflow

1. A rule is saved. 
1. The rule is automatically pushed to your staging site where you can perform testing. 
1. The saved rule is funneled into the approval queue, where the details of the rule can be viewed in summary. 
1. The Approver, Approver & Publisher, or Administrator level user approves the rule. 
1. The rule goes into the publishing queue. 
1. In the publishing queue, the Admin, Publisher, or Approver & Publisher level user must publish the rule before it goes live.

   If you make changes to a published rule, the changes are not published to the site until they have been funneled through the approval process.

   This process ensures that only approved rules and rule revisions are published to your live site. This approval process also retains all past and present revision information. This retention makes it easy to follow a rule’s history and pin-points when an issue may have occurred.

For details, see [Users and Permissions](../administration/users.md#concept_2FA1011890C04E59845E8EB1E2345488). 

## Manage account settings {#task_BEC6AC7A5DB542CB9B442D318A0E0305}

Manage your user account settings, including settings for names, title, mobile number, time zone, language for the user interface, opt-out notifications, and password changes. 

<!-- 

t_manage_account_settings.xml

 -->

1. In the upper right corner of the Dynamic Tag Management interface, click the Profile icon > **[!UICONTROL Account Settings]**.
1. Edit the fields as necessary:

   **First Name:** Specify your first name.

   **Last Name:** Specify your last name.

   **Title:** Specify your title.

   **Mobile Number:** Specify your mobile telephone number.

   **Outside of US:** Select this option if you are outside of the United States. Ensure that you provide a country code in the [!UICONTROL Mobile Number] field if you choose this option.

   **Time Zone:** Specify your time zone.

   **Language:** Choose the desired language from the drop-down list. The user interface displays in the selected language.

   **Email Address:** Specify your email address. You can add multiple email addresses separated by commas.

   **Opt Out of All Notifications:** Opt out of all email notifications when one of your web properties is published. By opting out of email notifications, you will no longer receive publish request, property published, note, or approval email notifications. However, you will continue to receive other email notifications.

   **Current Password:** If you want to change your Dynamic Tag Management password, specify your current password in this field.

   **Password:** Specify your new password.

   To maintain the utmost security possible for your account, all passwords must meet the following criteria:

    * Must be at least seven characters in length 
    * Must contain at least one number and at least one letter 
    * Must contain at least one special character that is not a letter or number 
    * Must not be one of your last five passwords

   **Password Confirmation:** Specify your new password for confirmation. 

1. Click **[!UICONTROL Save Changes]**.

## Architecture {#concept_03FEF75036BD4CD7822CEF47FAE443A9}

Information about Dynamic Tag Management architecture. 

<!-- 

architecture.xml

 -->

Architecturally, Dynamic Tag Management comprises two main components:

* **Management Application**: Offers an easy-to-use, tab-structured configuration user interface. 
* **JavaScript libraries**: Produced by the Management Application and transported to hosting servers. Dynamic Tag Management includes two types of JavaScript libraries:

    * **Staging Library:** Every change you make in the Management Application is immediately updated to use on the staging server. 
    * **Production Library:** Only the final, approved version of a tool or rules makes it onto the production server.

  This model fits well into the approval workflow, in that development or staging code is never accidentally included in the production library. See [Publish Workflow](../getting-started/get-started.md#concept_300552C4F89E418F94A4D755960B44B0).

>[!VIDEO](https://video.tv.adobe.com/v/17166/)

By the end of this video you should be able to:

* Describe the basic elements of DTM's architecture
