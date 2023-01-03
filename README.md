# Page 2

SUPERDOME FLEX / FLEX 280 – DEPLOYMENT RACK OPTIONS

July 2022

Confidential | For HPE Partner Only

Rev 18May21

Isidro Grau

Solution Architect

BUILDING BLOCKS AND REFERENCE CONFIGURATIONS

Product Overview

HPE SUPERDOME FLEX 280 SERVER

Scalability and performance

### •3rd generation Intel Xeon Scalable processors, gold or platinum, up to 28 cores •Modular scale

### up 5U building block, 2 or 4 sockets •“ Glueless ” modular architecture with 6 UPI links per processor for faster data rates\* •Scale from 2

### 8 sockets in 2

### socket increments, with 16

### 224 cores •Designed to provide 64GB – 24TB of shared memory; support for HPE Persistent Memory with next

gen Intel® Optane TM persistent memory

I/0 flexibility

### •Balanced I/O for extreme performance •Up to 32 PCIe 3.0 cards with choice of 16

### slot (all low profile) or 12

### slot (FH/FW) •16

### slot: each CPU has support for two x8 and two x16 PCIe cards •12

slot: each CPU has support for one x16 PCIe slot and one 300w GPU

•Up to 20 SAS/SATA/NVMe drives with RAID & HW encryption; Optional DVD

Extreme Superdome RAS

### •Advanced memory resiliency, Firmware First, analysis engine, self

healing •HPE Serviceguard for Linux •Enhanced security with Silicon Root of Trust

Simplified User Experience

•HPE Infosight AI for optimum server performance •Simplified management GUI •HPE OneView, OpenStack, Redfish API •Optional HPE GreenLake consumption model •HPE Datacenter Care, HPE Proactive Care

HPE Superdome Flex 280

### 2

### 8 socket, 5U, 4

socket modular block

SuperdomeFlex SuperdomeFlex SuperdomeFlex SuperdomeFlexCONFIDENTIAL | AUTHORIZED HPE PARTNER USE ONLY

### “ Glueless ” 4S/8S modular server designed for mission

critical workloads

HPE SUPERDOME FLEX 280 SERVER ARCHITECTURE

### • Leveraged mechanical design with 5U 4

### socket building block scales from 2S to 8S using only “ glueless ” UPI link fabric, based on the “Cedar Island” processor family from Intel • The processor, sometimes called the Cooper Lake 6 UPI or CPX6 provides 6 UPI links per processor at 10.4 GT/s data rates ( doubles the “ glueless ” fabric interconnect capacity ) • One chassis supports 2S or 4S (CPU socket population option) • Internal and external cabling routes UPI links to provide optimal interconnections between 4

### 8 processors at full data rates • 4S system (shown) uses 8 internal half

### width UPI cables for CPU cross links • 8S option uses 8 internal “Y” bulkhead cables and 8 external full

width UPI cables in “twisted hypercube” fabric for maximum performance

### • 6 independent memory channels provide slots for up to 12 DIMMs or 6 DIMM and 6 persistent memory modules • 16

### slot (shown) and 12

### slot I/O options provide up to 16 x16 slots plus 16 x8 slots or support for full

height and double width GPUs • Up to 10 2.5” form factor drives provide boot and limited data storage • New server management design includes a TPM v2.0 and even provides Silicon Root of Trust !!!

Compute

4 CPUs

112 cores

224 threads

Memory

48 DIMMs

6 TB capacity

(128 GB DIMMs)

I/O

8 (x8) slots

8 (x16) slots

10 2.5” drives

CONFIDENTIAL | AUTHORIZED HPE PARTNER USE ONLY

### 4

socket chassis

Glueless 8S server configuration

HPE SUPERDOME FLEX 280 SERVER ARCHITECTURE

• Compute: 8 CPU sockets provide up to 224 cores (448 threads) • Memory: 96 DIMM slots provide up to 12 TB capacity (using 128GB LRDIMMs) • I/O: up to 16 x16 PCIe 3.0 slots, 16 x8 PCIe slots and up to 20 2.5” drives

CONFIDENTIAL | AUTHORIZED HPE PARTNER USE ONLY

