# ESP32 enterprise wifi
----

The ESP32 allows for access to wifi networks. Most wifi networks require just the id of the network and a password to allow logging in. Some networks come with additional security considerations and use an additional username credential, enterprise wifi networks share this characteristic. Eduroam, the university wifi network, is an example of an enterprise network.

----
## Instructions for connecting to enterprise wifi.

### STEP 1
In the arduino IDE download the esp32 board package by espressive. If using the V2 feather board, Make sure you use 'Adafruit Feather ESP32 V2' as board. If you're using the ESP32-S3 feather board, use 'Adafruit feather ESP32-S3 no PSRAM'. Select the Serial port that corresponds to the USB device.

### STEP 2
If you're using enterprise wifi for the first time, download the esp32wifiEnterprise custom library. Go to manage libraries and search. To test, load the 'Basic Connection' sketch from the examples.

### STEP 3
Add the wifi login details for the local wifi to the sketch on line 19-21 these are the network id, username and password, see your local enterprise wifi settings for this. For Kingston University see [this page](https://kingstonuniversity.sharepoint.com/sites/mykingston/mysupport/itsupport/gettingstarted/Pages/Get-connected-to-eduroam.aspx:)

### STEP 4
With the V2 feather board, Press reset button down as download, when the connecting message appears, release the button and the download will take place. With the ESP32-S3, no reset is needed.

### STEP 5 
Make sure the baud rate is set to 115200 in the serial monitor to see the output and check the connection.
