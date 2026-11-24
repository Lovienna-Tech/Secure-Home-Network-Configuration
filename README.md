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

![Final Topology](Screenshot16_Final_Topology.png)

*Figure 1: Completed home network topology in Cisco Packet Tracer.*

## Network Configuration

### Part 1: Physical Network Connections

#### Step 1: Connecting Coaxial Cables

In this simulated home network, internet and television services are delivered through a coaxial cable. A coaxial splitter distributes the incoming cable signal to the cable modem and television.

**Configuration:**

- Connected the cable splitter (Coaxial1) to the cable modem (Port 0).
- Connected the cable splitter (Coaxial2) to the television (Port 0).

![Topology](Screenshot1_coaxial-connections.png)

**Purpose:**

The cable modem provides the connection between the home network and the simulated internet service provider (ISP), while the television receives the television signal.

**Verification:**

Powered on the television and confirmed that a television programme was displayed, verifying the simulated television connection.

![Topology](Screenshot2_TV_on.png)

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

![Topology](Screenshot3_Wired_Connections.png)
*Physical Ethernet connections between the network devices.*

## Part 2: Configure the Wireless Router
# Step 1: Access the Home Wireless Router GUI.
The Home wireless routers are configured using a graphical user interface (GUI) which is accessed through the computers web browsers. To accomplish this we follow the following steps.

Office PC → Desktop tab → IP Configuration → DHCP 

After clicking DHCP it automatically configured the Office PC to be on the same IP network as the Home Wireless Router. 

![Topology](Screenshot4_Office_PC_IP_Config.png)

To continue the configuration process, using the web browser I have pasted the default gateway into the browser. 

As the Home Router is newly installed I used default credientials such as 'Admin' for both the User Name and Password. The GUI for the Home Wireless Router appeared ready to continue configuring the network. 

![Topology](Screenshot5_Router_Login_GUI.png)

# Step 2: Configure Basic Settings
Now that I have accesseed the GUI I now needed to change the User name and Password from the default ones provided to my own. To do this I followed the following steps.

Administration tab → New password → Save Settings → Enter new credentials → Continue

# Step 3: Configure a wireless LAN
To connect wireless devices to the home wireless network over WIFI I enabled the 2.4 GHz network. 

Wireless tab → 2.4 GHz → Enable

I then changed the SSID from the default name to 'MyHome' so that those searching for my network can find it. I then saved these settings. 

To set up security for my network I enabled WPA2 Personal and created a PassPhrase so that my netwrok can ony be accessed by those I provided my PassPhrase to and then saved these settings. 
![Topology](Screenshot8_WPA2_Personal_Wireless_Security.png)

## Part 3: Configure IP Addressing and Test Connectivity
Now that my router is configured I configured the IP address for my home PC and Laptop to connect wirelessly to the internet. 

Laptop → Desktop tab → PC Wireless → Connect tab 

In the connect tab I entered the Passphrase in the Pre-shared Key field and clicked connect.
![Topology](Screenshot10_Pre_shared_Key.png)
![Topology](Screenshot11_Connected_To_Assess_Point.png)

To test the connectivity I opened the Web browser on the Laptop and did a search using the website 'Skillsforall.srv' and a verification appeared confirming connectivity 

![Topology](Screenshot12_Laptop_Internet_Connectivity.png)

To connect the Bedroom PC the the wireless network in enabled DHCP to recieve an IP address 
![Topology](Screenshot14_BedroomPC_DHCP.png)
To verify connectivity I did the same web browser search I did preciously for the laptop

![Topology](Screenshot15_BedroomPC_Internet_Connectivity.png)

I have now completed connecting the network devices, configured the router and wireless LAN and configure all hosts to the Home Network. 

This is my final Topology.

![Topology](Screenshot16_Final_Topology.png)

