Rear EIA Rails

Front EIA Rails

Rear Door

All Racks – SD Flex / 280 Requirements –

Front EIA Rails

Rear EIA Rails

Review recessed requirements for the FLEXgrid / UPI cables

HOW MUCH ROOM IS NEEDED IN THE FRONT FOR CABLE DEPLOYMENT? 6.5 I NCHES

Image To provide proper clearance for the chassis to slide forward and backward in the rack, you must:

Disconnect the Superdome Flex Grid cables from the front of the chassis

Remove the power cables and any I/0 cables from the rear of the chassis

ACCESSING COMPONENTS – CHASSIS NEEDS TO SLIDE – BOTH DIRECTIONS

SD FLEX 280 UPI CABLES – 4 SOCKET FACTORY SHIP

No UPI Cables or Bulkhead connectors – shipped or installed

SD FLEX 280 UPI CABLES

16 UPI Cables Connections

8 UPI Cables

SD FLEX 280 UPI CABLES

SD FLEX 280 UPI CABLES

Base Chassis CPU#PortsExpansion ChassisCPU#PortsBase Chassis CPU 1UPI 1Expansion ChassisCPU 1UPI 1Base Chassis CPU 1UPI 2Expansion ChassisCPU 1UPI 2Base Chassis CPU 3UPI 3Expansion ChassisCPU 3UPI 3Base Chassis CPU 3UPI 4Expansion ChassisCPU 3UPI 4Base Chassis CPU 0UPI 5Expansion ChassisCPU 2UPI 7Base Chassis CPU 0UPI 6Expansion ChassisCPU 2UPI 8Base Chassis CPU 2UPI 7Expansion ChassisCPU 0UPI 5Base Chassis CPU 2UPI 8Expansion ChassisCPU 0UPI 6 SD FLEX 280 UPI CABLES

IMG\_3840 Find the UPI cables kitted with the build and install short cables as per the reference diagram below. Note these will go from the same port to the same port of each chassis.1 to 1, 2 to 2, 3 to 3, and 4 to 4.

Install long UPI cables as per the reference diagram above. Note these will go from the same port to the same port of each chassis. 5 to 7, 6 to 8, 7 to 5, and 8 to 6 between each chassis, see Cabling diagram above .

See photo for proper UPI cable routing between each fan assemblies.

### WRONG VS RIGHT UPI CABLING

Do not install UPI cabling – on the left

Blocks the fans and airflow

No Shocker, here – airflow BLOCKED

guess what happens –

yep you guessed it

CPUs over heat!!!

Correctly installed

Does NOT Block airflow

SD FLEX 280 – ERMC

eRMC

Connects to management network

Base Chassis Base I/O

