---
type: rule
archivedreason: 
title: Customization - Do you always make backup versions of the XML schema? (CRM 4 only)
guid: eb940a71-b172-409d-bbb4-d95eba36e8e5
uri: customization---do-you-always-make-backup-versions-of-the-xml-schema-crm-4-only
created: 2012-12-10T18:31:19.0000000Z
authors:
- id: 1
  title: Adam Cogan
related: []

---

When the XML schema is published it re-generates the underlying SQL and .aspx code. If trouble hits, a "refresh" or "rollback" to an uncorrupted schema is always a backup plan. A versioning scheme is also required to keep track of different versions of the XML schema at different points in time. To make a backup of the schema from within Microsoft CRM navigate to Settings -> Customization -> Export Customizations. Browse to the location on your personal hard drive where the .XML file is to be stored.

<!--endintro-->
<dl class="image">&lt;dt&gt;<img alt="Microsoft CRM Customization Pane" src="CRM_CustomizationPane.jpg">&lt;/dt&gt;
<dd>Figure: Export customizations as backup </dd></dl>
**Tip #1:** Export only the customizations of entities that you customize and keep each entity customizations in a separate file, see the rule:[Customization](/Pages/Only-export-the-customizations-and-related-ones-that-you-have-made.aspx) - Do you export only the customizations of entities that you did customize?

**Tip #2:** Put the date on the file names and while you are working you will be doing this multiple times a day.

**Tip #3:** don't save this on the Dev Virtual Machine.

In CRM 2011 we use Solutions and TFS Source Control.