# EasyPalHelper
This program is intended to be used alongside EasyPal to provide some additional functionality not originally included with EasyPal and/or work around some of EasyPal's limitations. EasyPalHelper also provides an Ftps wrapper for the Ftps program used by EasyPal ("Patch EasyPal Ftps")

The extra functionality includes:
1. Notifications
   a. allows both senders and receivers to see the notifications that are posted
   b. provides statistics by receiver and sender (where sender callsign is available).
   c. Logs received notifications to a file in the EasyPalHelper data directory (%APPDATA%\EasyPalHelper\NotificationLog.cxv). THis file can be imported very easily into a spreadsheet program for further analysis).
3. On Air Status - allows additional information to be added about the station details (such as first name, grid ref) and tables all information. It also continuously updates the onair status so that users can tell when the status becomes 'stale'.
4. Provides an Ftps wrapper for the Ftps program used by EasyPal ("Patch EasyPal Ftps") so that a substitute server can be used in place of the hardcoded Ftps server set up by the original author. Updates to the config also update this config as well (provided the patch has been applied.
5. Introducing the concept of a 'station identifier' so that users can run multiple transceivers and the RX notifications are independent. For example a user may have a 'local' and 'remote' station. THese can be identified separately with notifications sent for each.

The software is built using Labview, and requires the Labview runtime environment to run.
The installer is available with or without the runtime. Updates (where the runtime has not changed significantly) can be performed with the 'no runtime' installer.

To use EasyPal Helper, in simple terms
1. Install EasyPalHelper
2. Set up the configuration for you, located on the "Setup Etc" tab. Note there are three (3) tabs of setup information. Most users will enter the same information for the Notification server and the On Air Status server

To make notifications and on-air status work well, it is recommended:
1. You set up a common ftp server for your EasyPal group (a qsl.net account works well for this).
2. Distribute these details to your group members.
3. Each group member sets EasyPal to use a "User Defined Server" with the common ftp server details.
Note: QSSTV users can also use these details in their config.

We thank/acknowledge silent key Eric(VK4AES ) as the author of the original EasyPal program. Unfortunately, by all accounts, the source was lost with his passing and so updates to that software are not possible.