•One RJ45 GigE management port (PEER) •One Reset switch •One RJ45 GigE eRMC port •One BMC console (mini USB-B) •Two RJ.5 Clock ports •One serial port (9-pin Dsub) •One eRMC USB port •Four external USB 3.0 ports •One VGA port (15-pin Dsub

Two 1GigE ports (LAN0 and LAN1)

SD FLEX 280 – ERMC – BASE IO – EXPANSION TRAY

Expansion Chassis BMC Tray

•One RJ45 RMC management port (PEER) •One RST Port •Two RJ.5 Clock ports

One SMC/BMC console (mini USB-B)

SD FLEX 280 – ERMC

➀Peer ports (RJ45 Cat6 cable)

➁Clock ports (RJ.5 cable)

➂eRMC network port (RJ45 Cat6 cable ) – connects to management network

Prerequisites

• 2 RJ45 Cat6 cables

• 2 RJ.5 shielded IM cables

SD FLEX 280 – ERMC

RMC PORTS

RMC Ports

Ingress RMC ports that are needed:

SSH: 22

HTTPS: 443 for Redfish and HTML5 web console, Remote Support (RS)

HTTPS: 1443 for JViewer use (if desired)

IPMI over LAN: 623

Egress RMC network ports:

NTP: 123

DNS: 53

LDAP: 389 or 636, or whatever they configure their LDAP server to listen on. Only if customer uses LDAP for RMC authentication.

HTTPS: 443. This is needed to support FW update over HTTPS, OneView control, Redfish events, Server->RS connection

SH: 22. Needed for FW update over scp/sftp

SNMP: 161, 162, or whatever they configure their SNMP trap receiver to listen on. Only if they want to use SNMP

Remote syslog: 514, or whatever they configure their Rsyslogserver to listen on. This feature is not yet available until our upcoming 2.4 release comes out.

Choice and flexibility to manage your HPE Superdome Flex deployment

OPEN MANAGEMENT FRAMEWORK SIMPLIFIES HYBRID IT ENVIRONMENTS

Open source manag ement

HPE management ecosystem

HPE OneView

HPE Insight Remote Support

HPE SUM

To learn more about HPE Superdome Flex manageability, click here

Insight Online

C:\Users\VazquezMar\AppData\Local\Microsoft\Windows\Temporary Internet Files\Content.Outlook\30RLWBQS\Dashboard\_noRSI (2).png Customer

Insight Online

HPE Global Solution Center

SIMPLIFIED MANAGEMENT EXPERIENCE ON HPE SUPERDOME FLEX

HPE Superdome Flex 280 Management

### All remote access functionality + server control + Analysis Engine for self

healing and troubleshooting.

Troubleshooting, alerts, and connectivity to HPE support

Partner

HPE Support

Firmware management

SUM

Image result for oneView HPE HPE OneView

Redfish API’s are consumed by:

•OneView •OVRS •OpenStack

Any Redfish compatible tools

Insight Remote Support

RMC

C:\Users\RALEVE\AppData\Local\Microsoft\Windows\Temporary Internet Files\Content.Outlook\N81PS3KS\Suse\_Lockup\_RGB.png SuperdomeFlex SuperdomeFlexOneView Remote

Support

HPE ONEVIEW SUPPORT FOR HPE SUPERDOME FLEX

Rack manager resource

### •Superdome Flex is monitored as rack manager (RM) •RM supports Redfish multi

node devices

Inventory support — rack manager

•Individual chassis •Rack management controller (RMC) •HPE nPar (partitions)

Health Monitoring

•Supports Redfish alerts related to fans, power supply, temperature, and chassis

HPE OneView support featuring managed mode

HPE OneView Remote Support (OVRS)

### •24x7 monitoring with pre

failure alerts •Automated case creation •Contracts’ expiration alerts

### Modular, 4

socket building blocks called chassis can be combined to form partitions (nPars). managed by

rack management controller (RMC)

4s chassis

HPE OneView communicates to RMC via Redfish API’s

Software

Server Infrastructure

Compute

Memory

Networking

I/O

BIOS FW

BMC FW

DATA PATH – SERVICE EVENTS TO REMOTE SUPPORT

HPE Support

Firmware management

SUM

Insight Online

C:\Users\VazquezMar\AppData\Local\Microsoft\Windows\Temporary Internet Files\Content.Outlook\30RLWBQS\Dashboard\_noRSI (2).png Customer

Insight Online

Partner

HPE Global Solution Center

Management Firmware

Operating Environment

C:\Users\RALEVE\AppData\Local\Microsoft\Windows\Temporary Internet Files\Content.Outlook\N81PS3KS\Suse\_Lockup\_RGB.png DCD

Applications

SGLX

Image result for oneView HPE HPE OneView

Troubleshooting, alerts, and connectivity to HPE Support

Insight Remote Support

ServiceNow and HPE OneView integrated management

SYSLOG

ServiceNow

Other…

• Muffles the “noise” • Fully Driven API • Reporting capability • Links to 3 rd Party SNMP monitoring

### • Python Add

on module (What gets exposed to public) • Currently in Private HPE Github

Detail of flow

• HPE OneView Global Dashboard — Aggregated critical events only • Extract routine will pull information from OVGD and processes events/alerts to a syslog file including HPE actionable events (HPE Case ID) • Architected in a plugin module setup that needs to expose an execute method • Central logging provided by the extract routine • Intelligence built in that understands when it’s a first run and subsequent runs to process delta alerts • Recommendation to run the routine under crontab or a schedule to provide for flexibility in operations

HW

Global Dashboard

HPE OneView

### GSE Plug

in

THE END
