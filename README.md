
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


