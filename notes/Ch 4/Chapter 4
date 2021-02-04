4.1.3 Manageable Network Plan Facts

Term	Definition
Manageable network plan	A process created by the National Security Agency (NSA) to assist in making a network manageable, defensible, and secure.
Milestone	A component of a manageable network plan that indicates an action or event.

No.	Milestone	Description
1	Prepare to Document	A useful document:
•	Is easy to use
•	Includes enough detail
•	Documents the important things
•	Uses timestamps
•	Is protected with restricted access and possibly encryption
•	Has a printed hard copy kept in a secure location
Determining the key elements you'll need in the required documents. 
Ensure that your documents are user-friendly. With an online wiki to document information and a blog or an RSS feed to notify your administrator of changes. information contained in your documents must include usable details 
2	Map Your
Network	be aware of all the components of the network and that you know where the physical devices are including your wireless devices. The steps are:
•	Create a map of the network topology.
•	Create a list of all devices. 
o	include wireless devices.
o	Use a network scanner and then confirm manually with a room-by-room walkthrough.
o	Identify who is responsible for each device and detail other information. Record the hostname, role, and MAC address of each device. If it's available, you should also record the IP address, whether it's statically or dynamically assigned, the service tag and its physical location, and what operating system or firmware versions it may be using. Considering using a network scanner(NMap)
o	Consider using a database file to store the information.
•	Create a list of all protocols being used on the network by using a network analyzer(wireshark)Consider removing unauthorized devices and protocols from your network.
3	Protect Your Network
(Network Architecture)	•	Identify and document each user on the network/accessible data
•	Identify the high-value, business continuity network assets
•	Document the trust boundaries: look at all the systems that comprise your network and rank them by your level of trust in that system. increase security to establish boundaries between systems that have different levels of trust. low-trust systems into a demilitarized zone, or DMZ, and trusted systems on a secured network.
•	Identify the choke points that allow access between different sections of your network. protect the high-value assets that you identified earlier. Reposition choke points through the trust boundaries i.e. limit the number of internet access points on your network. 
•	Segregate and isolate networks, use principles of least privileges and separate voice from data networks. Isolate wireless from wired.
•	Isolate server functions. To reduce the security exposure, use dedicated servers for each service. If a server is compromised, the services provided by other specialized servers can continue.
•	Physically secure high-value systems
4	Reach Your Network
(Device Accessibility)	ensure that all of the devices on your network can be easily accessed while still maintaining the device's security. Accessibility includes physical access as well as remote access. 
•	Do not use insecure protocols(Cleartext FTP, Telnet)
•	Use Windows Group Policies to administer Windows systems
•	Make sure that remote access connections are secure
•	Automate administration as much as possible
5	Control Your Network
(User Access)	ensures network security but restricts user access. 
•	Limits a user to the least privilege required for the user's job
•	Limits local admins to an absolute minimum
•	Uses regular user accounts for day-to-day work
•	Uses role-based access controls
•	Doesn't let users install software
•	Sets account expiration dates
•	Disables or removes accounts when a user leaves the organization
6	Manage Your Network
Part I
(Patch Management)	establishes an update-management process for all software on your network.
•	Patch all systems on a regular schedule 
o	Apply critical patches whenever they are released
o	Include mobile devices that connect to the network infrequently
•	Automate the patching process
•	Consider using Windows Server Update Services (WSUS)
7	Manage Your Network
Part II
(Baseline Management)	provides rules for establishing a baseline for all systems. 
Analyze critical systems, general systems, and users' workstations to develop standards for comparison and evaluation of the entire network. 
Minimum requirements for hardware, software, and network statistics.
•	Create an approved application list/version number for each class of device on the network
•	Establish the criteria and process for getting an application on the approved list also establish a process for testing new applications and adding them to the approved list
•	Verify apps before adding them to the allowed list
•	Create device baselines
•	Secure web browsers
•	Create baselines for workstations, servers, routers, firewalls, and switches. Then analyze those baselines to identify security misconfigurations. Consider using the Microsoft Baseline Security Analyzer (MBSA)
•	reviewed periodically or when something changes, such as software update, new software, equipment changes, etc
8	Document Your Network	•	Processes
•	Procedures

