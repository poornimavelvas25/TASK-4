# INTERVIEW QUESTIONS
## What is a Firewall?

A firewall is a network security system that monitors and controls incoming and outgoing traffic based on predefined security rules.

It acts as a barrier between a trusted internal network and an untrusted external network (like the internet).

Example:

In Windows → Windows Defender Firewall

In Linux → UFW, iptables

Firewalls prevent unauthorized access while allowing legitimate communication.

## Difference Between Stateful and Stateless Firewall
In Stateless Firewall
-Checks each packet individually
-Does NOT remember past packets
-Basic Security
-Example :-Simple packet filter

In stateful Firewall
-Tracks full connection state
-Remembers active sessions
-More Secure Security
-Modern enterprise firewalls

## What Are Inbound and Outbound Rules?

Inbound Rules

Control incoming traffic from external sources into your system.

Example:

Blocking port 23 prevents remote Telnet access.

Outbound Rules

Control traffic leaving your system to external networks.

## How Does UFW Simplify Firewall Management?

UFW (Uncomplicated Firewall) is a simplified interface for managing Linux firewalls.

Instead of writing complex iptables rules, you can use simple commands like:

sudo ufw allow 22
sudo ufw deny 23
Why UFW is simple:

Easy syntax

Human-readable commands

Less configuration errors

Quick enable/disable

## Why Block Port 23 (Telnet)?

Port 23 is used by Telnet protocol.

Telnet:

Sends data in plain text

No encryption

Easily intercepted by attackers

Because of this, Telnet is considered insecure.

Instead, secure protocol like SSH (Port 22) is preferred.

Blocking port 23 prevents:

Unauthorized remote login

Credential theft

Packet sniffing attacks

## Common Firewall Mistakes

Leaving unnecessary ports open

Not updating firewall rules

Misconfigured allow rules

Disabling firewall temporarily and forgetting to enable it

Not logging firewall activity

Allowing “Any” IP access

## How Does a Firewall Improve Network Security?

A firewall improves security by:

Blocking unauthorized access

Controlling network traffic

Preventing port scanning attacks

Reducing malware communication

Protecting internal services

## What is NAT in Firewalls?

NAT stands for Network Address Translation.

NAT:

Converts private IP addresses into public IP addresses

Hides internal network structure

Allows multiple devices to share one public IP

Example:

Your home router uses NAT to allow many devices to access the internet using one public IP address.
