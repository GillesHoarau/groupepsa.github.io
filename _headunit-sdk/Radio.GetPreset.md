---
title: Radio.GetPreset()
layout: headunit-sdk
supported:
  - 2
  - 3
  - 4
type: api
---

### `Radio.GetPreset()`

| **Description** | Indicates the saved preset corresponding to the current frequency.
| **Response** | *Number*  If the current frequency matches a saved preset returns the number < 6 corresponding to it, else returns 0.
| **Parameter**   | *Void*

#### Example

```javascript
if (Radio.GetPreset() === 0) {
	// Current frequency does not correspond to a preset frequency
} else {
	// The frequency has been defined as a preset by the user
}
```