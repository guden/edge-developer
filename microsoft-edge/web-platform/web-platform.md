---
title: Web platform overview
description: Testing for coming changes that could impact compatibility of your site with Microsoft Edge.  Moving users from Internet Explorer.  Setting up tracking prevention.  Detecting Microsoft Edge from your website. Detecting Windows 11 via User-Agent Client Hints.
author: MSEdgeTeam
ms.author: msedgedevrel
ms.topic: conceptual
ms.prod: microsoft-edge
ms.technology: devtools
ms.date: 02/14/2022
---
# Web platform overview

The following are considerations for developing websites and products for the web platform, specifically for Microsoft Edge:

*  Testing for coming changes that could impact compatibility of your website with Microsoft Edge.
*  Moving users to Microsoft Edge from Internet Explorer.
*  Configuring tracking prevention in Microsoft Edge.
*  Detecting Microsoft Edge from your website.
*  Customizing the Password Reveal button.
*  Detecting Windows 11 by using User-Agent Client Hints.

These aspects of developing for the web platform are described below.


<!-- ====================================================================== -->
## Site compatibility-impacting changes coming to Microsoft Edge

This article lists differences between the schedule of changes for Microsoft Edge versus the Chromium project, and high-impact changes which the Microsoft Edge team is tracking especially closely.

The web platform is a collection of technologies used for building webpages, including HTML, CSS, JavaScript, and many other open standards.  The web platform constantly evolves to improve the user experience, security, and privacy.  In some cases, changes may affect the functionality of existing webpages.

[Site compatibility-impacting changes coming to Microsoft Edge](site-impacting-changes.md)


<!-- ====================================================================== -->
## Move users to Microsoft Edge from Internet Explorer

Many modern websites have designs that are incompatible with Internet Explorer.  When an Internet Explorer user visits an incompatible public website, the user may be instructed by the website that the website is incompatible with Internet Explorer, and that the user must switch to a more modern browser in order to use the website.

To minimize disruptions, Microsoft Edge supports a new capability that automatically redirects users.  When an Internet Explorer user goes to a website that's incompatible with Internet Explorer, Windows can automatically redirect the user to Microsoft Edge.  Only websites that are part of the Need Microsoft Edge list are redirected.

[Move users to Microsoft Edge from Internet Explorer](ie-to-microsoft-edge-redirection.md)


<!-- ====================================================================== -->
## Tracking prevention in Microsoft Edge

The tracking prevention feature in Microsoft Edge protects users from online tracking by restricting the ability of trackers to access browser-based storage as well as the network.

The tracking prevention feature is built to uphold the Microsoft Edge _browser privacy promise_, while also ensuring that there is no impact by default to website compatibility or the economic viability of the web.

[Tracking prevention in Microsoft Edge](tracking-prevention.md)


<!-- ====================================================================== -->
## Detect Microsoft Edge from your website

Microsoft Edge enables your website to retrieve user agent information.  You use the user agent information to present webpages correctly for each user's browser.  Browsers provide mechanisms for websites to detect browser information such as brand, version number, and host operating system.

*  **User-Agent Client Hints** are an improved mechanism for retrieving browser information.

*  **User-Agent strings** are legacy; they are outdated and have a history of causing website compatibility problems.

You may want to provide different experiences to users based on their browser.  For example, if you include steps about how to configure Microsoft Edge or another browser for use with your site, you may want to detect the browser and then show the appropriate content.

[Detect Microsoft Edge from your website](user-agent-guidance.md)


<!-- ====================================================================== -->
## Detect Windows 11 using User-Agent Client Hints

Websites can differentiate between users on Windows 11 and Windows 10 by using User-Agent Client Hints (UA-CH).  The User-Agent Client Hints format is used by browsers to provide user agent information to websites.

Websites can use the user agent information that's sent from the browser to detect information such as:
*  The browser brand.
*  The browser version number.
*  The device platform on which the browser is running.

There are two approaches for sites to access user agent information:

*  User-Agent strings (legacy).
*  User-Agent Client Hints (recommended).

[Detect Windows 11 using User-Agent Client Hints](how-to-detect-win11.md)


<!-- ====================================================================== -->
## Customize the password reveal button

The `password` input control in Microsoft Edge includes a **password reveal** button.  To make sure that the password is entered correctly, a user can click the **password reveal** button or press `Alt`+`F8`, to show the characters in the password field.  You can remove the password reveal control, or customize the control styling.

[Customize the password reveal button](password-reveal.md)