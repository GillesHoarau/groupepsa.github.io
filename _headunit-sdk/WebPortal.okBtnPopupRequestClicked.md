---
title: WebPortal.okBtnPopupRequestClicked
layout: headunit-sdk
supported:
  - 2
  - 3
  - 4
type: event
---

Event triggered when the *OK* button of the popup is clicked.

### Example

```javascript
window.addEventListener("message", function(event){
	
	if (typeof event.data !== 'undefined' && typeof event.data.type !== 'undefined' ){

	    var data = event.data;
	    var type = event.data.type;

	    switch(type){

		//When the application is put in foreground
	    case "WebPortal.okBtnPopupRequestClicked":
		console.log("Popup ok button clicked!");
		alert("Popup ok button clicked!");
		break;
	    
	    }
	}
 });
```