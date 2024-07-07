

# Network Monitoring System

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Network Monitoring System is a comprehensive tool designed to monitor network traffic, scan devices and ports within a network, and capture network packets. The system provides real-time statistics and historical data on network bandwidth usage, identifies active devices and open ports, and captures and displays network packets for detailed analysis. It is built using Python and Flask, leveraging libraries such as `psutil` and `scapy`.

## Features

- **Bandwidth Usage Monitoring**
  - Monitor network bandwidth usage in real-time.
  - Historical data visualization of network usage over time.
  - User interface for selecting specific network interfaces for monitoring.

- **Network Scanning**
  - Scan specified IP ranges for active devices.
  - Identify and list IP and MAC addresses of active devices.
  - Scan and list open ports on identified devices.
  - User interface for inputting IP ranges for scanning.

- **Packet Capturing**
  - Capture network packets on specified interfaces.
  - Filter captured packets by specified IP ranges.
  - Display detailed information about each captured packet.
  - User interface to start and stop packet capturing.

## Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Steps

1. Clone the repository:

```bash
git clone https://github.com/yourusername/network-monitoring-system.git
cd network-monitoring-system
```

2. Create and activate a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Set up the database (if applicable):

```bash
flask db upgrade
```

5. Run the application:

```bash
flask run
```

The application should now be running on `http://127.0.0.1:5000/`.

## Usage

### Bandwidth Usage Monitoring

1. Access the dashboard at `http://127.0.0.1:5000/`.
2. Select the network interface you want to monitor.
3. View real-time and historical bandwidth usage statistics.

### Network Scanning

1. Navigate to the Network Scanning section.
2. Input the IP range you want to scan.
3. View the list of active devices and open ports.

### Packet Capturing

1. Navigate to the Packet Capturing section.
2. Select the network interface and IP range for capturing.
3. Start and stop packet capturing as needed.
4. View detailed information about captured packets.

## Configuration

### Environment Variables

You can configure the application using environment variables. Create a `.env` file in the root directory and add the following variables:

```env
FLASK_APP=app
FLASK_ENV=development
DATABASE_URL=sqlite:///db.sqlite3
```

### Customizing the Dashboard

You can customize the dashboard layout and features by modifying the templates in the `templates` directory and the static files in the `static` directory.

## Contributing

We welcome contributions from the community! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes and commit them with clear and concise messages.
4. Push your changes to your fork.
5. Open a pull request to the main repository.

Please ensure your code follows the existing coding style and includes tests where applicable.

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](LICENSE) file for more details.

 
