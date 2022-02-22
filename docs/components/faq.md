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
  // selector, ActiveTab, Single, OpenFirst, Collapsable, Collapsed 
  do_faqs2('#faq_container',2,false,true,true,false);
});
</script>
<div id="faq_container"></div>
```
*Note:* This example will place the resulting html code in the #faq_container selector (Selector).  The second tab (ActiveTab) will be selected (Leslie Science).  Since Single is set as false, all museum tabs will be visible.  If Single was set to true then only Leslie Science would be showing.  OpenFirst is set to true, which says that the first question will be automatically open on the initial display (unless on mobile). Collapsable is set to true, which says to add an expand/collapse toggle link above the tabs.  Collapsed being false, says that the tabs will be initially expanded when page is first visited.  

**Usage:**

*do_faqs2(Selector, Activetab, Single, OpenFirst, Collapsable, Collapsed)*

**Parameters:**

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
      <td><em>ActiveTab</em></td>
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
          <li>False=Initially expanded (default)</li>
        </ul>
      </td>
    </tr>

  </tbody>
</table>

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [FAQ's spreadsheet data]({{site.mybase}}/spreadsheets/faq.html)

