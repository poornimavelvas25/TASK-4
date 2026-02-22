# TASK-4

Objective

The objective of this project is to understand how a firewall filters network traffic by:

1.Viewing existing firewall rules

2.Blocking inbound traffic on a specific port (Telnet - 23)

3.Allowing SSH traffic (Port 22)

4.Testing firewall behavior

5.Restoring original configuration

#  Tools Used

1.Windows Defender Firewall

2.UFW (Linux)

3.Kali Linux

4.Nmap

5.Telnet

# How Firewall Filters Traffic 

A firewall acts as a security barrier between trusted and untrusted networks.

# It filters traffic based on:

Port numbers

Protocol (TCP/UDP)

IP address

Direction (Inbound/Outbound)

# When a rule is created:

Traffic matching the rule is either allowed or denied.

Rules are processed in order.

Deny rules override connections.

# Firewalls prevent:

Unauthorized access

Port scanning exploitation

Remote attacks

# Observations

When Port 23 was blocked, connection attempts failed.

After allowing SSH (Port 22), SSH connections were successful.

Firewall effectively filtered traffic based on defined rules.


