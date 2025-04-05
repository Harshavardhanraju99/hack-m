
![image](https://github.com/user-attachments/assets/3e2ba871-123f-4a4b-ab95-1231f029d43d)

🔧 What It Does
Waits for pin 2 to go LOW (connected to GND).

Based on the selected platform (WINDOWS, UBUNTU, or OSX), it sends the appropriate keyboard combination to initiate logout:

Windows: Ctrl + Alt + Delete, then Alt + L (logs off the user).

Ubuntu: Ctrl + Alt + Delete, then Enter (confirms logout).

macOS: Cmd + Shift + Q, then Return (confirms logout).

It then halts by entering an infinite loop (while(true);).

🔌 Hardware Requirements
Arduino Micro or Leonardo (because they support native USB HID).

A push button or jumper wire to connect pin 2 to GND.

Optional: Pull-down resistor if not using INPUT_PULLUP (but it's handled in the code already).

#✅ How to Use
#Upload the sketch to your Arduino Leonardo/Micro.

Set the correct platform by changing:

int platform = WINDOWS;
to your current OS.

Connect D2 to GND (via button or jumper) to trigger logout.

⚠️ Safety Tips
Be careful when testing—this will log you out immediately.

Don’t leave this running plugged into someone’s computer unless it’s part of a controlled demo or you have permission (ethical hacking rules apply!).

💡 Optional Improvements
Add a debounce for the button.

Add LED indicator for status.

Add EEPROM or serial input to change the OS dynamically.
