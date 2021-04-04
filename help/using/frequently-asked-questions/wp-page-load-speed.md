---
description: Information about effective solutions to the issues affecting page load speed.
keywords: Dynamic Tag Management
seo-description: Information about effective solutions to the issues affecting page load speed.
seo-title: How do tag management systems improve page load speed?
solution: Experience Cloud
title: How do tag management systems improve page load speed?
uuid: d5e9fed0-e5cb-4fae-b55f-8f4c9527e936
exl-id: 20df39ce-d85e-4b6e-a804-ded8a25ba537
---
# How do tag management systems improve page load speed?{#how-do-tag-management-systems-improve-page-load-speed}

Information about effective solutions to the issues affecting page load speed.

 Adobe Dynamic Tag Management provides a number of effective solutions to the issues affecting page load speed. Dynamic Tag Management approaches the page differently from most other solutions, by providing conditional logic in its core library file that delivers file assets only when needed. In addition to a focus on scenario-based logic and precise activation of vendor technologies, Dynamic Tag Management provides a series of features that dramatically improve page speed. These include:

* Self-hosted static file delivery that eliminates the dependency on third-party hosting and DNS 
* Parallelization of tag loading through asynchronous delivery 
* Tag killing options with timeouts that can be modified by the client 
* Dramatically reduced file size through the optimized Dynamic Tag Management library schema - over 90% smaller than competitors 
* Enhanced file compression and delivery 
* Optimized timing and delivery sequencing that can be modified by the client 
* Client-side delivery of file assets that eliminates any additional server-side processing

Each tag management system (TMS) vendor must deal with the challenges of page load speed and Adobe Dynamic Tag Management provides the best set of options that can be assembled to meet these challenges. There are also a number of guiding questions that should be answered when evaluating page load speed and TMS options.

**Page load speed**

There are essentially six areas that affect page load speed:

1. Caching of site assets 
1. Creating site pages from the server 
1. Reducing the number of downloaded files 
1. Reducing the size of downloaded files 
1. Improving the connection speed to source files 
1. Converting sequential file loading to parallel file loading

The caching of site assets occurs at the browser level and is not something that TMS vendors can directly address. The same is true of the time that it takes for servers to create site pages and prepare them for delivery. Both of these areas can increase and decrease the time that it takes for a page to load. Because TMS vendors cannot directly address the first two page load issues, this overview focuses on the remaining four areas.

All major TMS options attempt to reduce the number of downloaded files and also optimize their size. The approach that each TMS takes to accomplish those tasks might vary somewhat, but in the end they each provide some improvement to the final file weight that is delivered to the page. When evaluating a TMS it is important to understand the architecture involved in the packaging and deployment of the individual files to the client web browser.

* Are the files assembled server-side on each request or delivered from pre-published static files? 
* If files are assembled dynamically, how long does file assembly take for each request? 
* Is there a server-side-only management of a portion of the files, and if so, what are the limitations of that architecture? 
* What compression techniques are used in the generation of the files? 
* Are optimizations provided in the TMS file generation that might help mitigate browser errors?

In the final analysis, each major TMS vendor reduces the number of downloaded files and optimizes the file size with some degree of success.

The areas where TMS solutions can see appreciable speed differences on the page are in the areas of connection speed and file loading. All of the major TMS offerings provide the option of a globally distributed CDN to deliver their files. Hosting files on any infrastructure is also available as an option when using Adobe Dynamic Tag Management. In most cases a CDN provides an efficient means to deliver the TMS files. However, there are several cautionary questions that must be answered relating to the hosting methodology that is provided by the TMS.

* What happens if the host CDN or regional DNS service fails?

  A number of enterprise-level failures have occurred in these areas during critical delivery times for some TMS vendors. Self-hosting of TMS assets prevents this situation from occurring because the files are delivered along with the rest of the client-hosted website assets either on their own architecture or an architecture of their choice. 
* What are the response times for file retrieval? 
* Are international response times significantly different for regional visitors? 
* How responsive are the vendors of the third-party code that the TMS manages like Facebook, Google, Foresee, etc.?

  Each of these third-party connections can cause delays even if the TMS files are delivered quickly. Does the TMS have client-adjustable tag timeouts that mitigate vendor delays?

File loading also has an effect on page speed, but more specifically, on the user experience. The use of asynchronous tag loading, conditional logic that determines what file assets will be delivered, and the placement of timeouts on tags provide ways to parallelize tag behavior and improve the loading of the page. Although the final tag weight may not be significantly different at the end of the page load, moving third-party vendor tags from a synchronous to asynchronous load allows multiple assets to load in parallel rather than one at a time. How much flexibility does the TMS provide regarding the timing and sequencing of vendor code? Does the TMS vendor provide best practices for optimizing page performance in relationship to file loading? Can third-party vendor code be easily changed from synchronous to asynchronous loading and vice-versa?

Adobe Dynamic Tag Management excels in each of these four page speed areas and, in certain cases like hosting, provides a better solution than other vendors. However, page load speed is only one area that needs to be addressed when evaluating a TMS. Critical questions need to be answered regarding workflow and governance, rule deployment methodologies, the user interface, implementation, migration, maintenance, and user segmentation capabilities. These are areas that make Adobe Dynamic Tag Management stand out as a system with a proven performance record that clients enjoy using over the long-term.
