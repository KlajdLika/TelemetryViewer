# TelemetryViewer
Data Visualization Tool

#How to use BOTA FT Viewer

1.	Download the .jar and layout.txt file. The layout.txt is the default and most simplified example layout for Force Torque data logging for Rokubi 2.10 USB. 
2.	Plug in the sensor in a USB port of your computer. Device manager of Windows will recognize it and will appear as a serial port with name COMx. Where “x” a random number given from the OS to the device. Right click on the icon and choose Properties. Follow the settings found in the snapshots below and click ok.
  


3.	Wait for 2 seconds. Close the device manager windows and execute the bota_ft_viewer.jar
4.	Click on Open Layout and choose the layout.txt file provided and click ok.
5.	Choose the COMx you configured in step 2 from the dropdown menu and click connect.
6.	Once you click connect a pop-up window will appear with the default configuration the layout.txt contains. Press Done and you are done. 
7.	Wait for the Graph window to shrink to the measurements scale.
8.	To bias the sensor’s offset. 
a.	Click disconnect.
b.	Connect to the serial port through a RealTerm: 230400 baudrate, Data bits 8, Parity None, Stop bits 1, Flow control None.
c.	 To bias the sensor to its initial value when the sensor started operating an “a” should be sent to the device through the terminal while online.
d.	To store this bias configuration into the device’s memory you will have 4 seconds to send subsequently a “y”. If you do so, the offset values will be stored into the device. We recommend to do it whenever it is needed. The device’s memory have limited re-writing cycles. Do not apply loads to the sensor while this process is ongoing! 
e.	Connect again through the bota_ft_viewer.
  

