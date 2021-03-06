**_Wednesday, January 13, 2020_ | _Chapter 5: Devices and Infrasfrastructure_ | _Nick Handy_**

# 5.13 Router Security

## Section Focus

Ways to make routers more secure

## Key Terms

| Term                      | Definition                                                   |
| :------------------------ | :----------------------------------------------------------- |
| Router                    | A network device that transmits data from one network to another. |
| Access Control List (ACL) | A router filter that controls which network packets are permitted (forwarded) or denied (dropped) in or  out of a network. |

## Router Security

#### Change Default Config Settings

- Change Default username and password
  - Make both username and password complex and hard to guess
  - Change them before putting router online
- Change default IP address range
  - Security through obscurity
- SOHO Routers
  - Change SSID Range

#### Keep Router Firmware Up-to-date

#### Change connection protocol of router

- Example change FTP -> SFTP for router configuration
- Old routers are more likely to use insecure protocols
- Universal Plug and Play (UPnP)
  - Very insecure, disable it if it is a feature of the router

#### Disable Remote Access

- Do not allow remote access unless absolutely necessary
  - If it needs to be enabled, keep the amount of time it is accessible short

#### Keep Router in Secure Location

#### Encrypt and Backup Configuration Files

## Router ACLs

### Overview

- The ACL is not a routing table
- What can an ACL do?
  - An ACL on a router could ban all incoming traffic destined to a specific IP address inside the network

### Types of ACLs

###### Standard ACL

- Only able to filter traffic based on the sources host name or host IP
  - It can't filter traffic based on port number, destination host name, or host IP address

###### Extended ACLs

- Can filter traffic based on many more parameters than standard ACLs

| ACL Type     | Filters by                                                   | Placement in network                        |
| ------------ | ------------------------------------------------------------ | ------------------------------------------- |
| Standard ACL | Source host name or host IP address                          | As close to the **destination** as possible |
| Extended ACL | Source IP protocol<br />Source/Destination socket number<br />Destination host name or host IP address | As close to the **source** as possible      |

### Configuring an ACL

Access control lists can give us granular control over how data flows across our networks, and which computers can communicate with specific protocols

- The list defines what can and cannot be done on the network
- Can be configured with the router's configuration terminal
- Permit-and-deny statements, with an implicit deny at the end. 
- Typical lists range from 1-99 or 1300-1999

##### Example ACL Configuration

```dockerfile
# Standard ACL configuration
conf t	# open config menu
access-list 10 deny 10.0.0.2 0.0.0.0	# deny connections from host ip 10.0.0.2
int fa0/1 # selecting interface to apply access-list to
ip access-group 10 in # apply access list to the selected interface
no ip access-group 10 in # reverse previous command

# Extended Access Control List
access-list 100 deny icmp host 10.0.0.2 0.0.0.0 255.255.255.255 # deny access to ICMP
access-list 100 permit ip host 10.0.0.2 10.0.0.0 255.255.255.255 any # allow all other protocols
int fa0/1 # select interface to apply ACL to
ip access-group 100 in # apply access list to interface

```

