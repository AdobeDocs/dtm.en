---
description: Information about the various hosting options in Dynamic Tag Management  Akamai, self-hosting FTP delivery, and self-hosting library download.
keywords: Dynamic Tag Management
seo-description: Information about the various hosting options in Dynamic Tag Management  Akamai, self-hosting FTP delivery, and self-hosting library download.
seo-title: Embed code and hosting options
solution: Experience Cloud
title: Embed code and hosting options
uuid: b05e4cc2-8b2f-42af-97c0-2f68436a7d6e
exl-id: bbcdc2b0-318b-44be-b898-c5320101f2b1
---
# Embed code and hosting options{#embed-code-and-hosting-options}

This article includes information about the various hosting options in Dynamic Tag Management: Akamai, self-hosting FTP delivery, and self-hosting library download.

>[!IMPORTANT]
>
>For a successful implementation, it is critical that you follow these instructions as they appear in Adobe Help. Specifically, you must place the header code in the `<head>` section of your document templates. Also, you must place the footer code just before the closing `</body>` tag. Placing either of these embed codes elsewhere in your markup, or using asynchronous methods to append the embed codes, are *not* a supported implementation of Dynamic Tag Management. 
>
>An unsupported implementation will yield unexpected results and prevent Customer Care and Engineering from assisting with your implementation. 
>
>Including multiple embed codes on a single page is not supported, as it can cause conflicts.

## Hosting workflow {#section_A82AE50045D644F89069AB4523307964}

The following illustration shows the hosting workflow in Dynamic Tag Management:

![](assets/hosting_workflow.png)

## Hosting options {#section_A6D88EAD84D5473187AD786319927E63}

You can deploy Dynamic Tag Management using one or more of the following options, found on the [!UICONTROL Embed] tab:

### Akamai (migrated from Amazon S3)

