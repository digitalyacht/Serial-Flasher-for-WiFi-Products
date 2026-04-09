# Serial-Flasher-for-WiFi-Products

All of our wireless products feature a web interface where firmware updates can be uploaded Over The Air (OTA). However, sometimes for larger updates, where major changes have occurred to the software kernel, it is necessary to update the wireless units using a special 3.3v TTL to USB programming cable.

To make this programming experience as simple as possible and also to allow it to be done on any hardware platform (Windows/MacOSX/LINUX) we have developed this web app that will run on any modern browser that supports the Web Serial API, which currently are Chrome, Chromium, Opera and Edge.

Download and extract the ZIP file and then double click on the index.html file and you should see the web app landing page...
<br>
<img src="https://raw.githubusercontent.com/digitalyacht/Serial-Flasher-for-WiFi-Products/refs/heads/main/images/Landing_Page.png" width=70%>
<br>
Now click on the Baud Rate selection dropdown and select the baud rate required. If you are using a special 3.3v TTL programming cable, then 115,200 baud is the best baud rate to use, but if you are updating one of our WLN10SM or WLN30 via an NMEA 0183 or RS422 type adaptor cable, we recommend using 57,600 or even 38,400 baudrate for reliable communication...
<br>
<img src="https://github.com/digitalyacht/Serial-Flasher-for-WiFi-Products/blob/master/images/Select_Baudrate.png" width=70%>
<br>
