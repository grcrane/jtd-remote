---
layout: default
title: Calendar of Events
parent: Components
nav_order: 5
---

### Calendar of Events

The calendar custom function grabs data from a Google spreadsheet (calendar) and embeds Google calendars within an iframe on the page.  It uses the spreadsheet information to get the associated Google ID, iframe embed code, museum and title.

The calendar of events block is emplemented by adding a code block to the page with the following:

**Code block for calendar of events**
```
<script>
$(document).ready(function() {
  build_calendars('#calendarDiv',1, false);  
})
</script>
<div id="calendarDiv"></div>
```
Note that the function call "**build_calendars**" is being passed the number "2", which tells the function to select calendar number 2 (Leslie Science) as the default when opened. 

**Syntax:**

*build_calendars(selector, activeTab, expanded)*

**Where *activeTab* is:**

- 0, All museums (or null) - Default
- 1, Ann Arbor Hands On
- 2, Leslie Science
- 3, Yankee Air Museum
- 4, Challenger Learning Center

**Calendar Dependancies**
- Code block (see above)
- [Spreadsheet data](/Docs/spreadsheets.html)