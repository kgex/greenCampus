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
# Default Username: pi
# Default Password: raspberry

### 3.Gateway Configuration

 1. **Gateway Configuration:**
   - Once connected, access the Rak Gateway shell:
 ```bash
sudo gateway-config







