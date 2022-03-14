---
layout: default
title: Icon Bar <span class="new">(Updated)</span>
parent: Components
nav_order: 15
---

### Icon Bar

The icon bar appears above the footer on all pages, plus below the header image carousel on the home page.   There are two spots that code needs to be injected to accomplish this.

The image links for (currently) four museum icons, are hard coded in an array within the javascript library unity.js.   

**Home page advanced code-injection**

```
<script>
$( document ).ready(function() {
  addIconBar('header');
})
</script>
```

**Home page footer section**

***Cookbook***
- Edit any page
- Scroll down to the footer section
- Click "Edit Footer"
- Insert the following code block anywhere

```
<script>
$( document ).ready(function() {
  addIconBar('footer');
})
</script>
```

**Usage:**

*addIconBar(what)*

**Parameters:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td><em>What</em></td>
      <td>Optional.<br>is either "header" (default) or "footer"</td>
    </tr>
  </tbody>
</table>

**Return Value:**

None