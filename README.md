# Promised AngularJS wrapper for SweetAlert
[![Dependency Status](https://gemnasium.com/badges/github.com/LucianoGraziani/ngSweetAlert.svg)](https://gemnasium.com/github.com/LucianoGraziani/ngSweetAlert)

AngularJS wrapper for [SweetAlert](t4t5.github.io/sweetalert/) built with Promises. Sweet Alert is a beautiful replacement for Javascript's "Alert".

## Dependencies
- Required:
	[AngularJS](https://github.com/angular/angular).
	[sweetalert](https://github.com/t4t5/sweetalert).

## Install
1. Download the files, or
2. with Bower: `bower install --save ng-sweet-alert-promised`.
3. Include the file in your app:
	1. `ng-sweet-alert.js` OR `ng-sweet-alert.min.js`.
	2. `sweetalert.js` OR `sweetalert.min.js`.
	3. `sweetalert.css`.
3. Include the module in angular (i.e. in `app.js`) - `ngSweetAlert`.

## Examples

### Simple

```js
SweetAlert.success({
	message: "Here's a message"
}).then(function () {
	// User closed alert
});

```

### With cancel

```js
SweetAlert.warning({
	message: "Are you sure?",
	text: "Your will not be able to recover this imaginary file!",
	showCancelButton: true,
	confirmButtonColor: "#DD6B55",
	confirmButtonText: "Yes, delete it!"
}).then(function () {
	// User accepted
}, function () {
	// User declined
});
```
