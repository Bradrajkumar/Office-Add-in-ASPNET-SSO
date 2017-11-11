# Office Add-in that that supports Single Sign-on to Office, the Add-in, and Microsoft Graph

The `getAccessTokenAsync` API in Office.js enables users who are signed into Office to get access to an AAD-protected add-in and to Microsoft Graph without needing to sign-in again. This sample is built on ASP.NET and Microsoft Identity Library (MSAL). 

 > Note: The `getAccessTokenAsync` API is in preview.

## Table of Contents
* [Change History](#change-history)
* [Prerequisites](#prerequisites)
* [To use the project](#to-use-the-project)
* [Questions and comments](#questions-and-comments)
* [Additional resources](#additional-resources)

## Change History

* May 10, 2017: Initial version.
* September 15, 2017: Added support for 2FA.

## Prerequisites

* An Office 365 account.
* Office 2016, Version 1710, build 16.0.8605.1000 Click-to-Run, or later. You many need to be an Office Insider to obtain this version. For more information, see [Be an Office Insider](https://products.office.com/en-us/office-insider?tab=tab-1) .
* Visual Studio 2017, version 15.4.0 Preview 1 or later


## To use the project

This sample is meant to accompany the walkthrough at: [Create an ASP.NET Office Add-in that uses Single Sign-on (preview)](https://dev.office.com/docs/add-ins/develop/create-sso-office-add-ins-aspnet)

There are two versions of the sample, in the folders Before and Completed.

To use the Before version and manually add the crucial SSO-oriented code, follow all the procedures in the article linked to above.

To work with the Completed version, follow all the procedures, except the sections "Code the client-side" and "Code the server-side" in the article linked to above.

## Questions and comments

We'd love to get your feedback about this sample. You can send your feedback to us in the *Issues* section of this repository.

Questions about Microsoft Office 365 development in general should be posted to [Stack Overflow](http://stackoverflow.com/questions/tagged/office-js+API). If your question is about the Office JavaScript APIs, make sure that your questions are tagged with [office-js] and [API].

## Additional resources

* [Office add-in documentation](https://msdn.microsoft.com/en-us/library/office/jj220060.aspx)
* [Office Dev Center](http://dev.office.com/)
* More Office Add-in samples at [OfficeDev on Github](https://github.com/officedev)

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Copyright
Copyright (c) 2017 Microsoft Corporation. All rights reserved.

