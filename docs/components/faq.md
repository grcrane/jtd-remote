---
layout: default
title: Frequently Asked Questions
parent: Components
nav_order: 5
---

### Frequently Asked Questions

The calendar custom function grabs data from a Google spreadsheet (calendar) and embeds Google calendars within an iframe on the page.  It uses the spreadsheet information to get the associated Google ID, iframe embed code, museum and title.

The frequently asked questions block is emplimented by adding a code block to the page with the following:

**Code block for calendar of events**
```
<script>
$( document ).ready(function() { 
  // selector, activeTab, single, openfirst, collapsable, collapsed 
  do_faqs2('#faq_container',2,false,true,true,false);
});
</script>
<div id="faq_container"></div>
```

**Syntax:**

*do_faqs2(Selector, Activetab, Single, OpenFirst, Collapsable, Collapsed)*

**Parameters:**

| Parameter | Description |
| :-------- | :---------- |
| *Selector*  | Required.<br>jQuery selector identification where the resulting html code will be generated. |
| *Activetab* |Optional.<br>{::nomarkdown}<ul><li>1=Ann Arbor Hands On (Default)</li><li>2=Leslie Science</li><li>3=Yankee Air Museum</li><li>4=Challenger Learning center</li></ul>{:/}|
| *Single* |Optional.<br>{::nomarkdown}<ul><li>True=only one museum</li><li>False=All museums (Default)</li></ul>{:/}|
| *OpenFirst* |Optional.<br>{::nomarkdown}<ul><li>True=only one museum</li><li>False=All museums (Default)</li></ul>{:/}|
| *Collapable* |Optional.<br>{::nomarkdown}<ul><li>false=Not collapsable</li><li>true=Can be collapsed</li></ul>{:/}|
| *Collapsed* |Optional.<br>{::nomarkdown}<ul><li>false=Expanded</li><li>true=Can be collapsed (Default)</li></ul>{:/}|

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [FAQ's spreadsheet data]({{site.mybase}}/spreadsheets/faqs.html)

