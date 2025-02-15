---
author: davidiseminger
ms.service: powerbi
ms.topic: include
ms.date: 11/10/2023
ms.author: davidi
---

## Considerations and limitations

You can see the current limitations for row-level security on cloud models here:

* If you previously defined roles and rules in the Power BI service, you must re-create them in Power BI Desktop.
* You can define RLS only on the semantic models created with Power BI Desktop. If you want to enable RLS for semantic models created with Excel, you must convert your files into Power BI Desktop (PBIX) files first. [Learn more](../connect-data/desktop-import-excel-workbooks.md).
* Service principals can't be added to an RLS role. Accordingly, RLS won’t be applied for apps using a service principal as the final effective identity.
* Only Import and DirectQuery connections are supported. Live connections to Analysis Services are handled in the on-premises model.
* The Test as role/View as role feature doesn't work for DirectQuery models with single sign-on (SSO) enabled.
* The Test as role/view as role feature will show only reports from semantic models workspace.
* The Test as role/View as role feature doesn't work for paginated reports.
