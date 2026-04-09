# Serial-Flasher-for-WiFi-Products

All of our wireless products feature a web interface where firmware updates can be uploaded Over The Air (OTA). However, sometimes for larger updates, where major changes have occurred to the software kernel, it is necessary to update the wireless units using a special 3.3v TTL to USB programming cable.

To make this programming experience as simple as possible and also to allow it to be done on any hardware platform (Windows/MacOSX/LINUX) we have developed this web app that will run on any modern browser that supports the Web Serial API, which currently are Chrome, Chromium, Opera and Edge.

Download and extract the ZIP file and then double click on the index.html file and you should see the web app landing page...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Landing_Page.png" width=100%>
<br>

Now click on the Baud Rate selection dropdown and select the baud rate required. If you are using a special 3.3v TTL programming cable, then 115,200 baud is the best baud rate to use, but if you are updating one of our WLN10SM or WLN30 via an NMEA 0183 or RS422 type adaptor cable, we recommend using 57,600 or even 38,400 baudrate for reliable communication...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Select_Baudrate.png" width=100%>
<br>

Once the baudrate is selected, click on the CONNECT button and you will be prompted to select the COM port that the USB cable has been allocated by the operating system... 

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Select_Serial_Port.png" width=100%>
<br>

Once selected, make sure you have placed the wireless product in to "bootloader flash mode", which is done by turning the power on to the unit with the RESET button held down. Once powered up, release the RESET button and on the web app, click the CONNNECT button. You should see the communication log in the black terminal window, which confirms that the communication is good and the unit is ready to be updated...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Connected.png" width=100%>
<br>

Now click the "Choose File" button and in the browse for file pop-up that appears, navigate to where you have stored the update file. Please note that only official BIN files, released by Digial Yacht should be used and if you downloaded a ZIP file, make sure to extract the BIN file and select this file for the update. Once you have selected the correct file, the browse for file pop-up will dissappear and the chosen file will be shown...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/File_Chosen.png" width=100%>
<br>

To start the update proess, click the PROGRAM button and the status should be displayed in the black terminal window and in a small status bar graphic...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Flashing.png" width=100%>
<br>

Assuming the update is successful you should see the following text appear in the black terminal window...

<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Completed.png" width=100%>
<br>

Now you can remove the programming cable, power cycle the updated unit, perform a facory reset (always recommended after a major update) by pressing and holding he RESET button on the unit for >10 seconds and when the unit powers back up you will be able to see the new firmware version number in the unit's web interface SETTINGS page (About section).  
