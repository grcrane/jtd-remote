---
layout: default
title: Filters <span class="new">(Updated)</span>
parent: Components
nav_order: 15
---

### Filter Checkboxes

Filter summary blocks based on assigned categories.   

***Cook book to create a carousel summary block***
- Edit the page
- Click the "+" sign where you want the carousel to appear
- Select **Summary Block**
- Under ***content*** 
	- select the appropriate blog to display
	- Primary Metadata: None
	- Secondary Metadata: **Category**
	- Filter Items: If needed
- Under ***Design*** 
	- Select **Grid**
	- Number of items: 30 (max)
	- Aspect Ratio: 3:2 Standard
	- TEXT M, Left adjusted
	- Title: **checked**
	- Featured Image: **checked**
	- Ecerpt: **checked**
	- Read More Link: **checked**
	- Set Read more link text: Leave alone
	- Metadata Postion: Below Content
	- Size and Spacing: 
		- Column Width: 270px
		- Gutter Width: 60px
		- Use Columns number instead: No
- Under ***Lazy Settings***
	- Ignore for now, leave off
- Under ***Additional***
	- Ignore for now, leave off

***Cook book to add Slick Carousel***
- Edit the page
- Click a "+" sign just above the summary block, in the same section 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for calendar of events**
```
<script>
$(document).ready(function () {
    filterSelections('#filterContainer',
        'grades:checkbox:Grades,' +
        'outreach:checkbox:Outreach',false); 
});
</script>
<div id="filterContainer"></div>
``` 
The above example has 2 groups, comma separated, of category selections.

- grades: will be a group of grades checkboxes, labeled "Grades".  
- outreach: will be a group of outreach checkboxes with the label "Outreach". 
 
**Overrides:**

None

**Usage:**

*filterSelections(SelectorID, Filters, Lazy)*

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
    <tr>
      <td>Filters</td>
      <td>group<:[radio|checkbox]><:[label]>
      </td>
    </tr>
    <tr>
      <td>Lazy</td>
      <td>True or False selection for Lazy Settings.  If True then Lazy Settings must be enabled.  This extends the SquareSpace 30 record limit for summary blocks.  Default is false.
      </td>
    </tr>
  </tbody>
</table>

**Return Value:**

None
