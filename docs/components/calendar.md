---
layout: default
title: Calendars <span class="new">(Updated)</span>
parent: Components
nav_order: 2
---

### Calendar of Events

The calendar custom function grabs data from a Google spreadsheet (calendar) and embeds Google calendars within tabbed list on the page.  It uses the spreadsheet information to get the associated Google ID, iframe embed code, museum and title.

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for calendar of events**
```
<script>
$( document ).ready(function() { 
  // selector, activeTab, single, collapsable, collapsed 
  build_calendars('#calendarContainer',1,false, true, false);
});
</script>
<div id="calendarContainer"></div>
``` 

**Overrides:**

You can dynamically override *ActiveTab* by adding a parameter to the linking url as:

```
?tab=n  (where n is a number from 0-4, see ActiveTab below)
```

**Usage:**

*build_calendars(Selector, Activetab, Expanded)*

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
          <li>0=All museums (Default)</li>
          <li>1=Ann Arbor Hands On</li>
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
      <td><em>Collapasble</em></td>
      <td>Optional.
        <ul>
          <li>True=Can be collapsed or expanded (Default)</li>
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
- **function build_calendar**
  - Located in **AAHOM** GitHub repository **UIL** in file **unity.js**
  - See: [https://github.com/AAHOM/UIL/blob/main/unity.js](https://github.com/AAHOM/UIL/blob/main/unity.js){:target="_blank"}
- Code block (see above)
- See: [Calendar spreadsheet data]({{site.mybase}}/spreadsheets/calendar.html)

