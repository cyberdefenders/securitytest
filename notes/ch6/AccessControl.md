6.1 Access Control Models
by John

| Term | Definition |
| --- | --- |
| Access control | Access control is the ability to permit or deny access to resources on a network or computer.
Access control is the ability to permit or deny the privileges that a user has when accessing resources on a network or computer. Access control involves three entities:
- _Objects_ are data, applications, systems, networks, and physical space.
- _Subjects_ are users, applications, or processes that need access to objects.
- The _access control system_ includes policies, procedures, and technologies that are implemented to control subjects&#39; access to objects.
Access control includes the following processes:
- _Identification_ specifies the name used to identify the subject. Examples include a user name or a user ID number.
- _Authentication_ is the process of validating a subject&#39;s identity. It includes the identification process, the user providing input to prove identity, and the system accepting that input as valid.
- _Authorization_ is granting or denying an authenticated subject&#39;s access to an object based on the subject&#39;s level of permissions or the actions allowed with the object.
- _Auditing_, also referred to as _accounting_, is maintaining a record of a subject&#39;s activity within the information system.
 |
| Access control policy | An access control policy defines the steps and measures that are taken to control access to objects.
- _Preventive_ access controls deter intrusion or attacks. These include separation of duties and dual-custody processes.
- _Detective_ access controls search for details about the attack or the attacker. These include intrusion detection systems.
- _Corrective_ access controls implement short-term repairs to restore basic functionality following an attack.
- _Deterrent_ access controls discourage attack escalation.
- _Recovery_ access controls restore the system to normal operations after the attack and the short-term stabilization period.
- _Compensative_ access controls are alternatives to primary access controls.
 |
| Access control system | An access control system includes policies, procedures, and technologies that are implemented to control access to objects.Within the directory service:
- A user account is created for each subject.
- Identification is performed during logon when the user supplies a valid user account name.
- Authentication is performed during logon when the user password or other credentials are verified.
- Authorization to use network resources, such as files, printers, or computers, is controlled by permissions or rights.
- Auditing is performed by the operating system as it tracks subjects&#39; actions toward objects.
 |
| Access control measures | Access control measures can also be classified based on how they restrict or control access:
- _Administrative_ controls are policies that describe accepted practices. Examples include directive policies and employee awareness training.
- _Technical_ controls are computer mechanisms that restrict access. Examples include encryption, one-time passwords, access control lists, and firewall rules.
- _Physical_ controls restrict physical access. Examples include perimeter security, site location, networking cables, and employee segregation.
 |
| Access Control Models | **Discretionary Access Control** , or DAC.
- Least restrictive
- Individual resources have owners which decide who has access using **DACLs** /groups. Example: NTFS within a Windows system.
- Objects have DACL entries for each subject.
- Owners add subjects to the DACL, assign rights or permissions.
- Subjects can pass permissions on to other subjects.
**Dynamic Access Control** (DYAC) enhances NTFS permissions, controlling access to files and folders by adding tags and policies.

**Mandatory access control, or MAC**
- Static system with classification labels and levels. Every computer, every file, and every object is assigned a label, indicating importance.
- MAC compares the object labels with the user&#39;s access level to grant or deny access to a given resource.
- Example: Confidential, Secret, and Top Secret vs. 3 user access levels.
- Users with access level 1 can see anything labeled Confidential only. Level 2 can see anything labeled Confidential or Secret, but not Top Secret.
- Users with access level 3 can see anything.
- permissions can&#39;t be altered for specific instances
- Policy rather than ID based. Owners may only assign labels.
**Role-based access control(user)**
- Hybrid between MAC and DAC, and the most commonly used.
- role within the organization determines whether or not you&#39;re able to access certain kinds of data.
- Example: CFO can see Financial records, and reception can only see calendars.
- Group-based access control uses a collection of users; **RBAC uses a collection of permissions.**
**Rule-based access control(router/traffic)**
- Used with routers through router ACLs.
- Decide which IPs are allowed through the router using rules.
- Nothing to do with user account, group membership or classification labels. (ID neutral)
- Access control entries identify characteristics to match.
- If all characteristics match, access allowed or denied based on rule.
- Example of a rule-based access control: allows or denies traffic based on characteristics within the packet
- Count as a form of mandatory access control.
**Attribute-Based Access Control, or ABAC**
- More flexible, **combines object attributes to determine access with user&#39;s role, position, or even project association.**
- If-then-else format. If the user has the required attribute, they&#39;re granted access. If the user doesn&#39;t have the required attribute, they&#39;re denied access.
- Example: Role, Department, Project labels
- Check: if role = manager, if department = development, if on Boring App.project? Any fail = denial.
- uses special markup language, eXtensible Access Control Markup Language ( **XACML** ) to define access control policies
**Conditional Access**
- Enforce access control while also encouraging users to be productive
- Not intended as the first point of security, but after granting first-factor authentication, can be configured to consider many different factors.
- Administrators can:
- **maintain specific control at the user or group level** ,
- **permit or deny access based on an IP address or an IP range** ,
- **Permit, restrict, or deny access to users that use specific applications or devices/device states.**
 |
