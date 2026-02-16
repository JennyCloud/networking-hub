# Cloud Networking Concepts

## 1. Network Functions Virtualization (NFV)

**Definition:**  
Network Functions Virtualization (NFV) replaces traditional hardware-based network devices with software-based virtual appliances.

Instead of using physical devices like:
- Firewalls
- Routers
- Load balancers
- WAN optimizers

NFV runs these as virtual machines in a cloud or data center.

**Why it matters:**
- Reduces hardware cost
- Improves scalability
- Enables rapid deployment
- Centralized management

**Example:**
A virtual firewall running inside a cloud environment instead of a physical firewall appliance.

---

## 2. Virtual Private Cloud (VPC)

**Definition:**  
A Virtual Private Cloud (VPC) is a logically isolated virtual network within a public cloud environment.

It allows organizations to:
- Define their own IP address ranges
- Create subnets
- Configure routing tables
- Apply security rules

**Key Characteristics:**
- Isolation from other tenants
- Custom network configuration
- Control over traffic flow

**Example:**
An AWS VPC or Azure Virtual Network (VNet).

---

## 3. Network Security Groups (NSGs)

**Definition:**  
A Network Security Group (NSG) is a virtual firewall that controls inbound and outbound traffic to cloud resources.

NSGs filter traffic based on:
- Source IP
- Destination IP
- Port number
- Protocol (TCP/UDP)
- Direction (inbound/outbound)

**Purpose:**
- Enforce access control
- Restrict unauthorized traffic
- Protect virtual machines and services

**Example:**
Allowing only TCP port 443 (HTTPS) to a web server VM.

---

## 4. Cloud Gateways

**Definition:**  
A cloud gateway connects a cloud environment to external networks such as:
- On-premises networks
- Other cloud environments
- Remote users

**Types:**
- VPN Gateway (encrypted tunnel over internet)
- Direct Connect / ExpressRoute (private dedicated connection)

**Purpose:**
- Enable hybrid networking
- Secure communication between environments
- Extend internal networks to the cloud

**Example:**
A site-to-site VPN connecting a company’s office network to its cloud VPC.

---

## 5. Cloud Deployment Models

### Public Cloud
- Owned and operated by a third-party provider
- Resources shared among multiple customers
- Accessed over the internet

**Example:** AWS, Azure, Google Cloud

---

### Private Cloud
- Dedicated to a single organization
- Can be hosted on-premises or by a provider
- Greater control and customization

---

### Hybrid Cloud
- Combination of public and private cloud
- Allows data and applications to move between environments

**Benefit:**
Flexibility and scalability while maintaining control over sensitive workloads.

---

## 6. Cloud Service Models

### Infrastructure as a Service (IaaS)
Provides virtualized computing resources over the internet.

You manage:
- Operating system
- Applications
- Data

Provider manages:
- Physical hardware
- Networking infrastructure

**Example:** Virtual machines in Azure or AWS.

---

### Platform as a Service (PaaS)
Provides a platform for developing and deploying applications.

You manage:
- Applications
- Data

Provider manages:
- OS
- Runtime
- Infrastructure

**Example:** Azure App Service, AWS Elastic Beanstalk.

---

### Software as a Service (SaaS)
Provides fully managed software accessible via browser or client app.

You manage:
- User settings
- Data input

Provider manages:
- Everything else

**Example:** Microsoft 365, Google Workspace, Salesforce.

---

# Summary

NFV = Virtualized network devices  
VPC = Isolated virtual network in cloud  
NSG = Virtual firewall rules  
Cloud Gateway = Connects cloud to external networks  
Deployment Models = Public, Private, Hybrid  
Service Models = IaaS, PaaS, SaaS  

Understanding these concepts connects traditional networking with modern cloud architecture.
