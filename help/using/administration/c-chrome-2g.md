---
description: Chrome might block document.write calls for visitors on 2G networks.
seo-description: Chrome might block document.write calls for visitors on 2G networks.
seo-title: Chrome warning on 2G networks
title: Chrome warning on 2G networks
uuid: 51ce547c-1528-4626-8e6d-feddc8cbfb61
exl-id: 6ed26280-527f-4741-a8c7-4270c5f0078b
---
# Chrome warning on 2G networks{#chrome-warning-on-g-networks}

Chrome might block document.write calls for visitors on 2G networks.

 When using the most recent Chrome update for sites with DTM deployed, a warning might appear in the JavaScript console, which says that Chrome might block `document.write` calls in the browser if the device has poor network connectivity. Chrome specifically states they are currently targeting users on 2G networks. See "[Intervening against document.write()](https://developers.google.com/web/updates/2016/08/removing-document-write?hl=en)" on the Google Developers website.

Due to the limited usage of 2G network, the current 2G Google intervention should have a minimal impact on enterprise customers at this time. Adobe is proactively addressing future issues that might develop if Google continues to promote practices that contradict Internet community standards.

DTM's goal has always been to create and support the most powerful and flexible features in the space. This includes allowing DTM users to leverage both synchronous and asynchronous technologies.

If you are concerned about 2G Chrome users, you can use a more asynchronous deployment of DTM and continue to use the robust set of asynchronous specific features of DTM.

If you see this warning and want to deploy an asynchronous DTM setup that removes all `document.write` calls (and prevents the warning), refer to the following sections.

## Target {#section_ACCD81F813434282B64A56F813828483}

If you are using Target via DTM, and are concerned about visitors on a 2G cellular network who are using Chrome, please do the following:

1. Update your Target code from mbox.js to at.js in the DTM target tool.

   Make sure you use the custom code editor.

   To learn more about implementing Target with at.js, see [at.js Implementation](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/mbox-download.html) in the Target help. 

1. Uncheck the **[!UICONTROL Load Adobe Target Library synchronously]** checkbox in the DTM Target tool. 
1. Test well before deploying.

   >[!NOTE]
   >
   >Loading the Target library asynchronously prevents the warning, but might cause "flickering" on the page if default content loads before the targeted content.

## Third-party tags {#section_F9FE8A1120EE4932AD679AF8E4498930}

If you are deploying 3rd-party tags via rules in DTM, and are concerned about visitors on a 2G cellular network who are using Chrome, please do the following:

1. Review all 3rd-party scripts that are deployed via `Sequential JavaScript` or `Sequential HTML` for `top of page` or `bottom of page` positioning rules. 
1. In the code editor, change the Type to `Non-Sequential JavaScript` or `Non-Sequential HTML`.

   >[!NOTE]
   >
   >Any functionality that requires synchronicity will no longer work.

1. Review the code within the editor to ensure it isn't using `document.write`.

   Any code deployed through DTM that uses `document.write` might be affected. 

1. Test well before deploying.
