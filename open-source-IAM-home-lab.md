# Open Source IAM Home-Lab

## ℹ️Overview

This Home-lab focuses on Open-source Identity and Access Management tool. If you are interested to become a Security Engineer, this home-lab suite will help you set up a custom open source IAM solution.
Keycloak is an open-source Identity and Access Management (IAM) solution aimed at modern applications and services. It offers out-of-the-box support for web applications, single sign-on (SSO), two-factor authentication, and social login. 


## 🧮Requirements

**Hardware**: At least 4GB of RAM and 2 CPU cores (virtual or physical).  
**Software**:
- Docker and Docker Compose (for container management).
- JDK 11+ (if running Keycloak natively or for development purposes).

## 🖼️Lab Diagram

+-----------------+       +------------------+       +-----------------+
|                 |       |                  |       |                 |
|  User Browser   +------>+  Keycloak Server +------>+  Application(s) |
|                 |       |                  |       |                 |
+-----------------+       +------------------+       +-----------------+
                                 ^
                                 |
                          +------+------+
                          |             |
                          | Database    |
                          | (PostgreSQL)|
                          |             |
                          +-------------+

## What will you learn?
In this Open Source IAM Home-Lab, you'll master Keycloak and open-source IAM tools. Gain hands-on experience in:

- Setting up and configuring IAM solutions
- Implementing security measures like SSO and 2FA
- Customizing login pages and extending functionality
- Integrating LDAP, social login, and external systems
- Managing access control and monitoring user activities
- Implementing multi-tenancy and enhancing interoperability.


## </> Setting up Keycloak IAM

- **Installation**: Use Docker for an easy setup. Follow the Keycloak [Docker Guide](https://www.keycloak.org/getting-started/getting-started-docker).  

- **Initial Configuration**: Access the Keycloak Admin Console at http://localhost:8080/auth. Default admin credentials are used for login.  

- **Create a Realm**: Realms manage users, credentials, roles, and groups. Creating a New [Realm Guide](https://www.keycloak.org/docs/latest/server_admin/#configuring-realms).  

- **Define a Provider**: Organizations can have databases containing information, passwords, and other credentials. Add a [Provider](https://www.keycloak.org/docs/latest/server_admin/#adding-a-provider)  

- **Roles and Users**: Add roles and users under their respective tabs. Managing [Users and Roles](https://www.keycloak.org/docs/latest/server_admin/#assembly-managing-users_server_administration_guide).   


## 🧑‍💻Excercises
- **Create a New Realm**: Follow the guide to create and configure a new realm separate from the Master realm.
- **Define a New Client**: Add a new client for your application with appropriate settings for access type and valid redirects.  
- **User Registration**: Enable user registration in your realm and sign up a new user account.  
- **Configure Social Identity Providers**: Add a social identity provider, such as Google or Facebook, and test social login.  
- **Setup OTP for Two-Factor Authentication**: Configure and test OTP as a second authentication factor for a user.  
- **Customize Themes**: Change the theme of the login, admin console, or account management pages.  
- **Configure Client Scopes**: Create and apply client scopes to limit the information and access provided by tokens.  
- **User Federation with LDAP**: Integrate an LDAP directory for user federation and synchronize users.  
- **Role Mapping for Federated Users**: Map LDAP roles to Keycloak roles for federated users.  
- **Group Management**: Create groups, assign users to groups, and manage group roles.  
- **Session Management**: View and manage user sessions in the admin console, including logging out sessions.  
- **User Attributes**: Add custom user attributes and configure them to appear in the token claims.  
- **Fine-Grained Authorization**: Configure resource-based permissions and policies for a client.  
- **Service Accounts**: Create and configure a service account for a client for server-to-server communication.  
- **Protocol Mappers**: Add a protocol mapper to customize the claims in the token issued by Keycloak.  
- **Event Logging and Reporting**: Enable and review login and admin events for auditing purposes.  
- **Password Policies**: Set up and enforce password policies for users in your realm.  
- **Consent Management**: Configure client consent requirements and manage user consents.  
- **Multi-Tenancy Setup**: Configure Keycloak for multi-tenancy using realms or by configuring one realm to manage multiple tenants.  
- **Token Exchange**: Setup and test token exchange between clients or between realms.  


