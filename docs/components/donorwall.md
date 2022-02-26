---
layout: default
title: Donor Wall <span class="new">(Updated)</span>
parent: Components
nav_order: 8
---

### Donor Wall

List of donors

The **do_donor_wall** custom function grabs data from a Google spreadsheet (Donor Wall) and creates a list of donors grouped by amount breakpoints.  

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
    do_donor_wall('#donorWall');
});
</script>
<div id="donorWall"></div>
``` 

**Overrides:**

None

**Usage:**

*do_donor_wall(Selector)*

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

**Donor Wall Dependancies**
- **function do_donor_wall**
  - Located in **AAHOM** GitHub repository **UIL** in file **unity.js**
  - See: [https://github.com/AAHOM/UIL/blob/main/unity.js](https://github.com/AAHOM/UIL/blob/main/unity.js){:target="_blank"}
- Code block (see above)
- See: [Donor Wall spreadsheet data]({{site.mybase}}/spreadsheets/donorwall.html)

