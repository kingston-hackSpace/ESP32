# ESP32 enterprise Wi-Fi
----

The ESP32 allows for access to Wi-Fi networks. Most Wi-Fi networks require just the ID of the network and a password to allow logging in. Some networks come with additional security considerations and use an additional username credential, enterprise Wi-Fi networks share this characteristic. **Eduroam**, the university Wi-Fi network, is an example of an enterprise network.

----
## Instructions for connecting to enterprise Wi-Fi.

### STEP 1
In the Arduino IDE, download the esp32 board package by espressive (see [intructions here]()). If using the V2 feather board, Make sure you use **'Adafruit ESP32 Feather'** as board. If you're using the ESP32-S3 feather board, use **'Adafruit feather ESP32-S3 no PSRAM'**. Select the Serial port that corresponds to the USB device.

### STEP 2
If you're using enterprise Wi-Fi for the first time, download the **esp32wifiEnterprise** custom library:

  - Go to **"Sketch > Include Library > Manage libraries..."** and search "**esp32wifiEnterprise**"

  - Click the ""Install" button. 
  
  - To test, load the 'Basic Connection' sketch from the examples:
      
      - Go to **"File > Examples... > (scroll down until you see:) esp32wifiEnterprise > Basic Connection"**

### STEP 3
Add the Wi-Fi login details for the local Wi-Fi to the sketch on line 19-21 these are the network ID (eduroam), username (your KU email) and password, see your local enterprise Wi-Fi settings for this. For Kingston University see [this page](https://kingstonuniversity.sharepoint.com/sites/mykingston/mysupport/itsupport/gettingstarted/Pages/Get-connected-to-eduroam.aspx:)

**WARNING! DO NOT give your ID user and passwords to any AI chatbots!!** Ask a hackSpace technician if you need further help setting this up. 

### STEP 4
With the V2 feather board, Press reset button down as download, when the connecting message appears, release the button and the download will take place. With the ESP32-S3, no reset is needed.

### STEP 5 
Make sure the baud rate is set to 115200 in the serial monitor to see the output and check the connection.
