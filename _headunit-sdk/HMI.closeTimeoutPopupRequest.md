---
title: HMI.closeTimeoutPopupRequest
layout: headunit-sdk
supported:
  - 2
  - 3
  - 4
type: event
---
Event triggered when no button is clicked on the HMI popup request and the timeout expires.

### Example

```javascript
try {
	// HMI
	if ((typeof HMI !== "undefined") && (typeof HMI.addEventListener !== "undefined")) {
		HMI.addEventListener("closeTimeoutPopupRequest", TimeoutAction());
	}
} catch(e) {
	DealWithHMIError(e);
}
```