4.2.2 Hardening Facts
Recommendation	Description
Hardening	process of increasing the security of devices and software
Use a Trusted Operating System (TOS)	OS which comes hardened and validated to a specific security level as defined in the Common Criteria for Information Technology Security Evaluation (CC). Many TOSs provide sufficient support for multilevel security, a system in which multiple levels of classified data reside within the same system, but users are not permitted to access data at different classification levels. All personnel must have access approval on a need-to-know basis.
Control login	•	Limit privileges, especially administrative privileges.
•	Change default passwords
•	Require complex passwords
•	Require multi-factor authentication
•	Use smart cards, finger print readers, text services, or other apps that send verification codes
Use configuration baselines	set of consistent requirements for a workstation or server; defines the default system configuration, including loaded software, enabled services, and domain connectivity. Further configuration and changes to the configuration can be achieved via Group Policies.

security baseline: component of the configuration baseline ensureing all workstations and servers comply with the security goals of the organization. Definition updates and changes are all configured and ready to go as part of the baseline. In addition, any enterprise hardware such as firewalls, gateways, and SPAM filters (and their configurations) are specified as part of this baseline.
Software & use baseline defines acceptable system use and supported software. 
•	Software managers control a user's ability to employ software 
•	help administrators by keeping track of use licenses 
•	reduce expenditures by limiting the number of licenses. 
•	define appropriate use policies by defining how to implement Group Policies to provide allowed services while preventing unauthorized use of disallowed services. 
Update your security baseline after new software/versions, change in security policy. This is your guideline for safe computer use to reduce attack surfaces.
Use configuration baselines as follows: 
•	Identify common configuration baselines that should be applied to all, or a group, of systems.
•	Use security templates, saved set of configuration values that produce the system configuration as specified in the configuration baseline to quickly apply security baseline settings. 
•	 Use security templates to:
o	Quickly apply settings to one or more computers.
o	Configure consistent security settings between devices.
o	Quickly restore security settings to the baseline.
o	Compare the actual settings on a device to the settings required by the configuration baseline.
Microsoft operating systems include the following tools for managing security templates: 
•	The Security Templates snap-in creates and edits templates. May obtain security templates from various sources, including the NSA,.
•	The Security Configuration and Analysis snap-in compares the existing settings with the template or applies a template to a single device..
•	The Group Policy Editor imports a template into Group Policy and applies the template to multiple computers.
Manage software	•	up-to-date licenses. 
•	Install security software such as anti-virus, anti-spyware, anti-rootkit, and firewall.
•	Install only needed software.
•	Avoid installing freeware or software from untrusted publishers.
•	Reduce the attack surface of the device by limiting applications and services running on the device and removing unnecessary software, features, and non-essential services.
o	Use role separation by installing services on separate physical systems. If a single system is compromised, only the few services on that system will be affected.
o	Remove unnecessary services, protocols, and applications following installation. 
o	Determine the dependencies of services you are using before removing existing services. 
o	non-essential services include TFTP, Telnet, and SNMP.
o	Essential: DNS, ICMP, and NNTP are generally considered essential protocols and services
Use a Standard Operating Environment (SOE)	•	implemented as a standard disk image or master image. 
•	used when deploying new computers to the network. 
•	Automation used when deploying the master image and when running configuration scripts, to give the computer a name, to join a domain, and during any other customizations. 
•	reduces security risks by ensuring that security standards are consistent throughout the network. Master images should be based on a TOS and be fully patched.
Managing Updates
Update Type	Description
Hotfix	quick fix for a specific problem 
•	Typically made to address a specific customer situation and possibly may not be distributed outside that customer organization.
•	Commonly used to address freshly discovered security holes.
Patch	•	also a quick fix, more thoroughly tested 
•	designed for a wider deployment. 
•	Include previous hotfixes 
•	Include fixes that should be applied to wider audiences, such as patching security holes.
Best obtained from the manufacturer's website.
Service pack (SP)	•	collection of patches, hotfixes, and other system enhancements tested by the manufacturer for wide deployment. 
•	includes all previously released bug fixes, individual patches and previous SPs. 
•	Test in small group before wide deployment.

Use patch management software	simplify the patch distribution and management process. 

