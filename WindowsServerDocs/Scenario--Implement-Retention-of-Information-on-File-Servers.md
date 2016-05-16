---
title: Scenario: Implement Retention of Information on File Servers
ms.custom: 
  - AD
ms.prod: windows-server-threshold
ms.reviewer: na
ms.service: active-directory
ms.suite: na
ms.technology: 
  - active-directory-domain-services
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: ecdcc211-6983-4a8c-9f9d-84e45b5cb0b6
---
# Scenario: Implement Retention of Information on File Servers
A retention period is the amount of time that a document should be kept before it is expired. Depending on the organization, the retention period can be different. You can classify files in a folder as having a short, medium, or long\-term retention period, and then assign a timeframe for each period. You may want to keep a file indefinitely by putting it on legal hold.

## <a name="BKMK_OVER"></a>Scenario description
File Classification Infrastructure and File Server Resource Manager uses file management tasks and file classification to apply retention periods for a set of files. You can assign a retention period on a folder and then use a file management task to configure how long an assigned retention period is to last. When the files in the folder are about to expire, the owner of the file receives a notification email. You can also classify a file as being on legal hold so that the file management task will not expire the file.

You can find planning information for configuring retention in [Plan for Retention of Information on File Servers](assetId:///edf13190-7077-455a-ac01-f534064a9e0c).

You can find steps for classifying files for legal hold and configuring a retention period in [Deploy Implementing Retention of Information on File Servers &#40;Demonstration Steps&#41;](Deploy-Implementing-Retention-of-Information-on-File-Servers--Demonstration-Steps-.md).

> [!NOTE]
> That scenario only discusses how to manually classify a document for legal hold. However, it is possible in [!INCLUDE[win8_server_2](includes/win8_server_2_md.md)] to automatically classify documents for legal hold. One way to do this is to create a Windows PowerShell classifier that compares the file owner to a list of user accounts that are under legal hold. If the file owner is a part of the user account list, the file is classified for legal hold.

## In this scenario
This scenario is part of the Dynamic Access Control scenario. For additional information about Dynamic Access Control, see:

-   [Dynamic Access Control: Scenario Overview](Dynamic-Access-Control--Scenario-Overview.md)

## <a name="BKMK_NEW"></a>Features included in this scenario
The following table lists the features that are part of this scenario and describes how they support it.

|Feature|How it supports this scenario|
|-----------|---------------------------------|
|[File Server Resource Manager Overview_1](File-Server-Resource-Manager-Overview_1.md)|File Management Tasks is a feature that is included in File Server Resource Manager.|
|[File and Storage Services Overview](File-and-Storage-Services-Overview.md)|File Server Resource Manager is a feature that is included with the File Services server role.|

