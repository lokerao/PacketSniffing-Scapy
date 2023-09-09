# Network Packet Sniffer with Scapy

The Python script uses the Scapy library to sniff packets on a specified network interface and extract information related to HTTP requests, including URLs and potential login information. This can be useful for network monitoring and security analysis.

## Operating Systems

- [Windows](Windows)
- [Linux](Linux)

## Dependencies

Before using this script, ensure that you have the following dependencies installed:

- Python 3.x
- Scapy library (`scapy`)
  You can install Scapy using pip:

  ```bash
  pip install scapy
  
## Usage

 1. Clone this repository or download the Python script (**Packet sniffer.py**) to your local machine.

 2. Open a terminal and navigate to the directory containing **Packet sniffer.py**.

 3. Run the script with superuser privileges, specifying the network interface you want to sniff on. For example:

    ```bash
    sudo python Packet sniffer.py eth0
    
 4. Replace eth0 with the name of your network interface.

# Windows

## Packet Capture and Analysis with Scapy and Wireshark 

This explains how to capture and analyze network packets on a Windows system using a Python script with Scapy and Wireshark.

## Prerequisites

Before you begin, ensure you have the following dependencies installed on your Windows system:

1. **Python and Pip**: You can download Python for Windows from the [official website](https://www.python.org/downloads/windows/). Ensure you select the option to add Python to PATH during installation. After installation, open a command prompt and verify Python is installed:

     ```bash
     python --version
   
  To install Pip, download the [get-pip.py](https://bootstrap.pypa.io/get-pip.py) script and run it:
  
       python get-pip.py
     
2. **Scapy**: Open a command prompt and install Scapy using Pip:

   ```bash
   pip install scapy

3. **Wireshark**: Download and install Wireshark from the [official website](https://www.wireshark.org/download.html).


## Usage


1. **Clone the Repository**: Clone the repository containing your Python script to your local machine.

2. **Open Wireshark**: Launch Wireshark from the Start menu or desktop shortcut.

3. **Capture Packets in Wireshark**:
- Select the network interface you want to capture packets from.
- Click the "Start" button (usually a green shark fin icon) to begin capturing packets.

4. **Run the Python Script**: Open a command prompt, navigate to the directory containing your Python script (`sniffer.py`), and run the script with administrator privileges, specifying the network interface:

   ```bash
   python sniffer.py INTERFACE_NAME
   
Replace `INTERFACE_NAME` with the name of the network interface you want to capture packets from (in this case `eth0`).

5. **Expected Output**: The Python script will capture packets and print HTTP URLs along with possible username/password combinations to the terminal.

    ```bash
    Exmaple:
       HTTP url >>www.example.com/login
      [*] Possible username/password ->username=admin&password=123456

6. **Analyze Captured Packets**: Wireshark will display captured packets in real-time. You can filter, search, and analyze packets using Wireshark's features.


# Linux


## Packet Capture and Analysis with Scapy and Wireshark (Linux)

This explains how to capture and analyze network packets on a Linux system using a Python script with Scapy and Wireshark.

## Prerequisites

Before you begin, ensure you have the following dependencies installed on your Linux system:


1. **Python and Pip**: Most Linux distributions come with Python pre-installed. To check, open a terminal and run:

    ```bash
   python3 --version

  Install Python 3 and Pip if they are not already installed:

        sudo apt-get update
        sudo apt-get install python3 python3-pip

2. **Scapy**: Install Scapy using Pip:
   
    ```bash
    pip3 install scapy
    

3. **Wireshark**: Install Wireshark from your distribution's package manager. For example, on Debian-based systems:

    ```bash
   sudo apt-get install wireshark
    

## Usage

1. **Clone the Repository**: Clone the repository containing your Python script to your local machine:

     ```bash
     git clone https://github.com/lokerao/PacketSniffing-Scapy.git
 (or)
  
  Download **Packet sniffer.py** from the repo.


2. **Open Wireshark**: Launch Wireshark from your applications menu or by running:

    ```bash
   wireshark
    
    
3. **Capture Packets in Wireshark**:
- Select the network interface you want to capture packets from (e.g., "eth0") in the Wireshark GUI.
- Click the "Start" button (usually a green shark fin icon) to begin capturing packets.
  

4. **Run the Python Script**: Open a terminal, navigate to the directory containing your Python script (`sniffer.py`), and run it with superuser privileges, specifying the network interface:

    ```bash
    sudo python3 Packet sniffer.py eth0
    
Replace `eth0` with the actual name of the network interface you want to capture packets from.


5. **Expected Output**: The Python script will capture packets and print HTTP URLs along with possible username/password combinations to the terminal.

   ```bash
    Exmaple:
       HTTP url >>www.example.com/login
      [*] Possible username/password ->username=admin&password=123456

6. **Analyze Captured Packets**: Wireshark will display captured packets in real-time. You can filter, search, and analyze packets using Wireshark's features.


## Customization

   You can customize the script by modifying the process_sniffed_packet function to extract other information from captured packets or by adding additional logic 
   to suit your specific needs.
   

## Disclaimer

   Please note that packet sniffing may be subject to legal restrictions in some jurisdictions. Ensure that you have the necessary permissions and comply with 
   applicable laws and regulations when capturing and analyzing network traffic.

Happy Packet Analysis!




