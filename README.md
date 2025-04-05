
![image](https://github.com/user-attachments/assets/3e2ba871-123f-4a4b-ab95-1231f029d43d)

# 🔒 Arduino Keyboard Logout & Lock Trigger

This project demonstrates how to use an **Arduino Leonardo** or **Arduino Micro** to simulate keyboard actions that **log out** or **lock** a computer with the press of a button.

When pin **D2** is connected to **GND**, the Arduino sends a sequence of keystrokes depending on your selected platform:
- 🔐 **Windows**: Locks the screen (`Win + L`)
- 🔒 **macOS**: Logs out using `Cmd + Shift + Q`, then `Enter`
- 🔓 **Ubuntu**: Triggers logout using `Ctrl + Alt + Del`, then `Enter`

> ⚠️ Make sure you understand what each combination does before testing on your system.

---

## 🧠 How It Works

- Uses the **Arduino Keyboard library** to send keyboard commands over USB.
- Detects a digital input (pin D2) connected to **GND**.
- Sends OS-specific key sequences based on the configured platform.

---

## 🛠️ Requirements

- Arduino **Leonardo** or **Micro**
- Jumper wire or button to connect **D2 to GND**
- Arduino IDE installed with the `Keyboard` library

---

## ⚙️ Setup

1. Clone the repo and open the `.ino` file in the Arduino IDE.
2. Set your platform inside the code:
   ```cpp
   int platform = WINDOWS; // Change to OSX or UBUNTU as needed

Upload to your Arduino Leonardo/Micro.

Press the button or short D2 to GND to trigger.

🖥️ Platform Logic
Platform	Key Sequence Sent	Action
WINDOWS	Win + L	Lock PC
OSX	Cmd + Shift + Q + Enter	Logout
UBUNTU	Ctrl + Alt + Del + Enter	Logout
🚧 Important Notes
This only works on boards that support USB HID like Leonardo or Micro.

Do not use this without permission on someone else's device.

Timing delays may need adjustment depending on system speed.

📸 Demo (Optional GIF or image)
Add a demo GIF or photo here if available.

📄 License
This project is released into the public domain.

🤝 Contributing
Feel free to fork and submit pull requests for improvements, bug fixes, or extra features like:

Dynamic OS selection

LED indicators

Sleep/Wake functionality

👨‍💻 Created by: [Harsha Vardhan Raju.Yerra]
![image](https://github.com/user-attachments/assets/45d712e4-d9bf-4d85-8a75-9b4979e07647)
![WhatsApp Image 2025-04-05 at 23 15 12_b086874a](https://github.com/user-attachments/assets/5bb62302-bf06-4ad5-97af-96a73235c5dc)
![WhatsApp Image 2025-04-05 at 23 17 39_fb487924](https://github.com/user-attachments/assets/3735b218-9693-462e-8901-caf1ce8511f8)

---










