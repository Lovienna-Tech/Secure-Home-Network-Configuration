# Secure-Home-Network-Configuration Cisco Packet Tracer

## Project Overview
This project demonstrates the configuration and security of a simulated home network using Cisco Packet Tracer. The network consists of wired and wireless end devices, a wireless router, a cable modem and a coaxial splitter. The project focuses on establishing network connectivity, configuring automatic IP address allocation through DHCP, implementing wireless security controls and verifying network functionality. This project was completed as part of my Cisco Networking Basics training to develop practical skills in IT support, networking and cybersecurity.

## Project Objectives
- Establish wired and wireless connectivity within a simulated home network.
- Configure automatic IPv4 address allocation using DHCP.
- Identify and access the wireless router's management interface using the default gateway.
- Improve router security by changing default administrative credentials.
- Configure a wireless network using a custom SSID.
- Implement WPA2-Personal authentication and encryption.
- Verify network connectivity by testing access to a simulated external web server.
- Document network configurations and provide screenshots as technical evidence.

## Tools and Technologies
- Cisco Packet Tracer
- IPv4 addressing
- Dynamic Host Configuration Protocol (DHCP)
- Wireless Local Area Network (WLAN)
- Ethernet and coaxial cabling
- WPA2-Personal
- Router Graphical User Interface (GUI)

## Technical Skills Demonstrated
- Network topology interpretation
- Wired and wireless network configuration
- Dynamic IP address allocation
- Default gateway identification
- Router administration
- Wireless authentication and encryption
- Basic router hardening
- Network connectivity testing
- Technical documentation

## Network Topology

The network topology illustrates how wired and wireless end devices connect through a central wireless router and cable modem.
The network includes:
- A coaxial splitter
- A cable modem
- A wireless router
- Two wired desktop computers
- A wireless laptop
- A television

![Final Network Topology](Screenshot16_Final_Topology.png)

*Figure 1: Completed home network topology in Cisco Packet Tracer.*

## Network Configuration

### Part 1: Physical Network Connections

#### Step 1: Connecting Coaxial Cables

In this simulated home network, internet and television services are delivered through a coaxial cable. A coaxial splitter distributes the incoming cable signal to the cable modem and television.

**Configuration:**

- Connected the cable splitter (Coaxial1) to the cable modem (Port 0).
- Connected the cable splitter (Coaxial2) to the television (Port 0).

![Coaxial Connections](Screenshot1_coaxial-connections.png)

**Purpose:**

The cable modem provides the connection between the home network and the simulated internet service provider (ISP), while the television receives the television signal.

**Verification:**

Powered on the television and confirmed that a television programme was displayed, verifying the simulated television connection.

![Television Connectivity](Screenshot2_TV_on.png)

#### Step 2: Establishing Wired Network Connections

Ethernet cables were used to establish physical connections between the cable modem, wireless router and desktop computers.

**Configuration:**

- Connected the cable modem to the Internet (WAN) port of the wireless router.
- Connected the Office PC to a LAN port on the wireless router.
- Connected the Bedroom PC to a LAN port on the wireless router.

**Purpose:**

The WAN connection enables the wireless router to communicate with the simulated internet service provider through the cable modem.

The LAN connections allow the desktop computers to communicate within the local network and access external network services through the router.

**Evidence:**

![Wired Network Connectivity](Screenshot3_Wired_Connections.png)
*Physical Ethernet connections between the network devices.*

### Part 2: Wireless Router Configuration

#### Step 1: Configuring IPv4 Addressing and Accessing the Router

The Office PC was configured to obtain its network settings automatically using Dynamic Host Configuration Protocol (DHCP).

**Configuration:**

- Opened the Office PC in Cisco Packet Tracer.
- Navigated to Desktop > IP Configuration.
- Selected DHCP to obtain IPv4 configuration automatically.
- Identified the default gateway address from the assigned network settings.

![Office PC IP Configuration](Screenshot4_Office_PC_IP_Config.png)

**Purpose:**

DHCP simplifies network administration by automatically assigning network settings, reducing the need for manual configuration and minimising configuration errors.

The default gateway enables devices on the local network to communicate with external networks.

**Accessing the Router:**

