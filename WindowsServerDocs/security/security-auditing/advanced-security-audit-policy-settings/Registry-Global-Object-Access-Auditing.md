---
title: Registry (Global Object Access Auditing)
description: "Windows Server Security"
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: security-auditing
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: b02371ae-0be5-4fbc-82f3-5d8f4443bf99
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Registry (Global Object Access Auditing)

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

This topic for the IT professional describes the Advanced Security Audit policy setting, **Registry (Global Object Access Auditing)**, which enables you to configure a global system access control list (SACL) on the registry of a computer.

If you select the **Configure security** check box on this policy???s property page, you can add a user or group to the global SACL. This enables you to define computer system access control lists (SACLs) per object type for the registry. The specified SACL is then automatically applied to every registry object type.

This policy setting must be used in combination with the **Registry** security policy setting under Object Access. For more information, see [Audit Registry](Audit-Registry.md).

This policy setting is available on computers running the supported versions of the Windows operating system as designated in the **Applies to** list at the beginning of this topic.

## Related resource
[Advanced Security Audit Policy Settings](../Advanced-Security-Audit-Policy-Settings.md)