Windows Software Update Services (WSUS) allows clients on a network to download software updates from a WSUS server internal to their organization. 
•	The WSUS server receives a list of available updates from Microsoft.
•	On the WSUS server, you identify allowed or required patches for your organization.
•	Clients download only approved patches from an internal WSUS server or directly from Microsoft.
•	can also use Group Policy to distribute and automatically install patches. 
•	must use Group Policy to install updates to non-Microsoft software that is not supported by WSUS.
Patch management activities 
	•	determining which patches are needed on your systems 
•	create a system restore point before you patch systems
•	test in deployment group/power users, especially with service packs
•	applying patches,  first by department, then system-wide.
•	auditing for the successful application of those patches. 

Active Directory Users and Computers. 
•	rename the account in Properties, or create a new account for the administrator. 
•	Administrator account has many groups assigned to it, such as domain admins, required for group policy management. By default, a general administrator doesn't have access to group policy management. 
•	Use new account and disable admin account once you are sure you will not be locked out.
•	change default passwords. 
•	Use groups to control what users can access and what they can do. 
•	lock down the domain controller behavior. security options affect everyone. 
•	Consider having Ctrl + Alt + Del at startup, which can prevent some malware. May cause some problems for users, and must be set across the board.
•	installing only required software on the systems. Use role-based or feature-based installation, or Remote Desktop Service installation. 
•	Windows Server only installs binaries for any service that you want to run on the server. IN newer servers , security configuration wizard has been completely removed, so features are secured by default, REDUCING ATTACK SURFACE. 
•	use Group Policy Manager or Microsoft Security Compliance Manager to control specific security settings. 
•	disable or turn off at least the startup behavior of any services that the machine does not require
•	be careful not to disable a service that may be critical

4.3 File Server Security
Term	Definition
Shared folder	A folder whose contents are available over the network.
Network-attached 
storage (NAS)	A standalone storage device or appliance that acts as a file server.
Storage area network (SAN)	A special network composed of high-speed storage that is shared by multiple servers.
best practices	•	keep all file servers physically secure
•	principle of least privilege. 
•	use full-disk encryption on all storage mediums, or at least encrypt backups
•	Or :fully decrypt drives when they're powered on and encrypt them when the system shuts down. May not prevent someone from transferring files to a USB drive, but does prevent physical drive/server theft. 
•	Implement strong authentication 
•	Use hidden folders and files
•	file server needs proper auditing enabled that can track user behavior, such as when files are accessed, modified, deleted, and moved.
•	use implicit deny access control lists, or ACLs. ACLs control the system's permission. prevent access to everything that isn't explicitly granted. 
File server security	•	Use IPSec or a VPN to secure data in transit.
•	File and print resources are primarily vulnerable (DoS) and access attacks.
•	Attacks on file servers are often directed against the NetBIOS protocol. Verify that NetBIOS is not required on the server, disable the NetBIOS protocol on the server, and use a host-based firewall to close NetBIOS ports 135 and 137 - 139.
•	A shared folder is a folder whose contents are available over the network. 
o	An administrative share i= admins only, hidden
o	By default, the root of every drive is an administrative share.
o	appending  [&dollar] makes shares hidden
o	Users must know the name and have permission to access.
o	Do not share the root directory with regular users.
•	With Windows Server 2008 and later, File Server Resource Manager (FSRM) can control files saved on a file server. 
o	Quotas limit the amount of data that can be saved within a folder. Hard and soft limits available
o	File screens restrict the type of files that can be saved in a folder. can prevent media files (audio and video) or files with specific file extensions from being saved.  Active vs Passive.


4.3.2 File System Security Facts
Solution	Description
Big Data Storage
	•	Measured in Exabyte’s.
•	Analyzed to identify business trends, create computer models, and isolate network attacks.
•	Usually stored on NAS or SAN devices.
Network attached storage (NAS)	Standalone storage device or appliance that acts as a file server. 
•	Connected to the same network as all other network devices. And exposed to attacks from all network hosts.
•	Typically use well-known standard protocols for file sharing. 
•	Often has a limited operating system capable of sharing files and ACLs.
•	Should be secured with a strong password and strong authentication.
Storage area network (SAN)	Special network composed of high-speed storage that is shared by multiple servers. Typically a separate network that only file servers attach to. Security done as below:
•	Logical Unit Number (LUN) masking identifies devices that are allowed to attach to a logical unit.
•	SAN zoning groups SAN devices and servers into security zones. Only devices within the security zone can access data on the storage unit.
•	The Fibre Channel Authentication Protocol (FCAP) provides a method for mutual authentication of devices within the SAN. 
 more secure than NAS solutions.
