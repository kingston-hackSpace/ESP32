# ESP32 enterprise wifi
----

The ESP32 allows for access to wifi networks. The process for logging into a enterprise network requires additonal parameters due to increased security considerations.

----
## Instructions for loading connecting to enterprise wifi.

### STEP 1
In the arduino IDE download the esp32 board package by espressive. Make sure you use ESP32 Dev Module as board, serial port that corresponds to the USB device.

### STEP 2
If you're using enterprise wifi for the first time, download the esp32wifiEnterprise custom library. Go to manage libraries and search. To test, load the login sketch form the examples.

### STEP 3
Add the wifi login details for the local wifi to the sketch on line 19-21 these are the network id, username and password, see your local enterprise wifi settings for this. For Kingston University see [this page](https://kingstonuniversity.sharepoint.com/sites/mykingston/mysupport/itsupport/gettingstarted/Pages/Get-connected-to-eduroam.aspx:)

### STEP 4
Press reset button down as download, when the connecting message appears, release the button and the down load will take place.

### STEP 5 
Make sure the baud rate is set to 115200 in the serial monitor to see the output and check the connection.
