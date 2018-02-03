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
- $sudo adb start-server </br>
After that unplug the USB and plug it back </br>


**Problem 2:**
> *Error:Unable to resolve dependency for ':app@releaseUnitTest/compileClasspath': Could not resolve com.android.support:design:26.0.0-beta1.
<a href="openFile:/home/…../AndroidStudioProjects/Sandra/app/build.gradle">Open File</a><br><a href="Unable to resolve dependency for &#39;:app@releaseUnitTest/compileClasspath&#39;: Could not resolve com.android.support:design:26.0.0-beta1.">Show Details</a>*
>
**soln**</br>
-Add the marven google url on dependence </br>
``` 
allprojects {
    repositories {
        google()
        jcenter()
        maven {
            url "https://maven.google.com"
        }
    }
} 
```

