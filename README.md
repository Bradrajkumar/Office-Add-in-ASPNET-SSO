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
* December 8, 2017: Added extensive error handling.
* January 7, 2019: Added information about web application security practices.

## Prerequisites

* An Office 365 account.
* Office 2016, Version 1710, build 16.0.8605.1000 Click-to-Run, or later. You many need to be an Office Insider to obtain this version. For more information, see [Be an Office Insider](https://products.office.com/en-us/office-insider?tab=tab-1) .
* Visual Studio 2017, version 15.4.0 Preview 1 or later

## Deviations from Best Practices

The samples in this repo are narrowly focused on demonstrating the use of the SSO APIs. To keep it simple, some best practices are not followed, including best practices in web application security. <span style="color:red">You should not use any of these samples as the starting point of a production add-in unless you are prepared to make substantial changes.</span> We recommend that you begin a production add-in by using one of the Office Add-in projects in Visual Studio, or by generating a new project with the [Yeoman Generator for Office Add-ins](https://github.com/OfficeDev/generator-office).

_Some_ of the points to keep in mind about these samples:

* The data that the samples render on the home page &mdash; file and folder names from OneDrive &mdash; is not encoded against Cross-site Scripting (XSS) attacks. In the context of this sample, encoding is not needed because there are restrictions on what characters can be used in OneDrive file and folder names. These restrictions do not necessarily apply to other kinds of Microsoft Graph data. In general, a production add-in should protect against the possibility that data from a data source contains an XSS string by encoding or sanitizing the data before it is inserted into an HTML page.
* The samples send a hardcoded query parameter on the URL for the Microsoft Graph REST API. If you modify this code in a production add-in and any part of query parameter comes from user input, be sure that it is sanitized so that it cannot be used in a Response header injection attack.

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

