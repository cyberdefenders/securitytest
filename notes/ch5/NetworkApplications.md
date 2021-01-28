**_Wednesday, December 30, 2020_ | _Chapter 5: Devices and Infrasfrastructure_ | _Nick Handy_**

# 5.10 Network Applications

## Section Focus

Network Applications that can pose a threat to your network.

## Key Terms

| Term                        | Definition                                                   |
| :-------------------------- | :----------------------------------------------------------- |
| Peer-to-Peer (P2P) Software | Software that allows users to share content without centralized servers or centralized access control. |
| Instant Messaging           | Real-time text messaging communication that supports picture, music, and document exchange. |

## Peer-To-Peer (P2P) Networking Applications

> Peer-to-peer applications are a great way to share bandwidth and resources. However, they also pose a security risk to an organization.

P2P software allows users to share files without the need of a central server. Connections are made on the fly from one user to another. P2P software usually comes in the form as a torrent client such as *BitTorrent* or *uTorrent*. 

### Security Considerations

- Malware
  - Files from other users could contain malware

- Bandwidth Hogging
  - Without proper limits P2P can use a lot of upload/download bandwidth
- Knowlingly or Unknowling sharing confidential files
  - Files accessible from other users might be posted illegally

### Security Steps

| Security Step                     | Explanation                                                  |
| --------------------------------- | ------------------------------------------------------------ |
| Block P2P Ports                   | One option is to block the port the P2P software is using. This is not always effective since P2P software can change ports or use dynamic ports. |
| Blacklist P2P Traffic             | Add peer-to-peer traffic to the blacklist of a network content filter. The content filter can do all the work of identifying P2P packets. |
| Prevent P2P Software Installation | Blocking the installation of P2P software can be an effective measure for company owned devices. However, this does not protect against P2P software being used on the network. |

## Instant Messaging (IM) Applications

> Instant messaging can be great for company productivity and collaboration, especially when working with people in different geographic locations. However, they do pose a security risk.

Instant Message applications provide text communication and media/document exchange. 

### Common IM Applications

- Google Talk
- Skype
- iMessage
- Facebook Messenger
- Internet Relay Chat (IRC)
- Slack
- Discord

### Potential Threats

- IM communication could contain malware, viruses, social engineering exploits
- An IM can be susceptable to sniffing, capturing and viewing by others 
- Instant Messaging Spam (SPIM)
  - IM systems contain user directories, making it easy to identify spim targets
  - IM systems often contain demographic information about users
  - Information in contact lists can be remotely accessed
- IM clients can provide a lot of information about a user's system and their activity 
- Client-side scripting allows attackers to send messages on behalf of other IM users and can be used to create            social engineering attacks

## Configuring Application Control Software

Application controls focus on controlling the applications a user at a workstation can access over a network. 

#### Benefits

Implementing an application control system can provide additional security to a firewall. The application control system can identify application packets instead of just applying a filter to the network traffic. By identifying the packets this solution can block unauthorized applications. A central application whitelist can be applied to all devices on the network.  

