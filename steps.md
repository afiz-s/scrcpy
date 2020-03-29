### Steps to run SCRCPY Steps to run SCRCPY 

1. Enable USB debugging on the phone 
	- Tab 7 times on mobile build number to enable developer options. 
2. Connect the phone with USB 
3.  Run `adb usb` command 
4. Run `scrcpy` to enable the screen copy 

### For Wireless 

Follow the first two steps as above and then 
1. Run `adb tcpip 5555` command (enables adb over tcp/ip for the phone)
2. Disconnect the USB 
3. Run `adb connect <PHONE_IP>.2:5555` 
4. Run `scrcpy` to enable the screen copy

Note: Run `adb usb` command to switch back to USB mode