| Authentication | Process of validating identity.
Identification process:
1. user providing input to prove identity, i.e. claiming to be a user with (insert username here).
2. system accepting that input as valid. Verification done via password, toke, biometrics, etc. and compared against database.
 |
| Authorization | Granting or denying access to an object based on the level of permissions or the actions allowed with the object.First step: system administrator configures the rules for each user or group that dictate their access rights—&quot;their permission scope. Second step: After authentication, a user is either authorized or denied access to a particular resource based on the rules configured. |
| Auditing/Accounting | Tracks/gathers data on the actions of an authenticated user. A company might track:
- which files a user accesses,
- how much data a user sends and receives over the network,
- What times the user is active on the system,etc.
 |
| AAA server/example | User-server interaction is required for the AAA process
- User gives username and password to access company wireless network. **The username is their identity, and the password verifies their identity.**
AAA server compares this information to the records stored in its database. Both match = **authentication** completed.AAA server checks rules to ensure user is **authorized** to access these files. **Accounting** : User activity, initial connection, the attempt to access this file server, and the opening of this document have all been logged by the server. Even when the user disconnects, this action will be logged by the accounting process. |
| Objects | Objects are data, applications, systems, networks, and physical space. |
| Subjects | Subjects are users, applications, or processes that need access to objects. |
| Principle of least privilege | Easier to give privilege than it is to take away. Control Methods:
- _Implicit deny_ denies access to users or groups who are not specifically given access to a resource. Weakest form of privilege control.
- _Explicit allow_ specifically identifies users or groups who have access. Moderate form of access control
- _Explicit deny_ identifies users or groups who are not allowed access. Strongest form of access control/overrules.
Access recertification: continually reviewing permissions and privileges to make sure the user has the correct level of access. |
| _Need to know_ | Restriction of highly sensitive data unless needed for duty.
- Discourages casual browsing of sensitive materials.
- Even in a top secret setting, only given what they need, aka **mandatory access control (MAC).**
 |
| Separation of duties |
- System users should have the lowest level of rights and privileges necessary for work and should have those privileges only for the shortest length of time possible.
- To achieve a separation of duties, a business can use the principle of **split knowledge**. no single person has total control of a system&#39;s security mechanisms/ability to compromise systems.
- In cases of sensitive or high-risk transactions, a business can use two-man controls.
Having more than one person required to complete a task.
- reduce conflicts of interest.
- prevents insider attacks because no one person has end-to-end control and no one person is irreplaceable.

 |
| Job rotation | Cross trains staff in different functional areas in order to detect fraud.
- Exchanges positions of two or more employees to allow for oversight of past transactions.
- Can be used for training purposes.
 |
| Defense-in-depth |
- _A_n access control principle which implements multiple access control methods. Multiple defenses make it harder to bypass security measures.
 |
| Identification | Act of claiming an identity, such as telling someone your name. Important facts to know about identification include:
- username is a form of identification.
- Because anyone could pretend to be the user, identification by itself is not very secure.
To substantiate identity, the person must provide some form of identity verification. |
| _Multi-Factor Authentication_ | Using more than one way to verify identity. Something you are, such as biometric information (e.g., fingerprint or retina scan).
- Something you have, such as smart cards, RSA tokens, or security key fobs.
- Something you know, such as passwords and PINs.
- Somewhere you are, such as a geographical location.
- Something you do, such as how you type a sentence on a keyboard.
 |
| _Mutual authentication_ |
- Two communicating entities authenticate each other before exchanging data. It requires not only the server to authenticate the user, but the user to authenticate the server. More secure than one-way.
 |
| Transition Best Practices
 |
- **Creeping privileges** : user&#39;s current access privileges are not removed or modified with new posting, resulting in privilege escalation.
- User accumulates unnecessary privileges..
On account creation:
- Apply the appropriate access rights based on job role implemented in the access control system.
- Give only the minimum privileges required for duties.
When account is active:
- Modify access rights as job roles and circumstances change.
- Monitor password resets and lockouts to ensure account security.
- Re-evaluate access rights on a periodic basis.
When an account is no longer needed, take appropriate actions to:
- Delete accounts that will no longer be used.
- Rename accounts to give new users in the same job role the same access privileges.
- Lock accounts that will not be used for extended periods
- Remove unnecessary rights from accounts that will be kept on the system.
- Archive important data or files owned by the user, or assign ownership to another user.
- Prohibit the use of generic user accounts, such as the Guest or Administrator users on Windows systems.
End-of-life procedures prevent sensitive data from being accessible to unauthorized users
- deactivating /deleting unused accounts
- destroying data that might remain on storage media
 |

