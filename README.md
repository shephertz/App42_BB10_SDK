App42_BB10_SDK
====================

App42 Cloud API Client SDK JAR files for BB10 

Before you begin:
1. First you have to download ripple simulator and vmplayer to start with BB10 SDK.
2. Make sure that you configure the "Build" settings in the Ripple emulator.
3. Make sure that you store the configuration document (config.xml) file in the project root. 
4. For more information plase visit http://developer.blackberry.com/html5/download/
5. Register with App42 to get ApiKey/Secret Key

App42 platform in now equipped with BlackBerry 10 webworks SDK. This means you can make cloud enabled apps with scalable App42 platform with few lines of code java script. You can choose from different business and technical services available in App42 platform to make user engaging and feature rich app for BlackBerry 10.
Here are the few steps to add it in your BlackBerry 10 webworks App

· Add following script tag in your html page
· script type="text/javascript" src="https://raw.github.com/shephertz/App42_BB10_SDK/master/App42-all-0.6.0.min.js"
· Initialize your library using following java script code
· App42.initialize("API KEY","SECRET KEY");
· Instantiate the service that you want to use in your App, for example using User service you have to do following
· var user  = new App42User();
· Now you can call associated method of that service. For example user creation can be done with following snippet
·    user.createUser(userName, pwd, email,{
·       success: function(object) {
·          // Callback for Success },
·        error: function(error) {
·          // Callback for error }
·      });
Download the SDK and sample code from our BlackBerry 10 webwork repository to get started.

Running the Sample

Select Package.

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
 
	
