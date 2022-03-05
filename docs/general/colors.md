---
layout: default
title: Colors
parent: General
nav_order: 4
description: "Colors"
---

### Standard Colors
The following table shows the standard color schemes used throughout the site.   These colors are defined in styles.css (GitHub AAHOM).  

```
:root { 
    --global-color-unity: 64, 77, 92;
    --global-color-aahom: 60,100,168;
    --global-color-leslie: 109,143,60;
    --global-color-yankee: 237,27,48;
    --global-color-challenger: 237,159,33;
    --global-color-experience: 248,197,21;
}
```

<style>
:root { 
--global-color-unity: 64, 77, 92;
--global-color-aahom: 60,100,168;
--global-color-leslie: 109,143,60;
--global-color-yankee: 237,27,48;
--global-color-challenger: 237,159,33;
--global-color-experience: 248,197,21;
}
table.minimal {
	min-width:  unset;
	width:  auto;
}
div.table-wrapper {
	max-width:  unset;
	width:  auto;
	box-shadow:  unset;
}
</style>

<table class="minimal">
   <thead>
      <tr class="tableTop">
         <th style="width:120px">Museum</th>
         <th>RGB Color</th>
         <th>Sample</th>
      </tr>
   </thead>
   <tbody>
   		<tr>
         <td>unity</td>
         <td>rgb(64, 77, 92)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-unity);">&nbsp;</td>
      </tr>
      <tr>
         <td>aahom</td>
         <td>rgb(60,100,168)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-aahom);">&nbsp;</td>
      </tr>
      <tr>
         <td>leslie</td>
         <td>rgb(109,143,60)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-leslie);">&nbsp;</td>
      </tr>
      <tr>
         <td>yankee</td>
         <td>rgb(237,27,48)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-yankee);">&nbsp;</td>
      </tr>
      <tr>
         <td>challenger</td>
         <td>rgb(237,159,33)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-challenger);">&nbsp;</td>
      </tr>
      <tr>
         <td>experience</td>
         <td>rgb(248,197,21)</td>
         <td style="width:40px;background-color: rgb(var(--global-color-experience);">&nbsp;</td>
      </tr>
   </tbody>
</table>