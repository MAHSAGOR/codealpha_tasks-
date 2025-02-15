# Network Sniffer - CodeAlpha Internship Task

Welcome to the repository for my **Network Sniffer** project, developed as part of the **CodeAlpha Internship**! This project is a simple yet powerful network sniffer built using Python. It captures and analyzes Ethernet frames from network traffic, providing details such as source and destination MAC addresses and the protocol used. This tool is ideal for learning about network protocols, packet analysis, and cybersecurity fundamentals.

---

## Features

- **Ethernet Frame Capture**: Captures raw Ethernet frames from network traffic.
- **MAC Address Extraction**: Extracts and displays source and destination MAC addresses in a human-readable format.
- **Protocol Identification**: Identifies the protocol used in the captured Ethernet frame.
- **Raw Data Analysis**: Provides raw packet data for further analysis or debugging.
- **Real-Time Monitoring**: Continuously listens for and displays incoming network packets.

---

## Technologies Used

- **Python**: The core programming language used for the project.
- **Socket Programming**: For capturing raw network packets.
- **Struct Module**: For unpacking binary data from Ethernet frames.
- **Textwrap Module**: For formatting and displaying data in a readable manner.

---

## How It Works

1. **Socket Initialization**: The program creates a raw socket to capture packets at the Ethernet frame level.
2. **Packet Capture**: It listens for incoming packets and captures their raw data.
3. **Ethernet Frame Parsing**: The captured data is parsed to extract the destination MAC address, source MAC address, and protocol.
4. **Output Display**: The extracted information is displayed in a user-friendly format.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/network-sniffer.git
   ```
2. Navigate to the project directory:
   ```bash
   cd network-sniffer
   ```
3. Run the script (requires administrative privileges):
   ```bash
   sudo python network_sniffer.py
   ```
4. The program will start capturing and displaying Ethernet frames in real-time.

---

## Code Explanation

- **ethernet_frame(data)**: Parses the Ethernet frame to extract the destination MAC address, source MAC address, and protocol.
- **get_mac_addr(bytes_addr)**: Converts a byte-formatted MAC address into a human-readable string.
- **main()**: Initializes the socket, captures packets, and displays the extracted information.

---

## Example Output

```
Listening for network packets...

Ethernet Frame:
  Destination: 00:1A:2B:3C:4D:5E, Source: 00:5E:4D:3C:2B:1A, Protocol: 2048
```

---

## Use Cases

- **Network Analysis**: Understand network traffic patterns and protocols.
- **Cybersecurity Education**: Learn about packet-level data and network vulnerabilities.
- **Debugging**: Analyze network issues by inspecting raw packet data.

---

## Limitations

- **Basic Functionality**: Currently, the sniffer only captures Ethernet frames and does not decode higher-level protocols (e.g., IP, TCP, UDP).
- **Platform Dependency**: Requires administrative privileges and may not work on all operating systems.
- **No Filtering**: Captures all packets without filtering, which may result in a large amount of data.

---

## Future Improvements

- **Protocol Decoding**: Add support for decoding IP, TCP, UDP, and other higher-level protocols.
- **Packet Filtering**: Implement filtering to capture only specific types of traffic (e.g., HTTP, DNS).
- **GUI**: Develop a graphical user interface for easier interaction and visualization.
- **Logging**: Save captured packets to a file for later analysis.

---

## Contributions

This project is open for contributions! If you'd like to improve the sniffer, add new features, or fix bugs, feel free to fork the repository and submit a pull request. Some areas where contributions are welcome include:
- Adding support for more protocols.
- Implementing packet filtering.
- Enhancing the user interface.

---

Thank you for checking out my **Network Sniffer** project! If you have any questions, suggestions, or feedback, feel free to reach out. Let's explore the world of network traffic together! 😊
