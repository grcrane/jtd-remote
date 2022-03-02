---
layout: default
title: Flip Boxes <span class="new">(Updated)</span>
parent: Components
nav_order: 9
---

### Flip Boxes

Home page flip boxes for Visit, Learn and Support.

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
  build_flipcards("#flexbox"); 
});
</script>
<div id=flexbox></div>
```

**Overrides:**

None

**Usage:**

*build_flipcards(Selector, Boxnumber)*

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
      <td>Boxnumber</td>
      <td>Box number from column A in spreadsheet.  Default=1.  The spreadsheet can contain multiple variations of the flipboxes, each with unique number. 
      </td>
    </tr>
  </tbody>
</table>

**Return Value:**

None

**Spreadsheet:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Detail</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>Owner</td>
      <td>aahom220@gmail.com</td>
    </tr>
    <tr>
      <td>File Name</td>
      <td>Flip Boxes</td>
    </tr>
    <tr>
      <td>Folder</td>
      <td><a href="https://drive.google.com/drive/folders/1YaVLSr9quHsbMDChBrlZUjpI_ZeG0cG-" target="_blank">UIL_Web_Site_Docs</a></td>
    </tr>
    <tr>
    	<td>Link</td>
    	<td><a href="https://docs.google.com/spreadsheets/d/1wEfSb4Dnjz-eNEayaNiiws3ta1ZEueiQyG5-BTWSXag/edit?usp=sharing" target="_blank">https://docs.google.com/spreadsheets/d/1wEfSb4Dnjz-eNEayaNiiws3ta1ZEueiQyG5-BTWSXag/edit?usp=sharing</a></td>
    </tr>
    <tr>
      <td>ID</td>
      <td>1wEfSb4Dnjz-eNEayaNiiws3ta1ZEueiQyG5-BTWSXag</td>
    </tr>
    <tr>
      <td>Sheet Name</td>
      <td>Cards2</td>
    </tr>
  </tbody>
</table>