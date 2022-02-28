---
layout: default
title: fetchgoogledataall <span class="new">(Updated)</span>
parent: Supporting Functions
nav_order: 3
---

### fetchGoogleDataAll

Use promise to fetch data from Google spreadsheets and return resulting parsed Json array(s). 

***Usage***

```
fetchGoogleDataAll([url]).then(dataArray => {
	// dataArray[1] has error message
	// dataArray[0][0] has results from 1st URL
	// dataArray[0][1] has results from 2nd URL etc.
	if (dataArrayx[1]) {  // if there was a status error of some kind
		// do something about the error
		return; 
	}
	dataArray = dataArray[0][0].table.rows; // gets the spreadsheet row data

	// Process the data

}
```

**Parameters:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>urls</td>
      <td>An array of url's to fetch i.e. ['https:...','https:...']</td>
    </tr>
  </tbody>
</table>

**Return Value:**

Returns array with two values:
1=Array of data
2=status or error message
