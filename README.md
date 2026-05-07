# Sophos-installation-guide
Step-by-step Sophos installation-guide
## Description
This project documents the deployment and configuration of sophos firewall to secure a corporate network. It covers initial setup, network configuration, firewall rules, and basic security policies to protect internal resources from external threats.
## Features
- Cleanup and reorganization of network rack for improved cable management and optimal connectivity
- Removal of unused/obsolete network devices and cabling
- Successful claiming and integration of the firewall with existing Sophos Central account (both sites now centrally managed)
- Integration of Mainone as the primary ISP 
- Configuration of firewall rules and policies to allow controlled internet access and restrict non-ethical websites
- Deployment and configuration of captive portal for user authentication
- Verification of printer connectivity across the network
- Confirmation that all access point and printers are properly connected via the switch linked to the firewall
Assignment of static IP address to CCTV DVR and MAC address binding for consistent and secure access
- Installation of Sophos client authenticators and demonstration to admin for user deployment
- Demonstration of Sophos Central 30-day trial Endpoint protection,including agent download and installation
- Configuration of firewall rule to exempt management TVs from Captive portal authentication
- Assignment and enforcement of user-based policies based on roles and access privileges
- Configuration of web filtering,application control and additional security policies 
Network optimization for improved performance and secure usage
## Getting started
PRE-DEPLOYMENT PLANNING
- Assessing current network topology(ISP links, switches, Aps, endpoints)
- Taking note of IP scheme, VLANs and critical devices(printers, DVR,TVs)
- Backing up existing configurations
- Scheduling deployment window to minimize downtime
PHYSICAL SETUP & RACK OPTIMIZATION
- Powering down non-critical devices
- Cleaning up the network rack (Remove unused cables and obsolete devices and labelling all active cables properly)
- Mounting the Sophos firewall in the rack
- Connecting WAN(Mainone) ~> WAN Port
- LAN ~> Core Switch
- Powering on all devices
INITIAL FIREWALL ACCESS & SETUP
- Connecting laptop to firewall LAN Port
- Accessing default IP
- Running initial setup wizard
ISP CONFIGURATION(MainOne as Primary)
- Configuring WAN interface with MainOne details
- Setting gateway and DNS
- Testing Internet connectivity(ping)
FIREWALL RULES & INTERNET ACCESS
- Go to rules and policies>firewall rules
- Applying Security controls
- Blocking non-ethical and unwanted categories
CAPTIVE PORTAL CONFIGURATION
- Navigate to Authentication>captive portal
- Creating a captive portal policy
- Configuring authentication method
- Applying captive portal to firewall rule
- Testing login with a sample user
USER & POLICY MANAGEMENT
- Creating user group
- Assigning policies based on roles
- Enforcing user based firewall rules
DEVICE CONNECTIVITY VERFICATION
- Confirming all switches are connected to firewall LAN
- Checking access points
- Testing printer connectivity
STATIC IP & MAC BINDING(CCTV DVR)
- Go to network>DHCP
- Add static lease
- Testing DVR accessibility via assigned IP
SOPHOS CLIENT AUTHENTICATOR DEPLOYMENT
- Installing on user systems
- Demonstrating login process to admin
- Confirming users can authenticate without captive portal interruption
ENDPOINT PROTECTION TRIAL SETUP
- ACTIVATING 30-day endpoint protection trail
- Downloading endpoint agents
- Installing on selected systems
- Verifying endpoints shown in dashboard
EXCEPTION RULE FOR MANAGEMENT
- Identifying TV/Printer addresses
- Placing rule above captive portal rule
- Testing TV/Printer internet access
ADVANCED SECURITY CONFIGURATION
- Configuring web filtering,application control policies,intrusion prevention system(IPS)
- Applying policies to appropriate user groups
NETWORK OPTIMIZATION
- Enabling traffic shaping(QoS)
- Monitoring bandwidth usage
- Adjusting firewall rules for performance
- Running speed and latency tests
FINAL TESTING & VALIDATION
Testing internet access, captive portal, printer and CCTV access
DOCUMENTATION & HANDOVER
- IP allocations,Network diagram, firewall rules
- Sharing credentials securely
