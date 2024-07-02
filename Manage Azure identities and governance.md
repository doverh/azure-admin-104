# Manage Azure identities and governance

## Manage Microsoft Entra users and groups

Identity provided that speaks cloud. Graph (Rest based) is used to interact. Internal network uses active directory(kerberos , LDAP). Entra uses OAUTH , OIDC, SAML.

- Active Directory Domain Services (AD DS or traditionally called just "Active Directory") ON PREMISSES is a directory service that provides the methods for storing directory data, such as user accounts and passwords, and makes this data available to network users, administrators, and other devices and services. Runs as a service on Windows Server.
- Entra ID is part of platform as a service(PAAS) and operates as a Microsoft-managed directory service in the CLOUD.
Organization has a particular TENANT.
- Minimun required premium version Microsoft Entra ID P2
- Characteristics of AD DS

When comparing AD DS with Microsoft Entra ID, it’s important to note the following characteristics of AD DS:

AD DS is a true directory service, with a hierarchical X.500-based structure.
AD DS uses Domain Name System (DNS) for locating resources such as domain controllers.
You can query and manage AD DS by using Lightweight Directory Access Protocol (LDAP) calls.
AD DS primarily uses the Kerberos protocol for authentication.
AD DS uses OUs and GPOs for management.
AD DS includes computer objects, representing computers that join an Active Directory domain.
AD DS uses trusts between domains for delegated management.
You can deploy AD DS on an Azure virtual machine to enable scalability and availability for an on-premises AD DS. However, deploying AD DS on an Azure virtual machine doesn't make any use of Microsoft Entra ID.

-Characteristics of Microsoft Entra ID

Microsoft Entra ID is primarily an identity solution, and it’s designed for internet-based applications by using HTTP (port 80) and HTTPS (port 443) communications.
Microsoft Entra ID is a multi-tenant directory service.
Microsoft Entra users and groups are created in a flat structure, and there are no OUs or GPOs.
You can't query Microsoft Entra ID by using LDAP; instead, Microsoft Entra ID uses the REST API over HTTP and HTTPS.
Microsoft Entra ID doesn't use Kerberos authentication; instead, it uses HTTP and HTTPS protocols such as SAML, WS-Federation, and OpenID Connect for authentication, and uses OAuth for authorization.
Microsoft Entra ID includes federation services, and many third-party services such as Facebook are federated with and trust Microsoft Entra ID.

### Create users and groups

A user account has all the information required to authenticate the user during the sign-in process. Microsoft Entra ID supports three types of user accounts.

1.CLOUD IDENTITY - A user account with a cloud identity is defined only in Microsoft Entra ID. This type of user account includes administrator accounts and users who are managed as part of your organization.

2.DiIRECTORY SYNC IDENTITY - defined in an on-premises Active Directory. A synchronization activity occurs via Microsoft Entra Connect to bring these user accounts in to Azure. The source for these accounts is Windows Server Active Directory.

3.GUEST USERS- defined outside Azure. Examples include user accounts from other cloud providers, and Microsoft accounts like an Xbox LIVE account.

Consider user profile data.
Consider restore options for deleted accounts -  30 days after an account is removed.
Gathered account data.

## Groups

Two types of groups
1.Security Groups - sed to set permissions at group level, rather than individually. Implemented only by Entra Admin.
2.Microsoft 365 - add access for individuals outside org.
Normal users and Microsoft Entra Admin can both use Microsoft 365 groups.

## Manage user and group properties

Administrative units let you subdivide your organization into any unit that you want, and then assign specific administrators that can manage only the members of that unit.

Manage licenses in Microsoft Entra ID

Manage external users

Configure self-service password reset (SSPR)

## Manage access to Azure resources

Manage built-in Azure roles

Assign roles at different scopes

Interpret access assignments

## Manage Azure subscriptions and governance

Implement and manage Azure Policy

Configure resource locks

Apply and manage tags on resources

Manage resource groups

Manage subscriptions

Manage costs by using alerts, budgets, and Azure Advisor recommendations

Configure management groups
