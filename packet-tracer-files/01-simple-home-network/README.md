# Lab 01 - Create a Simple Home Network

## Overview

This lab introduces the fundamentals of building a small enterprise network using Cisco Packet Tracer.

The objective is to deploy end devices, connect them to a wireless router and cable modem, obtain IP addresses through DHCP, and verify network connectivity.

---

# Objectives

After completing this lab, you will be able to:

- Build a basic network topology
- Connect network devices using the correct cable types
- Configure end devices to obtain IP addresses automatically
- Connect a wireless client to a WLAN
- Verify network connectivity using Ping
- Inspect DHCP configuration using ipconfig

---

# Skills Learned

- Network Topology Design
- Ethernet Cabling
- DHCP
- IPv4 Addressing
- Wireless Networking
- Basic Connectivity Testing
- Packet Tracer Navigation

---

# Devices Used

| Device | Quantity |
|---------|----------|
| PC | 1 |
| Laptop | 1 |
| Wireless Router | 1 |
| Cable Modem | 1 |
| Internet Cloud | 1 |

---

# Network Topology

Insert image below.

```

![Topology](images/topology.png)

```

---

# Step 1 - Add Devices

Add the following devices.

- PC
- Laptop
- Wireless Router
- Cable Modem
- Internet Cloud

Rename them as:

- PC
- Laptop
- Wireless Router
- Cable Modem

---

# Step 2 - Connect Devices

Use the following cables.

| From | To | Cable |
|-------|----|-------|
| PC FastEthernet0 | Router Ethernet1 | Copper Straight-through |
| Router Internet | Cable Modem Port1 | Copper Straight-through |
| Cable Modem Port0 | Internet Cloud Coaxial7 | Coaxial |

---

# Step 3 - Configure PC

Navigate to

Desktop
→ IP Configuration

Verify

- DHCP Enabled
- IPv4 Address Assigned

Open Command Prompt

Run

```
ipconfig /all
```

Verify

- IPv4 Address
- Subnet Mask
- Default Gateway

---

# Step 4 - Verify Connectivity

Run

```
ping cisco.srv
```

Expected result

```
Reply from...
Reply from...
Reply from...
Reply from...
```

---

# Step 5 - Configure Laptop

Navigate to

Physical

Power Off

Remove

Ethernet Module

Install

Wireless WPC300N

Power On

---

# Step 6 - Connect to WiFi

Desktop

PC Wireless

Refresh

Select

HomeNetwork

Connect

---

# Step 7 - Test Connectivity

Open

Web Browser

Browse to

```
cisco.srv
```

The Cisco webpage should load successfully.

---

# Verification

## PC

| Item | Result |
|-------|--------|
| DHCP | Pass |
| Ping | Pass |
| Browser | Pass |

## Laptop

| Item | Result |
|-------|--------|
| Wireless Connected | Pass |
| Browser | Pass |

---

# IP Address Table

| Device | IPv4 Address | Subnet Mask | Gateway |
|---------|-------------|-------------|----------|
| PC | | | |
| Laptop | | | |

---

# Key Concepts

### DHCP

Automatically assigns IP addresses to network devices.

### Default Gateway

Allows devices to communicate outside the local network.

### Subnet Mask

Separates the network portion from the host portion of an IP address.

### Ping

Tests communication between devices.

---

# Conclusion

This lab demonstrated the deployment of a simple wired and wireless network using Cisco Packet Tracer. The network successfully provided IP addressing through DHCP and allowed end devices to communicate with external resources.
