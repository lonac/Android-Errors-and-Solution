# Android-Errors-and-Solution
-Some problems I encountered during learning Android Apps Development and the solution i used

### Note
a) I am using Ubuntu 16.04 on my computer</br>
b) I have successfully installed Android studio

**Problem 1:**
> *On running the App as debugging to Android phone connected to computer through USB, 
I got error says Insufficient permission for the device with ADB* 
>
**soln**</br>
Open *terminal and type the below command* </br>
- $adb kill-server </br>
- $sudo adb startserver </br>
After that unplug the USB and plug it back



