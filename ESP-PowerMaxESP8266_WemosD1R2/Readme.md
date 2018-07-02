1. Connect the Wemos to your computer and ensure that it appears in Windows Device Manager as a COM port (serial/USB bridge) - you may need a driver though hopefully it will automatically find it. Take a note of this COM port number.
2. Download the bin file and ESPtool.exe into the same folder and open a command prompt to this folder. (once the folder is open in Windows Explorer then hold shift and right click the background - that will allow you to 'Open a command prompt here')
3. Run the following command to flash the Wemos chip (change COMXX to be COM3 if the COM port identified above is #3): "esptool.exe -vv -cd nodemcu -cb 115200 -cp COMXX -ca 0x00000 -cf PowerMaxEsp8266.ino.bin"
4. You should see a success message, in which case you can start the main instructions above.
