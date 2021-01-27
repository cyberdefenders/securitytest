# 6.2 - Authentication
by Sabrina

## Chapter Topics

- Authentication
- Identity
- Authentication Methods
- Biometric Authentication
- Authentication Technologies

## Authentication

- Authentication is usually the 2nd step in identification process
  - It's verification process proving that you are who you say you are

### Multi-Factor Authentication

- Requires more than one method of identification, using factors and attributes

#### Factors for Authentication

|       Factor       |                         Description                          |
| :----------------: | :----------------------------------------------------------: |
| Something you know | Weakest type of authentication, though most commonly used. Can be passwords, PINs, passphrases, security questions, or other information used along with a username to validate identity |
| Something you have | Also called token-based authentication, this is based on something physical in your possession. Can be swipe cards, photo IDs, key fobs, security tokens, or smart cards |
| Something you are  | Uses a biometric system to authenticate. Can be eye/retina scan, fingerprint, etc. Most expensive and considered to be most secure form of authentication |

#### Attributes for Authentication

- Attributes (unlike factors) do not on their own verify identity

- They do help improve security and work well when MFA is needed

  |       Attribute       |                         Description                          |
  | :-------------------: | :----------------------------------------------------------: |
  | Something you can do  | Requires you to perform an action to verify your identity. Can be supplying handwriting sample to be analyzed against a baseline, or typing a sample text to analyze typing behaviors to verify identity |
  | Something you exhibit | Can be a personality trait or a habit, such as the time of day you usually log on, method used to access information, type of tasks usually peformed. If the actions exhibited are unusal or considered risky, access can be restricted by administrators |
  |   Somewhere you are   |    Geolocation uses physical location to verify identity     |
  |   Someone you know    | Certificates and attestation are examples of this attribute  |

  ## Identity

  - Identity is as simple as providing a name/username, but alone identity is not secure

  ### Key Identity Terms

  - **Identity Provider (IdP)** - online service that manages identity info for other organizations, and IdP creates records from the organization's existing data and those records are then used to authenticate

  - **Attributes** - can be your role, position, or current project. Often used to determine policy and permission.

  - **Certificates** - issued by a certificate authority and verify identity by providing the following:

    - Public keys
    - Details on owner of the certificate
    - Details on issuer of the certificate

  - **Tokens** - device or file used to authenticate. Some examples are hardware tokens (key fobs) or soft tokens (stored on devices)

  - **SSH Keys** - an access credential that operates like usernames and passwords but mostly used to implement single sign-on (SSO) and other automated processes

    

  ## Authentication Methods

  ### Types of Authentication Methods

  |       Method       |                         Description                          |
  | :----------------: | :----------------------------------------------------------: |
  | Directory Services | Implement SSO for resources on a network. Examples are Active Directory on a Microsoft Network, LDAP Directory Services, or Azure AD which is an identity and access management solution for the cloud. Can be implemented between directory service systems if they are compatible, such as with Windows and Linux |
  |     Federation     | A group of domains that have established trust and therefore share authorizations. Can be within one organization with multiple domains or include several trusted organizations to share resources. Everything happens onsite and provides detailed levels of access control |
  |    Attestation     | A protocol used to prove that a software can be trusted. Tells remote user that the application/software is legitimate and has been certified. |

  ## Biometric Authentication

  - Biometric authentication is based on a unique physical attribute or characteristic
  - For biometric authentication to be a viable security mechanism, it must conform to the following parameters:
    - **Universal** - Does each person have the physical attribute being measured?
    - **Unique** - Is the attribute distinctive enough that it can be used to distinguish between individuals?
    - **Permanent** -  How well does the specified attribute hold up to aging?
    - **Collectible** - How easy is it to acquire this measurable attribute?
    - **Circumvention** - Can the attribute be easily circumvented?
    - **Accuracy** - Are the results accurate? (See: false rejection rate FRR, falce acceptance rate FAR, and crossover error rate)
  - Biometric information can be collected for fingerprint, retina, iris, facial, voice, vein, or gait analyzation. 

  ### Biometric Authentication Considerations

  - Biometrics used alone are no more secure than a strong password
  - Biometric attacks aren't necessarily violent attacks (i.e cutting off a finger) but can be a number of methods to fool the biometric reader
  - The most important consideration for a biometric device is accuracy

  ## Authentication Technologies

  ### Technologies Used for MFA

  |         Technology          |                         Description                          |
  | :-------------------------: | :----------------------------------------------------------: |
  | Short Message Service (SMS) |     Uses SMS messaging to send one-time code or password     |
  |         Phone Call          | User receives a phone call with the one-time code or password |
  | Authentication Applications | Third-party tools used by organizations to authenticate their users. Authenticator apps are often used. Similarly used is a one-time password that can be created via HMAC-based one-time password (HOTP) or time-based one-time password (TOPT) |
  |      Push notification      | After providing a username, user receives an access request notification via their mobile device |

  
