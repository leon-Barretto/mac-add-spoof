# MAC Address Spoofing (Educational Demo)

> **Note:** This project is for educational purposes only. Do not use these methods for unauthorized activity.

## Overview

This project demonstrates how to change (spoof) the MAC address of a device using Kali Linux. This technique is commonly used in penetration testing to help with network testing and evasion.

## Tools Used

- **Operating System:** Kali Linux  
- **Commands:** `ifconfig`, `sudo`, `ifconfig eth0 hw ether`

## Screenshots

The screenshots provided show:  
- The original MAC address  
- The process of changing the MAC address  
- The final result after the change

All screenshots are saved in the `screenshots/` folder.

> Sensitive information such as usernames and IP addresses have been blurred or removed for privacy.

## Commands

```bash
# List network interfaces and details
ifconfig

# Disable the network interface
sudo ifconfig eth0 down

# Change the MAC address to the desired value
sudo ifconfig eth0 hw ether 00:11:22:33:44:55

# Re-enable the network interface
sudo ifconfig eth0 up

# Confirm the MAC address has been changed
ifconfig
