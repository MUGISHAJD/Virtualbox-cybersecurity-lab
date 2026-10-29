# VirtualBox Cybersecurity Lab: Kali Linux, Windows 10 & Android 9x

## 1. Project Overview

This project focuses on building a virtual cybersecurity testing lab using Oracle VirtualBox. The lab consists of multiple virtual machines (Kali Linux, Windows 10 and Android 9x) configured to support practical learning in cybersecurity, networking, and ethical hacking.

Kali Linux serves as the attacking and security-testing machine, while Windows 10 and Android 9x provide additional virtual environments for network connectivity testing and future security experiments.

## 2. Project Objectives

The main objectives of this project are to:

- Install and configure Oracle VirtualBox.
- Deploy Kali Linux as the primary cybersecurity testing machine.
- Install Windows 10 and Android 9x as additional virtual machines.
- Configure a NAT Network
- Assign Kali Linux the static IP address
- Configure clipboard sharing and drag-and-drop functionality.
- Set up a shared folder between the host computer and Kali Linux.
- Test network connectivity between the virtual machines using ping.

## 3. Tools and Technologies
Oracle VirtualBox: Virtualization platform.
Kali Linux: Attacking machine and cybersecurity testing environment.
Windows 10: Additional virtual machine for connectivity testing.
Android 9x: Additional virtual machine for connectivity testing.
NAT Network: Virtual network connecting the lab machines.
Ping: A command for testing network connectivity between virtual machines.
	
## 4. Network Configuration

The lab uses a NAT Network with the 10.0.0.0/24 subnet to allow virtual machine to communicate between them and access internet. 

## i. Kali Linux Configuration (Attacking machine and cybersecurity testing environment)

The required configuration includes:

- IP address: `10.0.0.2/24`
- Network: `10.0.0.0/24`
- Internet access through the VirtualBox NAT Network
- Bidirectional clipboard sharing
- Drag-and-drop functionality
- Shared host folder access

## ii. Window 10 Configuration (virtual machine for network connectivity testing and future security exercises)

The required configuration includes:

- IP address: `10.0.0.10/24`
- Network: `10.0.0.0/24`
- Internet access through the VirtualBox NAT Network
- Bidirectional clipboard sharing
- Drag-and-drop functionality
- Shared host folder access

## iii. Android 9x Configuration (virtual machine for network connectivity testing and future security exercises)

The required configuration includes:

- IP address: `10.0.0.9/24`
- Network: `10.0.0.0/24`
- Internet access through the VirtualBox NAT Network
- Bidirectional clipboard sharing
- Drag-and-drop functionality
- Shared host folder access


## 5. Shared Folder Configuration

A folder named `downloads` on the host computer is shared with the Kali Linux virtual machine. The shared folder allows files to be exchanged between the host and guest operating systems.

Configuration requirements:

1. Create or identify the host's `downloads` folder.
2. Open the Kali Linux virtual machine settings.
3. Add the host folder under Shared Folders.
4. Enable automatic mounting if appropriate.
5. Enable permanent sharing.
6. Verify that Kali Linux can access the shared folder.


## 6. Connectivity Testing

Ping tests are used to verify whether the virtual machines can communicate over the configured network.

Example 1: Test the Windows 10 Machine from Kali Linux

ping -c 4 10.0.0.10

Example 2: Test the Android Machine from Kali Linux

ping -c 4 10.0.0.9

### Test Internet Connectivity

ping -c 4 8.8.8.8

### To test DNS resolution, run:

ping -c 4 google.com

If ping tests fail, check the IP addresses, subnet configuration, virtual network adapter settings, guest operating system support, and firewall rules. Some systems may block ICMP requests even when other network communication is working.

## 7. Evidence and Screenshots

Suggested evidence:

1. VirtualBox installation or main interface.
2. VirtualBox NAT Network configuration showing `10.0.0.0/24`.
3. Kali Linux IP address configuration.
4. Successful Kali Linux internet connectivity test.
5. Shared folder and clipboard configuration.
6. Windows 10 virtual machine running.
7. Android 9x virtual machine running.
8. Successful ping test results.
9. Virtual machine snapshots.

## 8. Learning Outcomes

Through this project, I developed practical experience in:

- Virtual machine installation and management.
- Virtual networking and NAT Network configuration.
- IPv4 addressing and subnetting.
- Basic network troubleshooting.
- Testing network connectivity using ping.
- Shared folder and clipboard configuration.
- Snapshot creation and virtual machine recovery.
- Preparing a virtual environment for cybersecurity practice.

## 9. Conclusion

This project established the foundation for a practical cybersecurity lab using VirtualBox, Kali Linux, Windows 10, and Android 9x. The lab provides an environment for learning virtualization, network configuration, connectivity testing, and basic cybersecurity concepts. It will also serve as a foundation for future hands-on security exercises.

Author: Jean De Dieu Mugisha
