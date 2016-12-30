---
layout: post
title: How to migreate SSRS reports from one server to another?
---

>Watch my [Youtobe video](https://youtu.be/1knwXRIbVNw) to get details!


Let's say you want to migrate SSRS reports​ from an old reporting service server (e.g., SQL Server 2008 R2) to a new one (e.g., SQL Server 2016). What involves?

**There are three steps:​**

#### Step 1: Find the reports that don't need to be migrated

* You need to install SSW SQL Reporting Service Auditor both on the old and new servers. (You'll also need to run it on 3rd step)
* Find those reports are not-in-use, as per a rule: Do you know which reports are being used?
* Find creators of those reports, by clicking “Detail Views” in reports folder
![enter image description here](https://rules.ssw.com.au/SiteAssets/do-you-know-how-to-migrate-reporting-service-reports/detailsview.png)
**Figure: Find reports creators by clicking "Details View" inside report folder**

* Send an email to ask permission
![enter image description here](https://rules.ssw.com.au/SiteAssets/do-you-know-how-to-migrate-reporting-service-reports/sent.png)
 **Figure:  Send an email to ask permission**
 
  ![enter image description here](https://rules.ssw.com.au/SiteAssets/do-you-know-how-to-migrate-reporting-service-reports/receive.png)
  **Figure: Get an Email to act**

#### Step 2. Migrate those in-use reports from old server to new server​
>Tip: use the [ReportSync](https://github.com/dapaxx/reportsync) tool to save time.

#### Step 3. Check audit results

 * Run SSW SQL Reporting Service Auditor on both sides
 * Compare audit results. Note that even error and warning messages also
   need to be the same

If audit results are exactly the same on old and new servers, it indicates that migration is successful.​

> [SSW](https://www.ssw.com.au) is a leading Australia based software development company. SSW creates [rules](https://rules.ssw.com.au) and share them with developers around the world. I wrote this rule under the instruction of [Adam Cogen](https://sharepoint.ssw.com.au/AboutUs/Employees/Pages/Adam.aspx), who is the founder of SSW.