- Opened the web browser on the Office PC.
- Entered the default gateway address into the address bar.
- Accessed the wireless router's management interface using the default administrative credentials provided for the simulation.


![Router Management Interface](Screenshot5_Router_Login_GUI.png)

**Verification:**

Successfully obtained IPv4 configuration and accessed the router's management interface.

#### Step 2: Securing Administrative Access and Reviewing DHCP Settings

Default administrative credentials can present a security risk because they may be publicly known and could allow unauthorised access to network infrastructure.

**Configuration:**

- Accessed the wireless router's management interface.
- Reviewed the existing DHCP settings.
- Changed the default administrator password.
- Saved the updated configuration.

**Purpose:**

Changing the default administrator password is a basic router hardening measure that helps protect the management interface against unauthorised access.

Reviewing the DHCP settings helps ensure that connected devices can automatically obtain the network configuration required for communication.

**Evidence:**

![Router Security and DHCP Configuration](Screenshot6_DHCP_Setting_Password_Change_Success.png)

**Security Considerations:**

Unauthorised administrative access could allow an attacker to modify network settings, change wireless security configurations or disrupt network availability.

In a real-world environment, administrative access should be restricted to authorised individuals and protected using strong, unique credentials.

#### Step 3: Configuring the Wireless Network

The wireless router was configured to provide wireless connectivity to compatible end devices within the home network.

**Configuration:**

- Navigated to the wireless settings within the router's management interface.
- Enabled the 2.4 GHz wireless network.
- Configured the Service Set Identifier (SSID) as MyHome.
- Saved the wireless configuration.

**Purpose:**

The SSID identifies the wireless network and allows users to distinguish it from other available wireless networks.

The 2.4 GHz frequency band provides wireless connectivity and generally offers greater coverage than higher frequency bands, although it can be more susceptible to interference.

**Evidence:**

![Wireless SSID Configuration](Screenshot7_SSID_Wireless.png)

**Security Considerations:**

Configuring a custom SSID helps identify the intended wireless network. However, an SSID alone does not prevent unauthorised access.

Wireless authentication and encryption must be configured separately to protect the network.

#### Step 4: Implementing Wireless Security

Wireless security was configured to protect the home network against unauthorised access and protect data transmitted over the wireless connection.

**Configuration:**

- Navigated to the wireless security settings.
- Selected WPA2-Personal as the wireless security mode.
- Configured a pre-shared key (PSK).
- Saved the wireless security configuration.

**Purpose:**

WPA2-Personal uses a shared passphrase for wireless authentication and provides encryption to protect wireless communications.

Devices must possess the correct passphrase to successfully authenticate to the wireless network.

**Evidence:**

![WPA2-Personal Wireless Security](Screenshot8_WPA2_Personal_Wireless_Security.png)

**Security Considerations:**

An unsecured wireless network could expose the network to unauthorised access, misuse of network resources and interception of unprotected communications.

Although WPA2-Personal is suitable for many home networks, its reliance on a shared passphrase limits individual access management and accountability.

In an enterprise environment, WPA2-Enterprise or WPA3-Enterprise with 802.1X authentication can provide individual authentication and more granular access management.


### Part 3: Client Device Configuration and Connectivity

#### Step 1: Connecting the Wireless Laptop

The laptop was configured to connect to the secured wireless network using the SSID and authentication credentials established during the wireless router configuration.

**Configuration:**

- Opened the laptop in Cisco Packet Tracer.
- Navigated to Desktop > PC Wireless.
- Located the available wireless network with the SSID MyHome.

![Available Wireless Network](Screenshot9_Connect_Laptop_To_Network.png)

- Selected the wireless network.
- Entered the configured WPA2-Personal pre-shared key.

![Wireless Authentication](Screenshot10_Pre_shared_Key.png)

- Established a successful connection to the wireless access point.

![Successful Wireless Connection](Screenshot11_Connected_To_Assess_Point.png)

**Purpose:**

This configuration enables the laptop to communicate wirelessly with the local network without requiring a physical Ethernet connection.

**Verification:**

Confirmed that the laptop successfully connected to the wireless access point using the configured security credentials.

**Security Considerations:**

Wireless authentication helps restrict network access to devices possessing the correct credentials. However, shared passphrases do not provide individual user accountability and should be managed securely.

