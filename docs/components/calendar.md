---
layout: default
title: Calendars
parent: Components
nav_order: 2
---

### Calendar of Events

The calendar custom function grabs data from a Google spreadsheet (calendar) and embeds Google calendars within an iframe on the page.  It uses the spreadsheet information to get the associated Google ID, iframe embed code, museum and title.

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Paste the following code block
- Adust parameters as needed

**Code block for calendar of events**
```
<script>
$(document).ready(function() {
  // Selector, ActiveTab, Expanded
  build_calendars('#calendarDiv',1, false);  
})
</script>
<div id="calendarDiv"></div>
``` 
By default, the resulting calendars are wrapped in an accordian that is normally compressed 
when the page is displayed.  

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
      <td><em>Expanded</em></td>
      <td>Optional.
        <ul>
          <li>True=Initially expanded (Default)</li>
          <li>False=Initially collapsed</li>
        </ul>
      </td>
    </tr>

  </tbody>
</table>

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [Calendar spreadsheet data]({{site.mybase}}/spreadsheets/calendar.html)

