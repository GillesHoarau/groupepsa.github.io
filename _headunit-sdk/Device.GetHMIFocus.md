---
title: Device.GetHMIFocus()
layout: headunit-sdk
supported:
  - 2
  - 3
  - 4
type: api
---

### `Device.GetHMIFocus()`

| **Description** | Get the focus of the HMI
| **Response** | *boolean* `True` if focus is on portal, else `False`
| **Parameter**   | *Void*

#### Example

```javascript
if (Device.GetHMIFocus() === False) {
	//focus is not on portal
} else {
	//focus is on portal
}
```