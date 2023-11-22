# Green Campus

The project aims to deploy and configure IoT devices (Rak PiHat) within a LoRaWAN network environment, facilitating seamless connectivity and data transmission for environmental monitoring. Leveraging ChirpStack as the central server, this setup enables real-time monitoring of temperature, air quality, and other environmental parameters across various locations.



## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Configuration](#configuration)
4. [Contributing](#contributing)
5. [License](#license)

## Configuration

### 1. Initial Setup

1. **Download Firmware:**
   - Obtain the Rak PiHat firmware from [this link](https://drive.google.com/file/d/1MoqZ3JeULfrjy7yOFgUPQUoxvpd3ceYY/view?usp=sharing).

2. **Connect to Rakwireless_FF13:**
   - Ensure your PC network is connected to the Rakwireless_FF13 network.

### 2. SSH Connection to Gateway

Use SSH to connect to the gateway:

```bash
ssh pi@192.168.230.1

#Default IP : 192.168.230.1
# Default Username: pi
# Default Password: raspberry 

```

### 3. Gateway Configuration

1. **Gateway Configuration:**
   - Once connected, access the Rak Gateway shell:

   ```bash
   sudo gateway-config
   ```
2. **Configure WiFi:**
   - Enable Client Mode/Disable AP Mode.
   - Add your WiFi SSID using "Add New SSID for Client."
   - Restart the gateway.

### 4. Connect to Servers

1. **ChirpStack**
   - Navigate to "Setup RAK Gateway Channel Plan".
   - Select ChirpStack as the preferred server.
   - Choose the desired Server Channel-plan frequency (e.g., Europe).
   - Find the connected IP of the gateway.
   - Access ChirpStack via the browser:
   ```bash
   Browser Address: "Gateway IP Address:8080"
   (e.g., http://192.168.61.237:8080)
   #Default Username: admin
   #Default Password: admin
   ```
   - Your gateway will automatically connect. Check the status in the ChirpStack Options (Gateways).

2. **The Things Network (TTN)**
   - Navigate to "Setup RAK Gateway Channel Plan".
   - Select TTN as the preferred server.
   - Choose the desired Server Channel-plan frequency (e.g., Europe).
   - Open TTN, sign in or sign up, and choose "Console."
   ```bash
   #Click Profile -> Console to get inside the gateway and application.
   ```
   - Choose the Network Cluster matching your gateway settings.
   - Click on the Gateway, select "Register Gateway," and enter the Gateway EUI obtained from the Gateway Shell.
   - Download the Global Configuration from TTN.
   - Paste the configuration code into the "Edit packet-forwarder config" in the Gateway Shell, updating the Gateway Server address.
   - Save and close the configuration.
   - Reload the TTN page to check the connection status.

```bash
#Feel free to customize the formatting or add any additional information you find relevant.
```









