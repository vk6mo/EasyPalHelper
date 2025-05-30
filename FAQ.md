# Frequently Asked Questions


### What does the Status indicator (green, orange, red) tell us?

The status indicator tells us how long it has been since the station updated its status. 
* Green - the station updated its status within the last 5 minutes
* Amber - the station hasn't updated its status within the last 5min but it has updated its status less than 4hrs ago.
* Red - its been longer than 4hrs since the station updated its status.

You can see the time a station last updated its status by the "LastUpdated" field. The 'traffic light' gives a quick visual representation of whether the status is current.
EasyPalHelper very regularly updates the status so you have a high confidence that the station is still active and has internet connectivity etc.

### What is the Station Identifier all about? How do I use it?

There are a couple of things to understand to answer this. Firstly, running two (2) sessions of EasyPal with the same callsign can create unpredictable results (even if on different computers) due to the way EasyPal works. Also, many hams now run multiple transceivers with separate antennas etc etc etc.  

Station identifier introduces a way to have two (or more) setups of gear running with the same callsign and denote each station with a separate "station Identifier". That then means they can each send notifications separately and those notifications can be seen by others as separate notifications.  
  
An example might best illustrate this:  

'Mark' runs a local station at his house and also a remote station which he connects to via remote rig software. Using the station identifier, he could set the station identifier of his house station as "1" and his remote station as "2".
Now, when Mark receives a picture, each station will report separately, and others will see two separate reports from Mark - one identified with his callsign and a "1", the second identified with callsign and a "2".  
  
The station identifier can be a bit more descriptive than just 1, 2, etc. The software allows three (3) alphanumeric characters (this restriction is to keep file sizes down so the limits are unlikely to be exceeded).
So a better solution for Mark might be to set the station identifier for his home station as "HOM" and his remote station as "REM".   
Fellow hams can now see Marks two reports and easily identify which came from his home setup and which came from his remote setup.







