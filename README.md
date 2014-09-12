RingCentral RingOut OS X Service 
=======================

A simple [Mac OS X service][1] built in Automator, using curl, that utilizes the [RingOut API][2] to connect a call to any phone number from your Mac.

#Setup

You'll need to create a file in your home directory:

	mkdir -p ~/.ringcentral
	echo '#Must prefix username with "1".' > ~/.ringcentral/config
	echo RINGCENTRAL_USERNAME=\'17135551212\' >> ~/.ringcentral/config
	echo RINGCENTRAL_PASSWORD=\'mypassword\' >> ~/.ringcentral/config
	
Be sure and edit your username and password above.

#Protips

* If you use a bunch of services, or want to start... Download [Services Manager][3], it will let you add / remove items from the context menu and modify hotkeys.
* I install two copies of the service, I modify the `CALL_ME_HERE` variable in the Automator script so that the other one calls me on my cellphone.

[1]: http://www.macosxautomation.com/services/
[2]: http://service.ringcentral.com/ringoutapi/
[3]: http://www.macosxautomation.com/services/servicesmanager/
