## v2

### v2.1.2

* added option `maxFileSize` for specyfying max file size available for upload, in bytes. Use 0 for turning it off.
* added option `maxUploadedItems` for specyfying max item count. Default is set to 10, use 0 for turning it off.
* added new emited event `error` with token `this.errorMsg`, which is called everytime when some error shows up from when you put some files on dropzone.
* added options `allowedFileTypesErrorMsg`, `maxUploadedItemsErrorMsg` and `maxFileSizeErrorMsg` with token `__FILENAME__`, where you are able to specify emited error msg.
* Added indexOf polyfil for IE8 so now it should work in ie8 too, i need to test it..


### v2.1.1

* fixed bug when updating default theme (usually by error msg)
* fixed state names and state messages


### v2.1.0

* refactored js
* refactored API - now it is more using friendly and more error proof
* changed methods of rendering and updating theme
* a little performace savings
* default theme is generated and stored by init. Customizing by `Dropzone.customizeTemplate()` generate new template and replace default template in storage. When you `Dropzone.show()` or `Dropzone.hide()`, script use stored template and will not generate template again. On `Dropzone.updateState()` it only makes changes in rendered DOM, not in stored template.


### v2.0.0

* refactored js
* Dropzone can now run multiple instances on one page
* Every Dropzone object instance is now marked with it's own generated ID
* Refactored object Options
* added optional setting `allowedFileTypes` to Options
* xhr from uploaded files are stored also in `xhrResponseArray` array, since uploading another file/files on same Dropzone instance
* updated Readme.md


---
## v1

### v1.3.0

* Fixed reserved names
* Added back-end api json
* JSLinted a index.js file a bit

### 1.2.0

* Fixed previous merge
* Input file is now reseting
* Test if I get ohter status than 200 in response from server
* Error state is now reversible to default state on click

### 1.1.0

* Fixed state templates issues
* Added ~~Dropzone.stateTemplates()~~ Dropzone.templateStates() function
* Improved example.html to show new features

### 1.0.0

* First public release