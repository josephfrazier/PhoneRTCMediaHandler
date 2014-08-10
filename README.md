PhoneRTCMediaHandler
====================

An experimental compatibility layer between [SIP.js](https://github.com/onsip/SIP.js) and [PhoneRTC](https://github.com/alongubkin/phonertc), enabling SIP calls in [Cordova](https://cordova.apache.org/) applications.

Usage (adapted from [sipjs-cordova](https://github.com/joseph-onsip/sipjs-cordova)):
-

**Shell:**
```shell
cordova plugin add https://github.com/alongubkin/phonertc
cordova plugin add com.sipjs.phonertc
```

**Javascript:**
```javascript
var SIP = cordova.require('com.onsip.sipjs.sipjs');
var PhoneRTCMediaHandler = cordova.require('com.sipjs.phonertc.mediahandler')(SIP);
var ua = new SIP.UA({
  mediaHandlerFactory: PhoneRTCMediaHandler
});
```
