---
# required metadata

title: Working with the ATA Console | Microsoft Advanced Threat Analytics
description: Describes how to log into the ATA console and the components of the console
keywords:
author: rkarlin
manager: stevenpo
ms.date: 04/28/2016
ms.topic: article
ms.prod: identity-ata
ms.service: advanced-threat-analytics
ms.technology: security
ms.assetid: 1bf264d9-9697-44b5-9533-e1c498da4f07

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: bennyl
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Working with the ATA Console

Use the ATA console to monitor and respond to suspicious activity detected by ATA.

## Enabling access to the ATA Console
Any user who is a member of the local Administrators group on the ATA Center server has permission to log in to the ATA Console and manage ATA settings.
To allow a user to log in to the ATA Console without making them a local administrator, add them to the local group: **Microsoft Advanced Threat Analytics Administrators**.

## Logging into the ATA Console

1. In the ATA Center server, click the **Microsoft ATA Console** icon on the desktop or open a browser and browse to the ATA Console.

    ![ATA server icon](media/ata-server-icon.png)

    > [!NOTE]
    > You can also open a browser from either the ATA Center or the ATA Gateway and browse to the IP address you configured in the ATA Center installation for the ATA Console.    

2.  Enter your username and password and click **Log in**.

![ATA login screen image](media/ATA-log-in-screen.jpg)

    > [!NOTE]
    > You have to log in with a user who is a member of the local administrator group OR of the Microsoft Advanced Threat Analytics Administrators group.

## The ATA Console

The ATA Console provides you a quick view of all suspicious activities in chronological order. It enables you to drill into details of any activity and perform actions based on those activities. The console also displays alerts and notifications to highlight problems with the ATA network or new activities that are deemed suspicious.

These are the key elements of the ATA console.


### Attack time line

This is the default landing page you are taken to when you log in to the ATA Console. By default, all open suspicious activities are shown on the attack time line. You can filter the attack time line to show All, Open, Dismissed or Resolved suspicious activities. You can also see the severity assigned to each activity.

![ATA attack timeline image](media/attack-timeline.png)

For more information, see [Working with suspicious activities](/advanced-threat-analytics/deploy-use/working-with-suspicious-activities).

### Notification bar

When a new suspicious activity is detected, the notification bar will open automatically on the right hand side. If there are new suspicious activities since the last time you logged in, the notification bar will open after you have successfully logged in. You can click the arrow on the right at any time to access the notification bar.

![ATA notification bar image](media/notification-bar.png)

### Filtering panel

You can filter which suspicious activities are displayed in the attack time line or displayed in the entity profile suspicious activities tab based on Status and Severity.

### Search bar

In the top menu, you will find a search bar. You can search for a specific user, computer or groups in ATA. To give it a try, just start typing.

![ATA console search image](media/ATA-console-search.png)

### Health Center

The Health Center provides you with alerts when something isn't working properly in your ATA deployment.

![ATA health center image](media/health-center.png)

Any time your system encounters a problem, such as a connectivity error or a disconnected ATA Gateway, the Health Center icon will let you know by displaying a red dot. ![ATA health center red dot image](media/ATA-Health-Center-Alert-red-dot.png)

Health Center alerts can be dismissed or resolved and are categorized High, Medium or Low depending on their severity. If you resolve an alert that the ATA service detects as still active, it will automatically be moved to the Open list of alerts. If the system detects that there is no longer cause for an alert (the situation has been fixed), it will automatically be moved to the resolved list.

### User and computer profiles

ATA builds a profile for each user and computer in the network. In the user profile ATA displays general information, such as group membership, recent logins, and recently accessed resources.

![User profile](media/user-profile.png)

In the computer profile, ATA displays general information, such as recently logins and recently accessed resources.

![Computer profile](media/computer-profile.png)

ATA provides additional information about entities (computers, devices, users) on the following pages: Summary, Activities, and Suspicious activities.

A profile that ATA has not been able to fully resolve will be identified with half-filled circle icon next to it.


![ATA unresolved profile image](media/ATA-Unresolved-Profile.jpg)

### Mini profile

Anywhere in the console where there is a single entity presented, such as a user or computer, if you hover your mouse over the entity, a mini profile will automatically open displaying the following information if available:

![ATA mini profile image](media/ATA-mini-profile.jpg)

-   Name

-   Picture

-   Email

-   Telephone

-   Number of suspicious activities by severity



## See Also
[Check out the ATA forum!](https://social.technet.microsoft.com/Forums/security/en-US/home?forum=mata)
