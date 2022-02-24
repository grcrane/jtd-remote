---
layout: default
title: Faqs <span class="new">(Updated)</span>
parent: Components
nav_order: 3
---

### Frequently Asked Questions

The Frequently Asked Questions custom function grabs data from a Google spreadsheet (faqs) and displays the questions/answers in an accordian style list.  Each museum will have a separate tab, and separate questions based on data from the spreadsheet. 

The frequently asked questions block is emplimented by adding a code block to the page with the following:

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for frequently asked questions**
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

**Overrides:**

You can dynamically override *ActiveTab* by adding a parameter to the linking url as:

```
?tab=n  (where n is a number from 1-4, see ActiveTab below)
```

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
    <tr>
      <td><em>Title</em></td>
      <td>Optional.<br>
      Title line at top, default is "View Location Maps"
      </td>
    </tr>


  </tbody>
</table>

**Return Value:**

None


**Calendar Dependancies**
- Code block (see above)
- See: [FAQ's spreadsheet data]({{site.mybase}}/spreadsheets/faq.html)