Data Transfer Security Protocols
Protocol	Description
File Transfer Protocol 
(FTP)	•	Anonymous login (also known as blind or anonymous FTP) allows unrestricted access to the FTP server. Disable anonymous login to control access based on username.
•	Use secure protocols such as SSL( secure socket layer) to protect logon credentials, transmitted in cleartext.
•	Use IPSec or a VPN/SSH tunnel to protect data transfers. 
•	Restrict write permissions, = ability to upload.
•	Port 2- for transfer, 21 for login.
Trivial File Transfer Protocol 
(TFTP)	TFTP provides no authentication, encryption, or error detection. In addition, TFTP uses UDP instead of TCP. TFTP might be faster than FTP, but it does not perform error detection, so it could result in file errors.
Secure Copy Protocol 
(SCP)	SCP uses Secure Shell version 1 (SSH1) to secure file transfers and login credentials. CLI only, no directory traversal.
Secure Shell File Transfer Protocol 
(SFTP)	SFTP is a file transfer protocol that uses Secure Shell version 2 (SSH2) to secure data transfers. SFTP is not FTP that uses SSH, but rather a secure transfer protocol that is different from FTP. GUI and user-friendly
Secure FTP
(SEC-FTP)	Secure FTP (also known as FTP over SSH) tunnels FTP traffic through an SSH tunnel. 
FTP Secure 
(FTPS)	FTPS adds SSL or Transport Layer Security (TLS) to FTP in order to secure logon credentials and encrypt data transfers. FTPS requires a server certificate.

4.3.3 File Permission Facts
Permission Type	Description
Share	Controls access through a network connection with the file server. 
•	If files are accessed locally, share permissions do not control access.
•	Share permissions have three levels of permissions: 
o	Reader (read only)
o	Contributor (read and write)
o	Owner or Co-owner (full control, or all permissions)
•	Share permissions can be set only on a folder.
NTFS	NTFS permissions: 
•	Can be set on drives, folders, and files.
•	Control both local and network access.
•	Have dozens of permissions that offer granular control over what actions are allowed.
•	Can be set only on volumes formatted with NTFS.
File Permission Facts	•	Share and NTFS permissions use a discretionary access control list (DACL) for controlling access,which identifies the users or groups and their associated permissions to files or folders.
•	Both share and NTFS permissions include Allow or Deny permissions. Deny permissions override Allow permissions.
•	Both share and NTFS permissions must be configured to allow access through the share. (Both exist in the infrastructure)
•	Effective permissions to shared folders are the more restrictive of either share or NTFS permissions.
•	A user's effective permissions cannot be greater than the share permissions assigned to the user or a group to which the user belongs. 
•	common strategy for combining share and NTFS permissions: 
o	Assign Co-owner share permissions to Everyone.
o	Use NTFS permissions with least privilege to control access. 
o	Use the principle of least privilege by assigning NTFS permissions 
•	Permissions for folders and files can be inherited. 
•	Whenever possible, assign permissions to groups, rather than users. Users receive the permissions assigned to their groups.
4.4 Linux Host Security
Term	Definition
iptables	Built-in firewall command line utility for Linux operation systems that uses three policy chains to allow or block network traffic.
Chains
	(sets of rules) to allow or block network traffic. 

