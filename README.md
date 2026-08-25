# AWS VPC Network Security Architecture

## 📌 Project Overview

This project demonstrates a layered AWS VPC network security architecture for an EC2 instance running inside a public subnet.

The architecture shows how internet traffic reaches an EC2 instance through multiple AWS networking components.

## 🏗️ Architecture

![AWS VPC Architecture](architectureaws-vpn-network-security.png
)

## 🔄 Traffic Flow

Internet User
↓
Internet Gateway
↓
Network ACL
↓
Route Table
↓
Security Group
↓
EC2 Instance

## 🔐 AWS Components

### 1. Internet Gateway
Provides communication between the VPC and the internet.

### 2. Network ACL
Controls traffic at the subnet level using IP addresses, protocols and ports.

NACLs are stateless.

### 3. Route Table
Determines where network traffic should be routed.

Example:

`0.0.0.0/0 → Internet Gateway`

### 4. Security Group
Acts as a virtual firewall for the EC2 instance and controls inbound and outbound traffic.

Security Groups are stateful.

### 5. EC2 Instance
Hosts the application and receives legitimate traffic after the network controls are applied.

## 🛡️ Security Benefits

- Controls inbound and outbound traffic
- Reduces unnecessary exposure
- Provides multiple layers of network control
- Helps prevent unauthorized access
- Supports defense-in-depth architecture

## 🚀 Key Learning

This project helped me understand how AWS networking components work together to control and secure traffic reaching an EC2 instance.

## 🛠️ Technologies

- AWS VPC
- Amazon EC2
- Internet Gateway
- Network ACL
- Route Tables
- Security Groups
-  web application 

## 📚 Conclusion

A secure AWS architecture should not depend on a single security control.

Combining routing, NACLs and Security Groups provides multiple layers of network protection.
