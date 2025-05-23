# EasyPalHelper (EPH)
This program is intended to be used alongside EasyPal to provide some additional functionality not originally included with EasyPal and/or work around some of EasyPal's limitations. EasyPalHelper also provides an Ftps wrapper for the Ftps program used by EasyPal ("Patch EasyPal Ftps")

The extra functionality includes:
1. Notifications
   - allowing both senders and receivers to see the notifications that are posted
   - provides statistics by receiver and sender (where sender callsign is available).
   - Logs received notifications to a file in the EasyPalHelper data directory (%APPDATA%\EasyPalHelper\NotificationLog.csv). This file can be imported very easily into a spreadsheet program for further analysis).
3. On Air Status - allows additional information to be added about the station details (such as first name, grid ref) and tables all information. It also continuously updates the onair status so that users can tell if/when a status becomes 'stale'.
4. Provides an Ftps wrapper for the Ftps program used by EasyPal ("Patch EasyPal Ftps") so that a substitute server can be used in place of the hardcoded Ftps server set up by the original author. Updates to the config also update this config as well (provided the patch has been applied).
5. Introducing the concept of a 'station identifier' so that users can run multiple transceivers and the RX notifications are independent. For example a user may have a 'local' and 'remote' station. These can be identified separately with notifications sent for each. Station identifier is limited to three alphanumeric characters.

The software is built using the National Instruments (NI) Labview (LV) IDE, and requires the LV runtime environment to run.
The EPH installer is available with or without the runtime. You may choose to install the LV runtime separately directly from NI, in which case you can use the 'NoLVRuntime' installer. To download the LV runtime installer direct from NI you will need to create a National Instruments account (no charge). Updates (where the runtime has not changed significantly) can be performed with the 'no runtime' installer.

The original author of EasyPal provided a common server for notifications and on-air status. That server no longer exists and it is not the intention of this author to provide a replacement. To make notifications and on-air status work well, it is recommended:
1. You set up a common ftp server for your EasyPal group (a qsl.net account works well for this).
2. Distribute these details to your group members.
3. Each group member sets EasyPal to use a "User Defined Server" with the common ftp server details and enters these details in EPH as well.
Note: QSSTV users can also use these details in their config.

### System Requirements:
* Win 10 or later
* NI LabVIEW Runtime 2024 Q3 (can be installed with EPH using the applicable installer)

### Installation
To install the EPH software.
1. Download EasyPalHelper to your computer (from this repository in 'releases').
2. Double click on the installer to run the installer. Use the defaults unless you specifically want something different and know the implications of using different values.

### Configuration
To configure the software for your station, firstly click on the "Setup Etc" tab. Then:
   1. Click on the "Station Details" tab. Fill in your station details.
   2. Click on the "Notifications Server" tab. Fill in the details of your server account you are using for notifications. The path should normally not need to be changed.
   3. Click on the "OnAirStatus Server" tab. Fill in the details of your server account you are using for on air status. The path should normally not need to be changed.
   4. Click on "Save and Reinitialise" button to save your configuration.

Most users will enter the same information for the Notification server and the On Air Status server.

If you need to patch EasyPal Ftps (indicator is amber and says "Needs Patching/Updating"), then click on "Patch EasyPal Ftps" button.

Some parameters provide more information if you 'hover' over them using your mouse. This has been done where it was thought additional information would be helpful.

We thank/acknowledge silent key Eric (VK4AES) as the author of the original EasyPal program. Unfortunately, by all accounts, the source was lost with his passing and so updates to that software are not possible.

