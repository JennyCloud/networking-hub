# Logical Security

Logical security refers to software-based protections that safeguard data, systems, and network access. Key concepts include:

## Encryption
- **Data in Transit**: Protects data while moving across networks (e.g., HTTPS, TLS, VPN).
- **Data at Rest**: Protects stored data on disks, databases, or cloud storage (e.g., AES, BitLocker).

## Public Key Infrastructure (PKI)
- Framework for managing **digital certificates** and **public/private keys**.
- Ensures secure communications and identity verification.

## Identity and Access Management (IAM)
- Processes and tools for managing **user identities** and controlling access.
- Includes provisioning, authentication, and authorization.

## Multi-Factor Authentication (MFA)
- Requires **two or more forms of verification**:
  - Something you know (password)
  - Something you have (token or smart card)
  - Something you are (biometrics)

## Single Sign-On (SSO)
- Allows users to **authenticate once** and access multiple applications.
- Reduces password fatigue and administrative overhead.

## Authentication Protocols
- **RADIUS (Remote Authentication Dial-In User Service)**: Centralized AAA (Authentication, Authorization, Accounting) for network access.
- **LDAP (Lightweight Directory Access Protocol)**: Access and maintain distributed directory information (e.g., Microsoft Active Directory).
- **SAML (Security Assertion Markup Language)**: Exchanges authentication and authorization data for SSO.
- **TACACS+ (Terminal Access Controller Access Control System Plus)**: Cisco AAA protocol, separates authentication, authorization, and accounting.

## Time-Based Authentication
- Access controlled based on **time restrictions**, e.g., business hours or temporary access tokens.

## Authorization
- Determines **what an authenticated user is allowed to do**.
- Works together with authentication to enforce security policies.

## Least Privilege
- Users are given **only the access necessary** to perform their duties.
- Reduces risk if accounts are compromised.

## Role-Based Access Control (RBAC)
- Permissions assigned to **roles** rather than individuals.
- Users inherit permissions based on their role, simplifying management.

## Geofencing
- Controls access based on **geographic location**.
- Can allow or deny login attempts depending on physical or IP location.
