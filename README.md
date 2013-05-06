App42_BB10_SDK
====================

App42 Cloud API Client SDK files for BB10 

- [Download] (https://github.com/shephertz/App42_BB10_SDK/raw/master/1.1/app42_BB10_1.1.zip) the latest App42 BB10 SDK

Before you begin:

1. First you have to download ripple simulator and vmplayer to start with BB10 SDK.

2. Make sure that you configure the "Build" settings in the Ripple emulator.

3. Make sure that you store the configuration document (config.xml) file in the project root. 

4. For more information plase visit http://developer.blackberry.com/html5/download/

5. Register with App42 to get ApiKey/Secret Key on click [Get Started] (https://apphq.shephertz.com/register/index)

Add following script tag in your html page

	script type="text/javascript" src="App42-all-x.x.x.min.js"
Initialize your library using following BB10 code.
 	
 	App42.initialize("API KEY","SECRET KEY");
 	
 Instantiate the service that you want to use in your App, for example using User service you have to do following.

 	var user  = new App42User();
 	Now you can call associated method of that service. For example user creation can be done with following snippet.

 	user.createUser(userName, pwd, email,
	{
     	     success: function(object) {
        	 // Callback for Success 
		},
            error: function(error) {
           // Callback for error 
		}
    });
Download the SDK and sample code from our BlackBerry 10 webwork repository to get started.

Running the Sample


Steps : 


a. SDK path - The path to where the BlackBerry 10 WebWorks SDK is installed. The following are the default SDK paths

	Windows XP : C:\Program Files\Research In Motion\BlackBerry 10 WebWorks SDK <version>
	
	Windows 7 : C:\Program Files (x86)\Research In Motion\BlackBerry 10 WebWorks SDK <version>
	
	Mac OS : /Developer/SDKs/Research In Motion/BlackBerry 10 WebWorks SDK <version>

Required: This setting is required to package your application.

b. Project Root - The location of your project. 
	
c. Archive Name - The name you want the archive file to be (for example, App42Sample).
	
d. Output Folder - The location where you want the output to reside. This cannot be the same location as the Project Root.

In launch field

a.Target - Simulator
	
b.Device IP -  The IP address of your BlackBerry 10 simulator.

Note : Make sure that your VMPLAYER is running.
	
The Ripple emulator builds your application. If the build and package completes successfully, the message "Build succeeded!" is displayed.
This option builds, packages, and launches your application on the specified simulator.

The BlackBerry 10 simulator launches your application.
 
	
