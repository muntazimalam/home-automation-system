

# 🏠 Home Automation System using NodeMCU and Arduino Cloud

This project demonstrates a cost-effective and scalable **Home Automation System** that allows users to remotely control and monitor electrical appliances via the **Arduino IoT Cloud**, using **NodeMCU (ESP8266/ESP32)** and **relay modules**. The system is designed for real-time performance, intuitive user interaction, energy efficiency, and layered security.

## 📌 Features

* Control appliances remotely via web or mobile app
* Real-time appliance status updates
* Schedule-based automation and rule configuration
* Manual override using physical switches
* Encrypted communication between components
* Expandable system (add sensors, more relays, or voice assistants)

## 🧰 Components Used

| Component                | Quantity  | Description                                |
| ------------------------ | --------- | ------------------------------------------ |
| NodeMCU (ESP8266/ESP32)  | 1         | Wi-Fi enabled microcontroller              |
| Relay Module             | 1-4       | For switching appliances (AC devices)      |
| Arduino IoT Cloud        | -         | For remote monitoring and control          |
| Electrical Appliances    | As needed | Lights, fans, plug points, etc.            |
| Push Buttons / Switches  | Optional  | For local/manual control                   |
| Jumper Wires, Breadboard | As needed | For circuit connections                    |
| Power Supply             | 1         | 5V/3.3V regulated power source for NodeMCU |

## ⚙️ System Architecture

1. **User Interface (Web/Mobile)**: Controls appliances, views statuses, sets schedules.
2. **Arduino Cloud**: Handles communication, user commands, automation rules, and syncs devices.
3. **NodeMCU**: Interprets cloud commands and toggles relays accordingly. Sends feedback to the cloud.
4. **Relay Module**: Controls the ON/OFF state of connected appliances.
5. **Appliances**: Operated remotely or locally with manual override.

## 🚀 Setup Instructions

1. **Hardware Setup**

   * Connect relay IN pins to digital pins on NodeMCU.
   * Connect VCC and GND of relay module to NodeMCU.
   * Connect appliances to relay NO (Normally Open) contacts and COM.
   * Optional: Add manual switches to allow local control.

2. **Cloud Setup (Arduino IoT Cloud)**

   * Create an account at [Arduino Cloud](https://create.arduino.cc/).
   * Set up a new "Thing" and link your device.
   * Define cloud variables for each relay (e.g., `light1`, `fan1`).
   * Auto-generate and upload the sketch to NodeMCU.

3. **Testing**

   * Open the dashboard on Arduino Cloud.
   * Use switches or sliders to control appliances.
   * Test real-time feedback and scheduling options.

## 🛡️ Security Features

* All data transmitted via Arduino Cloud is encrypted.
* Only authenticated devices can access or control connected appliances.
* Local control available even during internet outages.

## 🌱 Future Enhancements

* Voice control integration (Amazon Alexa, Google Assistant)
* Motion or temperature-based automation
* Mobile app customization
* Energy usage analytics


## 🧠 Authors

* **Muntazim Alam**
  [LinkedIn](https://www.linkedin.com/in/muntazim-alam-463b4626a) • [GitHub](https://github.com/muntazimalam)

## 📄 License

This project is licensed under the MIT License. Feel free to modify and expand!