#### Step 2: Verifying Wireless Laptop Connectivity

Following successful wireless authentication, a connectivity test was performed to verify that the laptop could access external network services within the simulated environment.

**Testing Procedure:**

- Opened the laptop in Cisco Packet Tracer.
- Navigated to Desktop > Web Browser.
- Entered Skillsforall.srv into the address bar.
- Confirmed that the simulated webpage loaded successfully.

**Purpose:**

This test verifies that the wireless laptop can communicate with a simulated external web server through the configured network infrastructure.

**Expected Result:**

The simulated webpage should load successfully.

**Actual Result:**

The webpage loaded successfully, confirming connectivity to the simulated web server.

**Test Status:** PASS

**Evidence:**

![Laptop Connectivity Test](Screenshot12_Laptop_Internet_Connectivity.png)

#### Step 3: Verifying Office PC Connectivity

A connectivity test was performed on the Office PC to verify that the wired Ethernet connection and DHCP configuration supported access to external network services within the simulated environment.

**Testing Procedure:**

- Opened the Office PC in Cisco Packet Tracer.
- Navigated to Desktop > Web Browser.
- Entered Skillsforall.srv into the address bar.
- Confirmed that the simulated webpage loaded successfully.

**Purpose:**

This test verifies that the Office PC can communicate with a simulated external web server through its wired network connection.

**Expected Result:**

The simulated webpage should load successfully.

**Actual Result:**

The webpage loaded successfully, confirming connectivity to the simulated web server.

**Test Status:** PASS

**Evidence:**

![Office PC Connectivity Test](Screenshot13_OfficePC_Internet_Connectivity.png)


#### Step 4: Configuring the Bedroom PC

The Bedroom PC was configured to obtain its IPv4 network settings automatically through DHCP.

**Configuration:**

- Opened the Bedroom PC in Cisco Packet Tracer.
- Navigated to Desktop > IP Configuration.
- Selected DHCP.
- Confirmed that IPv4 network settings were assigned automatically.

**Purpose:**

Using DHCP allows additional devices to join the network without requiring manual IP address configuration. This simplifies network administration and reduces the risk of configuration errors.

**Evidence:**

![Bedroom PC DHCP Configuration](Screenshot14_BedroomPC_DHCP.png)

#### Step 5: Verifying Bedroom PC Connectivity

A connectivity test was performed to verify that the Bedroom PC could access external network services through its wired Ethernet connection.

**Testing Procedure:**

- Opened the Bedroom PC in Cisco Packet Tracer.
- Navigated to Desktop > Web Browser.
- Entered Skillsforall.srv into the address bar.
- Confirmed that the simulated webpage loaded successfully.

**Expected Result:**

The simulated webpage should load successfully.

**Actual Result:**

The webpage loaded successfully, confirming connectivity to the simulated web server.

**Test Status:** PASS

**Evidence:**

![Bedroom PC Connectivity Test](Screenshot15_BedroomPC_Internet_Connectivity.png)

## Security Implementation Summary

Security controls were implemented to reduce the risk of unauthorised access to the simulated home network and its administrative interface.

| Identified Risk | Security Control Implemented | Control Type | Expected Security Benefit |
|---|---|---|---|
| Unauthorised access to router administration | Changed the default administrator password | Preventative | Reduces the risk of unauthorised configuration changes |
| Unauthorised wireless network access | WPA2-Personal authentication | Preventative | Restricts wireless access to devices possessing valid credentials |
| Interception of wireless communications | WPA2 encryption | Preventative | Protects data transmitted over the wireless connection |

### Security Limitations

Although the implemented controls improve the security of the home network, some limitations remain:

- WPA2-Personal relies on a shared passphrase rather than individual user identities.
- Shared credentials limit individual accountability.
- Individual wireless access cannot be easily revoked without changing the shared passphrase.
- Network segmentation and guest network isolation were not implemented.

### Recommended Security Improvements

In a real-world environment, additional security measures could include:

- Regular router firmware updates.
- Strong and unique administrative credentials.
- WPA3 security where supported.
- Guest network isolation.
- Individual authentication using 802.1X in enterprise environments.

These recommendations were identified as potential improvements and were not implemented as part of this simulation.


















