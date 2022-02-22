---
layout: default
title: Frequently Asked Questions
parent: Components
nav_order: 3
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
| *Single* |Optional.<br>{::nomarkdown}<ul><li>True=Show only the active museum tab.</li><li>False=All museums (Default)</li></ul>{:/}|
| *OpenFirst* |Optional.<br>{::nomarkdown}<ul><li>True=Automatically open the first faq question for the selected museum.</li><li>False=All faq questions closed on initial open.</li></ul>{:/}|
| *Collapasble* |Optional.<br>{::nomarkdown}<ul><li>false=Not collapsable</li><li>true=Can be collapsed or expanded (Default)</li></ul>{:/}If true you will see a link above the tabs to open/close|
| *Collapsed* |Optional.<br>{::nomarkdown}<ul><li>false=Initially expanded (default)</li><li>true=Initially collapsed</li></ul>{:/}Collapsable must be set to true, otherwise this paramter is ignored.|

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [FAQ's spreadsheet data]({{site.mybase}}/spreadsheets/faq.html)

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td><em>Selector</em></td>
      <td>Required.<br>jQuery selector identification where the resulting html code will be generated.</td>
    </tr>
    <tr class="w3-white">
      <td><em>Activetab</em></td>
      <td>Optional.
      	<ul>
      		<li>1=Ann Arbor Hands On (Default)</li>
      		<li>2=Leslie Science</li>
      		<li>3=Yankee Air Museum</li>
      		<li>4=Challenger Learning center</li>
      	</ul>
	   </td>
    </tr>
    <tr>
      <td><em>Single</em></td>
      <td>Optional.
        <ul>
          <li>True=Show only the active museum tab.</li>
          <li>False=All museums (Default)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><em>OpenFirst</em></td>
      <td>Optional.
        <ul>
          <li>True=Automatically open the first faq question for the selected museum.</li>
          <li>False=All faq questions closed on initial open. (Default)</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><em>Collapasble</em></td>
      <td>Optional.
        <ul>
          <li>Frue=Can be collapsed or expanded (Default)</li>
          <li>False=Not collapsable</li><li>true=Can be collapsed or expanded (Default)</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><em>Collapsed</em></td>
      <td>Optional.<br>
      Collapsable must be set to true, otherwise this paramter is ignored.
        <ul>
          <li>True=Initially collapsed</li>
          <li>False=Initially expanded (default)</li><li>true=Initially collapsed</li>
        </ul>
      </td>
    </tr>

  </tbody>
</table>

