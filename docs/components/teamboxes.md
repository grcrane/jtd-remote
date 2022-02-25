---
layout: default
title: Team Members <span class="new">(Updated)</span>
parent: Components
nav_order: 4
---

### Team Members

The team_members custom function grabs data from a Google spreadsheet (teams) and dynamically builds a list of all team members, ordered by last name, first name.  Each team member is displayed in a separate flex box with name and title.  Hovering over team member displays the members profile, if provided.   Clicking on the team member displays the details in a modal box.  It uses the spreadsheet information to get the associated team member information. 

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for team members**
```
<script>
$( document ).ready(function() {
    // SelectorID
    do_team_members('#teamContainer'); 
});
</script>
<div id="teamContainer"></div>
``` 

**Overrides:**

None


**Usage:**

*do_team_members(SelectorID)*

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
  </tbody>
</table>

**Return Value:**

None


**Team Members Dependancies**
- **function team_members**
- **addMyModal**
- **teamCardResize**
  - Located in **AAHOM** GitHub repository **UIL** in file **unity.js**
  - See: [https://github.com/AAHOM/UIL/blob/main/unity.js](https://github.com/AAHOM/UIL/blob/main/unity.js){:target="_blank"}
- Code block (see above)
- See: [Team Members spreadsheet data]({{site.mybase}}/spreadsheets/teamboxes.html)