* The simplest hosting option to implement. 
* Globally distributed delivery network. 
* Adds additional third-party infrastructure dependencies (DNS lookup, Akamai availability). 
* See [Akamai](../client-side-information/deployment.md#concept_722B01555D0441ACBB052BC34DC5B67D) for information about migrating from Amazon S3 to Akamai.

1. Dynamic Tag Management generates custom JavaScript libraries. 
1. Dynamic Tag Management exports the custom JavaScript libraries to Akamai. 
1. The target website references the Akamai-hosted Dynamic Tag Management libraries directly at the page level.

### Amazon S3

>[!NOTE]
>
>After July 31, 2015 Adobe will no longer support Amazon S3. Your Dynamic Tag Management libraries on Amazon S3 will continue to be served until December 31, 2015, but in a read-only state. Any changes made in Dynamic Tag Management will no longer be reflected in these files.
>
>To deploy additional changes to your site after July 31, 2015, you must select one of our other hosting options. Self-hosting (FTP Delivery or Library Download) is always the suggested best practice, but our 3rd-party Akamai hosting is a world-class option as well.

### Self-hosting: FTP delivery

Dynamic Tag Management uses a *`push`* approach to export custom JavaScript libraries directly to the web content server host via the FTP protocol.

This solution requires an FTP server and credentials to be available on the web content server to publish changes to the custom Dynamic Tag Management libraries.

For more detailed information, see [FTP](../client-side-information/deployment.md#task_A7B37CB2C89941A4A4D1F9AF06FC493D).

1. Dynamic Tag Management generates custom JavaScript libraries. 
1. Dynamic Tag Management exports the custom JavaScript libraries to host server via FTP. 
1. The target website locally references the custom Dynamic Tag Management libraries.

### Self-hosting: Library download

The application uses a *`pull`* approach to export custom JavaScript libraries to Amazon S3. There, the libraries can be accessed by a hosted server-side process.

Additionally, the libraries are available via web download directly from the Dynamic Tag Management interface.

This solution requires either a manual retrieval and publication of the Dynamic Tag Management libraries or the creation of an automated process that pulls the libraries from Akamai onto the web content server.

This approach takes the most time to set up, but is also the most secure and flexible option.

For more detailed information, see [Library Download](../client-side-information/deployment.md#task_B7A42F3B1D3E4B71B0BADD17C181F22A).

1. Dynamic Tag Management generates custom JavaScript libraries. 
1. Dynamic Tag Management exports the custom JavaScript libraries to Akamai. 
1. Custom Dynamic Tag Management libraries are manually or programmatically moved to the web content server. 
1. The target website locally references the custom Dynamic Tag Management libraries.

You can expect improved performance and more control over security by hosting the FTP Delivery and the Library Download options on your CDN or infrastructure.

>[!VIDEO](https://video.tv.adobe.com/v/17175/)

By then end of this video you should be able to:

* Explain the different hosting options

## Hosting considerations (FAQ) {#concept_B38C7659E3EC4324A42A199C761EF1F4}

Consider these questions when deciding on a hosting option. 

<!-- 

hosting.xml

 -->

You might consider the following questions when deciding which hosting option is best for your organization:

* How do I choose a hosting option?

  Dynamic Tag Management creates and uses various JavaScript files that contain all the code needed to run the system. These library files can be hosted by Adobe, or they can be hosted on your own servers within your own Web architecture.

  The Library Download hosting option also allows you to self-host the library files. When an authorized Dynamic Tag Management user makes a change in the software, our system writes those changes out to the library files. When you host the library files on your servers with this option, our system needs a way to get those changes to your servers. With the Library Download hosting option, our system sends a ping (an http post) to your system to let your servers know there’s been an update to the library files. Your IT team can create a cron job, or other scripted process, so your servers can pick up the changed files. In this way, whenever a change is made in Dynamic Tag Management, the files you’re hosting on your servers can be updated in an automated manner.

  You can use one or more of these hosting options for a web property, just don’t use more than one embed code in any single page. For example, you could use Akamai in your staging environments and one of the self-hosted options in your production environments. Or, you could use the Akamai option for any sites, domains, or subdomains hosted by one of your agency partners. These options give you more flexibility to host the library files according to your specific needs. 

* What is your current policy regarding website content sources?

  The answer to this question helps determine whether the JavaScript library can be hosted on Akamai, pushed to the website file structure via FTP, or manually pulled into the file structure by a server-side process.

* Can I use more than one Dynamic Tag Management library hosting option at once?

  Yes, you can turn on and use any number of the hosting options and use different embed codes for different domains or subdomains.

  For example, you might want to use the Akamai option for your lower-level, non-production environments such as staging, dev, test, or UAT. At the same time, you might use one of the self-hosted options, such as Library Download, for your production environments.

  Remember that you cannot use more than one option on the same page. You should not implement more than one Header Embed code on any page. 

* What is your current website content deployment process?

  The deployment process affects how quickly changes can be deployed to the site from the Dynamic Tag Management administrative interface. It also affects how long it takes to initially install Dynamic Tag Management on the website. 
* What is the current page-level markup and structure of the website?

  An understanding of the basic page-level markup and structural decisions on the website helps with the proper installation of Dynamic Tag Management and the construction of rules within the administrative interface.

  Key items to identify include:

    * Which JavaScript libraries are referenced within the `<head>` section of the web page. 
    * Whether the individual sections of the page, such as headers and footers, are dynamically generated.

  Knowledge of any content management systems that are used is helpful in determining the appropriate hosting methodology.

## Akamai {#concept_722B01555D0441ACBB052BC34DC5B67D}

Akamai is the primary external hosting option. Akamai provides you with a reliable hosting experience and is the simplest option to implement. Akamai provides the greatest third-party infrastructure dependencies, such as DNS lookup, faster load times, and faster round-trip delivery times. 

<!-- 

akamai.xml

 -->

The Akamai hosting option allows you to store your web property library files on Adobe’s Edge CDN, which sits on the Akamai architecture. This option allows you to install the Embed codes in your page templates and quickly get up and running with Dynamic Tag Management without involving your internal IT teams and servers.

>[!NOTE]
>
>After July 31, 2015 Adobe will no longer support Amazon S3. Your Dynamic Tag Management libraries on Amazon S3 will continue to be served until December 31, 2015, but in a read-only state. Any changes made in Dynamic Tag Management will no longer be reflected in these files. 
>
>To deploy additional changes to your site after July 31, 2015, you must select one of our other hosting options. Self-hosting (FTP Delivery or Library Download) is always the suggested best practice, but our 3rd-party Akamai hosting is a world-class option as well.

## Akamai cache control headers {#section_E004368DEA0143B4B17B2D5966A4664E}

Cache control headers are automatically set for libraries hosted on Akamai (`assets.adobedtm.com`).

* Production builds: Cache control headers are set to 60 minutes 
* Staging builds with `-staging` in the filename: Cache control headers are set to 0 minutes

>[!NOTE]
>
>It is up to browsers to receive and respect the cache control headers. Some browsers might ignore them.

## Why choose Akamai hosting? {#section_36B2C1C4EBB946898E430F52F8991F3C}

When you choose the Akamai option in the Embed section of Dynamic Tag Management, it means that your Dynamic Tag Management library files are served to your visitors from Adobe’s Edge CDN, which runs on Akamai architecture.

Akamai is robust when serving content to a global, high-volume audience of Web visitors. Akamai runs redundant networks of load-balanced, geo-optimized nodes to serve content as quickly as possible to visitors wherever they are located throughout the world.

Specifically, Akamai runs more than 137,000 servers in 87 countries within more than 1,150 networks. In terms of redundancy, Akamai does not just route from one server to another, Akamai routes from one node of servers to another node of servers as-needed. In other words, each node consists of multiple servers for redundancy within a node, so a box going down is not an issue because he other boxes in the node take over. If a node goes down, Akamai serves from the next closest one, with the same cached content. Nodes are dynamically selected based on visitor location, traffic load, and other factors so content is consistently served from the best local node for each visitor.

## Can I avoid errors if Akamai is unavailable? {#section_40E66A23608441A09BD433FC18B00E68}

No. Dynamic Tag Management can do nothing from the client side if the library is unavailable. However, it is extremely unlikely that Akamai would be unavailable. 

## Migrate from Amazon S3 to Akamai {#task_20543879440C4154B01F517FABE636C2}

Migrate from Amazon S3 hosting to Akamai by replacing Amazon S3 code. 

<!-- 

t_akamai_migrate.xml

 -->

>[!NOTE]
>
>Since July 31, 2015 Adobe no longer supports Amazon S3. Your Dynamic Tag Management libraries on Amazon S3 will continue to be served until December 31, 2015, but in a read-only state. Any changes made in Dynamic Tag Management will no longer be reflected in these files. 
>
>To deploy additional changes to your site after July 31, 2015, you must select one of our other hosting options. Self-hosting (FTP Delivery or Library Download) is always the suggested best practice, but our 3rd party Akamai hosting is a world class option as well.

1. Navigate to the [!UICONTROL Embed] tab.
1. Replace your existing Amazon S3 header codes with the new Akamai header codes.

   No change is necessary in the footer code. 

1. Click **[!UICONTROL Akamai]** to the **[!UICONTROL On]** position.

   ![Step Result](assets/akamai.png)

1. Click the **[!UICONTROL Amazon S3]** option to the **[!UICONTROL Off]** position.

   >[!NOTE]
   >
   >After you disable Amazon S3, you can no longer use Amazon S3 hosting. Ensure that you no longer need Amazon S3 before turning it off.

   Akamai hosting in Dynamic Tag Management functions independently of any Akamai hosting you currently use for your website. 

## FTP {#task_A7B37CB2C89941A4A4D1F9AF06FC493D}

This section provides steps to deploy Dynamic Tag Management using FTP (the *`push`* methodology). 

<!-- 

deployment_ftp.xml

 -->

The FTP Delivery hosting option lets you self-host the library files. When an authorized Dynamic Tag Management user makes a change in the software, Dynamic Tag Management writes those changes to the library files. When you host the library files on your servers with this option, Dynamic Tag Management must get those changes to your servers. With the FTP Delivery hosting option, Dynamic Tag Management connects to your system, using credentials and server locations you enter into the system, and delivers any changed files. In this way, whenever a change is made in Dynamic Tag Management, the files you are hosting on your servers can be updated automatically.

You must be an administrator to be able to deploy via FTP. 

1. In the web property, click the **[!UICONTROL Embed]** tab.
1. Click **[!UICONTROL FTP Delivery]**. ![](assets/deploy_ftp_1.png){width="672"}
1. Provide the required FTP information for the staging and production servers, then click **[!UICONTROL Save FTP Information]**.

   >[!NOTE]
   >
   >Click **[!UICONTROL Enable Relative Hostnames for Staging and Production Library Hosting]**, if desired. Enabling relative hostname prepends the provided library paths with "window.location.hostname". This allows DTM to load hosted scripts from relative paths, giving you the ability to host your library without editing your path for each deploy.

1. Toggle the switch in the top right corner to **[!UICONTROL ON]**.
1. Click **[!UICONTROL Header Code]** and **[!UICONTROL Footer Code]** to expand those sections.
1. Click the appropriate **[!UICONTROL Copy Embed Code]** button to copy header and footer codes for your staging or development environments.

   >[!NOTE]
   >
   >The staging code should go only into your staging or development environment. Production code should be placed on the live production site.

1. Copy the header code and place it within the HEAD section of the site HTML, on every page of the website. Place it as close to the beginning `<head>` tag as possible.
1. Copy the footer code and place it within the BODY section of the site HTML, on every page of the website. Place it as close to the closing `</body>` tag as possible

## Library download {#task_B7A42F3B1D3E4B71B0BADD17C181F22A}

This section provides steps to deploy Dynamic Tag Management using Library Download (the `pull` methodology). 

<!-- 

deployment_download.xml

 -->

The Library Download hosting option also lets you self-host the library files. When an authorized Dynamic Tag Management user makes a change in the software, Dynamic Tag Management writes those changes to the library files. When you host the library files on your servers with this option, Dynamic Tag Management must get those changes to your servers. With the Library Download hosting option, Dynamic Tag Management sends a ping (an HTTP post) to your system to let your servers know there has been an update to the library files. Your IT team can create a cron job, or other scripted process, so your servers can pick up the changed files. In this way, whenever a change is made in Dynamic Tag Management, the files you are hosting on your servers can be updated automatically.

You must be an administrator to deploy using the Library Download. 

1. In the web property, click the **[!UICONTROL Embed]** tab.
1. Click **[!UICONTROL Library Download]** in the left navigation. ![](assets/deploy_libdown_1.png){width="672"}

1. Fill out one or both of the following optional fields:

   | Option| Description|
   |--- |--- |
   |Shared Secret|Encrypts the Dynamic Tag Management library during download. If you enter a shared secret, AES-256 is used to encrypt your .zip file using this passphrase.|
   |Deploy Hook URL|The process of deploying Dynamic Tag Management files to the server can be automated whenever there is an update. Create a script that is accessible via the specified public URL. If you enter a deploy hook URL, an HTTP POST is made to it every time your bundle is successfully updated. The body of the post includes a payload containing the download URL of the bundle.|
 
1. Complete the fields under [!UICONTROL Domain and Paths to Tracking File], for staging and production.

   Specify the location where the files reside when deployed to your server. Do not include the protocol or any leading or trailing slashes. Dynamic Tag Management requires a domain and a path for HTTP or HTTPS for the production and staging environments.

   >[!NOTE]
   >
   >Click **[!UICONTROL Enable Relative Hostnames for Staging and Production Library Hosting]**, if desired. Enabling relative hostname prepends the provided library paths with `window.location.hostname`. This allows DTM to load hosted scripts from relative paths, giving you the ability to host your library without editing your path for each deploy.

1. Download the files from the specified URL for the respective environment (staging or production), and deploy them to the location specified in the settings.
1. Click the **[!UICONTROL Header Code]** and **[!UICONTROL Footer Code]** sections.
1. Click the appropriate **[!UICONTROL Copy Embed Code]** button to copy header and footer codes for your staging or development environments.

   >[!NOTE]
   >
   >The staging code should go only into your staging or development environment. Production code should be placed on the live production site.

1. Copy the header code and place it within the HEAD section of the site HTML, on every page of the website. Place it as close to the beginning `<head>` tag as possible.
1. Copy the footer code and place it within the BODY section of the site HTML, on every page of the website. Place it as close to the closing `</body>` tag as possible
