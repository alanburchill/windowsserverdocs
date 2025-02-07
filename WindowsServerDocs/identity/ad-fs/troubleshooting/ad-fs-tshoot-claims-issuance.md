---
title: AD FS Troubleshooting - Claims Issuance
description:  This document describes how to troubleshoot token issuance issues with AD FS
author: billmath
ms.author: billmath
manager: amycolannino
ms.date: 08/15/2023
ms.topic: article
ms.custom: ihenkel
---

# AD FS Troubleshooting - Claims Issuance
A claim is a statement that one subject makes about itself or another subject.  Claims are issued by a relying party, and they're given one or more values and then packaged in security tokens that are issued by the AD FS server.  Because there are several moving parts in this process, claims issuance can be broken down into these key parts.

>[!NOTE]
>You can use [ClaimsXRay](https://adfshelp.microsoft.com/ClaimsXray/TokenRequest) on the [AD FS Help](https://adfshelp.microsoft.com) site to assist in troubleshooting claims issues.

## Token Request
When you go to a relying party, it will redirect you to AD FS with a token request.  Issues can arise with the request.  Most notably:

### The request formatting with 3rd parties (particularly SAML)

### Preformatted URLs that have typos
When issuing a token from WS-Federaion relying parties that token request comes across with URL query string parameters.  If the relying party doesn't specify the correct parameters in that URL when it does the redirect to AD FS, then it could cause an issue with the request.


In order to verify the token format, a web debugger tool can be used


## Token Response

## Authentication

## Claim Rule Processing
