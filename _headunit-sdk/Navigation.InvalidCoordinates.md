---
title: Navigation.InvalidCoordinates
layout: headunit-sdk
supported:
  - 2
  - 4
type: event
---
Event triggered when at least one of the coordinates used with `Navigation.LaunchGuidance` is invalid, due to : Type, size...

### Example

```javascript
try{	
	// Navigation
	if ((typeof Navigation !== "undefined") && (typeof Navigation.addEventListener !== "undefined")) {
		Navigation.addEventListener("InvalidCoordinates", InformUserInvalidCoordinates()	}
} catch(e) {
	DealWithNavigationError(e);
}
```

>**Note :** The Navigation events are triggered only if the Navigation was launched using either `LaunchGuidance` or `LaunchGuidanceWaypoints`.