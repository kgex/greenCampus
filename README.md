# Green Campus

A short description of your project goes here.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Configuration](#configuration)
4. [Contributing](#contributing)
5. [License](#license)

## Installation

1. Clone the repository: `git clone https://github.com/yourusername/yourproject.git`
2. Install dependencies: `npm install`
3. Additional steps, if any...

## Usage

```bash
$ command-to-run-your-project arg1 arg2

### 5. Configuration:

If your project requires configuration, provide details on how users can configure it. Include information about configuration files and environment variables.

```markdown
## Configuration Guide: Setting up Rak PiHat Firmware and ChirpStack Connection

### 1. Initial Setup

1. **Download Firmware:**
   - Download the Rak PiHat firmware from [here](https://drive.google.com/file/d/1MoqZ3JeULfrjy7yOFgUPQUoxvpd3ceYY/view?usp=sharing).

2. **Connect to Rakwireless_FF13:**
   - Connect your PC network to the Rakwireless_FF13 network.

### 2. SSH Connection to Gateway

Use the following commands to connect to the gateway via SSH:

```bash
ssh pi@192.168.230.1
# Default Username: pi
# Default Password: raspberry
## Configuration

1. Open the `config.yml` file.
2. Modify the following settings:

```yaml
api_key: YOUR_API_KEY
debug_mode: true


### 6. Contributing:

Encourage others to contribute to your project. Include guidelines for submitting issues or pull requests.

```markdown
## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Make your changes and commit: `git commit -m 'Add feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
