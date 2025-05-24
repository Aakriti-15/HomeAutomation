# HomeAutomation
# 🔌 Home Automation using ESP8266 & Arduino

This project is a basic **home automation system** built using an **ESP8266 Wi-Fi module**, controlled through a web interface. Users can turn devices ON/OFF by clicking buttons hosted on a local web server, accessed over Wi-Fi.

---

##  Features

- Control GPIO pins (D4 and D5) remotely via a web browser.
- Real-time ON/OFF state display on the web page.
- Simple and responsive HTML/CSS interface.
- Can be used for automating home appliances like lights and fans.

---

##  Components Used

- ESP8266 Wi-Fi Module
- Arduino UNO
- Relay Module (for connecting AC appliances)
- Jumper Wires
- Breadboard / PCB
- Power Supply

---

##  How It Works

1. The ESP8266 connects to your Wi-Fi using the provided SSID and password.
2. A web server is hosted on port `80`.
3. When accessed through a browser, it displays buttons for GPIO 4 and 5.
4. Clicking a button sends an HTTP GET request to the ESP8266, triggering the relay.

---

##  Web Interface Preview

```html
<button>ON</button>    <button>OFF</button>

## edit these lines to match your wifi name and pass
const char* ssid = "YOUR_SSID";
const char* password = "YOUR_PASSWORD";




