MAC Address Spoofing (Educational Demo)
This project is for educational purposes only. Do not use these methods for unauthorized activity.

What this is
As part of a penetration testing course, I practiced changing the MAC address of a device using Kali Linux. Spoofing a MAC address is a common step in network testing and evasion during security assessments.

Tools Used
Operating system: Kali Linux

Commands: ifconfig, sudo, ifconfig eth0 hw ether

Screenshots
The screenshots show:

The original MAC address

The process and final result after changing it

Screenshots are located in the screenshots/ folder.

Sensitive information like usernames and IP addresses has been blurred or removed.

# Check network interfaces
ifconfig

# Disable the network interface
sudo ifconfig eth0 down

# Change the MAC address
sudo ifconfig eth0 hw ether 00:11:22:33:44:55

# Enable the network interface
sudo ifconfig eth0 up

# Verify the MAC address change
ifconfig