•	Input: Controls the behavior for incoming connections. 
1.	Ex: if a user attempts to ping the system, iptables attempts to match the IP address and port to a rule in the input chain.
•	Forward: Used for past-through packets leaving the system. 
•	Output: ping testout.com, iptables checks its output chain to see what the rules are regarding ping and testout.com before allowing or denying the ping request.
•	Default 
Actions	•	Allows the connection. 
•	Drops the connection. No response is sent to the user. 
•	Rejects the connection, with response.
Examples iptables Commands
Action 	Command
List current rules	sudo iptables -L
Clear current rules	sudo iptables -F
Save iptables changes (Ubuntu) 	sudo /sbin/iptables-save 
The command may be different on other Linux systems.
Drop all incoming traffic	sudo iptables -A INPUT -j DROP
Block connections from 192.168.0.254	sudo iptables -A INPUT -s 192.168.0.254 -j DROP
Block SMTP mail on port 25	sudo iptables -A OUTPUT -p tcp --dport 25 -j REJECT
Allow SMTP mail on port 25	sudo iptables -A INPUT -p tcp --dport 25 -m conntrack --ctstate NEW,ESTABLISHED -j ACCEPT
sudo iptables -A OUTPUT -p tcp --sport 25 -m conntrack --ctstate ESTABLISHED -j ACCEPT
Allow HTTP traffic on port 80 	sudo iptables -A INPUT -p tcp --dport 80 -m conntrack --ctstate NEW,ESTABLISHED -j ACCEPT
sudo iptables -A OUTPUT -p tcp --sport 80 -m conntrack --ctstate ESTABLISHED -j ACCEPT 
To allow HTTPS, you would use port 443.
Allow HTTP traffic on port
Allow HTTPS traffic on port 443	sudo iptables -A INPUT -p tcp -m multiport --dports 80,443 -m conntrack --ctstate NEW,ESTABLISHED -j ACCEPT
sudo iptables -A OUTPUT -p tcp -m multiport --dports 80,443 -m conntrack --ctstate ESTABLISHED -j ACCEPT
Linux Hardening
Security Task	Procedure
Remove unnecessary software	1.	Enter one of the following commands:
o	yum list installed to see installed RPM packages on the computer.
o	apt 
	apt autoremove automatically removes unused packages
	apt list list all installed packages
o	dpkg get-selections to see installed Debian packages on the computer.
2.	Research and evaluate.
3.	Use one of the following commands to uninstall unnecessary packages.
o	yum erase packagename
o	apt remove packagename
o	rpm -e packagename
o	dpkg -r packagename
Check for unnecessary network services	Many services utilize a specific TCP/IP port that's exposed to the network. Services such as DNS, FTP, SNMP, and others may or may not be required on your system.
1.	Find all installed services and determine which are not needed:  DNS, SNMP, DHCP and others. 
o	systemctl --type=service --state=active
2.	Use the man command and the Internet to research services you don't recognize.
o	If the service is not needed, determine if it is a dependency for another service.
3.	Disable the service by using the following command:
o	systemctl disable servicename
o	systemctl enable x (at startup)
o	is-enabled checks for status
4.	Use one of the following commands to immediately stop the script:
o	systemctl stop servicename
5.	Use one of the following commands to remove the script package entirely.
o	yum erase packagename
o	apt remove packagename
o	rpm -e packagename
o	dpkg -r packagename
6.	cd/etc/init.d/ (view services)[older, deprecated]
Locate open ports	1.	Install the nmap utility if it is not already installed.
o	yum install nmap
o	apt -i nmap
2.	Use both of the following commands to scan for open ports:
o	nmap -sT ipaddress|fqdn scans for TCP ports
o	nmap -sU ipaddress|fqdn scans for UDP ports
-6 for ipv6, -A or –O for OS detection, -p for range, -sn for ping only for host availability.
3.	Determine which services use the open ports.
4.	Disable any unused service using the open ports information.  (Make sure the service used is not a dependency for another service).
o	systemctl disable servicename
o	systemctl stop servicename
Check network connections	A socket is an endpoint of a bi-directional communication flow across a computer network. Use the following netstat (network statistics) options 
•	-a lists both listening and non-listening sockets.
•	-l (lowercase 'L') lists listening sockets.
•	-s displays statistics for each protocol enabled on system.
•	-i displays a table of all network interfaces.
•	-r for routing table
Install needed updates
	•	Debian(Ubuntu/mint) apt update
•	Redhat(CentOS/Fedora) yum update
•	SuSe:zipper
Enable host-based firewall	•	firewalld(python dependent)
•	gatekeeper between your system and the external and internal network.
•	monitors all traffic that flows in both directions between the computer and network, configured with ACLs(access control lists)

‘systemctl start firewalld'
	
--state: status
--get-active-zones: default zone configuration (levels of security)

Give exceptions to enable traffic with ports
Firewall-cmd, firewall –permanent(make permanent exceptions)

-reload: refresh firewall after new exceptions

