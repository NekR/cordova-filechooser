Cordova FileChooser Plugin

Requires Cordova >= 2.8.0

Install with Cordova CLI
	
	$ cordova plugin add http://github.com/NekR/cordova-filechooser.git

Install with Plugman 

	$ plugman --platform android --project /path/to/project \ 
		--plugin http://github.com/NekR/cordova-filechooser.git

API

	fileChooser.pick(type, successCallback, failureCallback);

where type can be "audio", "video", "image" and "*".

The success callback get the uri of the selected file

	fileChooser.pick("image",function(uri) {
		alert(uri);
	});

	
Screenshot

![Screenshot](filechooser.png "Screenshot")


