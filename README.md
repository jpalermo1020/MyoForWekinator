# MyoForWekinator
A simple data router to ease experimenting with the Myo Armand and Wekinator 


YOU MUST HAVE THE MYO OBJECT FOR MAX by Jules Francoise INSTALLED ALREADY:
https://github.com/JulesFrancoise/myo-for-max#:~:text=myo%20for%20max,Humanities%20Research%20Council%20(SSHRC).

YOU MUST HAVE MYO CONECT INSTALLED BEFORE THIS CAN BE USED:
https://support.getmyo.com/hc/en-us/sections/200934509-Myo-Connect

This patch is intended to help speed up using the Myo armband with max/msp! Simply copy the bpatcher into your patch and you’re good to go!  

Download and Assembly: Copy the “MyoForWek” patch into your externals folder. If you want to use the prebuilt bpatcher with tabs I made then just copy it from “MyoForWek_Bpatcher”. “MyoForWek” has a udpSend built in and is communicating to Wekinator on Port 6448.


TABS:
Features:  This should be used while Wekinator is still on the setup page. It will auto-populate the input numbers and names as you make your choices.

Device: 
*Myo Connect must be running* 
This tab is where you’ll interface with the Myo armband itself. You can print the device list to the max window to check if max is seeing the Myo armband! Click “connect” once you see your device in the max window. There are a few  displays for information like the device name, the arm sync information, and  the battery amount. At the bottom you can choose to stream the data from the Myo continuously or poll at a given millisecond rate. 

Device unlock: This is checked by default. If device unlock is enabled then the Myo will continuously output gestures when it “see’s” them. If  you disable device unlock then the Myo will only send gesture data for a short time after performing the “double tap” gesture.

Data:
Here you’ll see your incoming data (besides the EMG chart). You can choose here  to gate different sets of data if you so choose. 

The “Set Origin” option will set a new “0,0,0,0” location for wherever your arm is currently positioned in space. This can be useful if you want all motion to be based off of the change from a  position like “your arm flat on the table” for instance.

EMG:
Here you’ll see a scrolling display of all 7 EMG outputs at once.
