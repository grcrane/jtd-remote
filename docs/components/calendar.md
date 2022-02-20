---
layout: default
title: Calendar of Events
parent: Components
nav_order: 2
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
By default, the resulting calendars are wrapped in an accordian that is normally compressed 
when the page is displayed.  

**Syntax:**

*build_calendars(Selector, Activetab, Expanded)*

**Parameters:**

| Parameter | Description |
| :-------- | :---------- |
| *Selector*  | Required.<br>jQuery selector identification where the resulting html code will be generated. |
| *Activetab* |Optional.<br>{::nomarkdown}<ul><li>0=All museums (Default)</li><li>1=Ann Arbor Hands On</li><li>2=Leslie Science</li><li>3=Yankee Air Museum</li><li>4=Challenger Learning center</li></ul>{:/}|
| *Expanded* |Optional.<br>{::nomarkdown}<ul><li>false=Compress on open (Default)</li><li>true=expanded on open</li></ul>{:/}|

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [Calendar spreadsheet data](/jtd-remote/docs/spreadsheets/calendar.html)


site.gh_edit_repository={{ site.gh_edit_repository }}<br>
site.gh_edit_view_mode={{ site.gh_edit_view_mode }}<br>
sit.gh_edit_branch={{ site.gh_edit_branch }}<br>
site.gh.edit_source={{ site.gh_edit_source }}<br>
page.path={{ page.path }}<br>
site.gh_edit_link_text={{ site.gh_edit_link_text }}<br>
                  </p>