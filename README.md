# Deployment-of-a-HIPAA-compliant-hospital-management-application-on-the-Azure-platform.
We created a secure application by integrating advanced cloud operations that enhances patient care, providing seamless access to medical information and emphasizing the importance of confidentiality and data integrity.

Name: Nicole Udochukwu

Project Title: Hospital Management System Deployment on Azure Cloud Platform

Start Date: 2nd July 2024

End Date: 

Role: Cloud Security Engineer

GitHub Link:

Description:

I spearheaded the development of a cutting-edge hospital management system, leveraging a three-tier architecture to ensure compliance with healthcare data standards on the Azure Cloud Platform. We carefully crafted a scalable and secure environment, integrating Azure Virtual Machines, Azure Virtual Network, and Azure Network Security Groups to provide a robust foundation. I oversaw the design and implementation of the frontend, utilizing Node.js, React.js, and JavaScript to deliver a seamless user experience.

We developed a robust backend using Java, JDK 17, and Maven, and implemented a secure managed database solution using Azure SQL Database. Throughout the project, I ensured adherence to the highest security standards, utilizing Azure DevOps for CI/CD, conducting thorough code reviews, and performing regular security audits. By implementing multiple measures to protect patient data and maintain the integrity of the application, we achieved a secure and compliant hospital management solution.

Key Features
* User Authentication and Role Management: Implemented Azure Active Directory for secure user authentication, allowing role-based access control to ensure that sensitive data is only accessible to authorized personnel.

* Data Encryption: Utilized Azure's built-in encryption features for data at rest and in transit, ensuring that patient information is protected against unauthorized access.

* Audit Logging: Integrated comprehensive logging mechanisms to track user activities and system changes, facilitating compliance with healthcare regulations and enabling 
  quick incident response.

* Responsive Design: Ensured the frontend application is fully responsive, providing an optimal user experience across various devices, including desktops, tablets, and 
  smartphones.

Tools and Technologies 

* Git/GitHub: Version control for managing the codebase for both backend and frontend applications.
* Draw.io: Created visuals of the three-tier architecture, illustrating interactions between frontend, backend, and database components.
* Jira: Project management tool for tracking development and deployment phases.
* Slack: Facilitated efficient team communication and feedback exchange.
* Azure Active Directory: Managed identity and access, providing secure user authentication.
* Azure Network Security Groups: Controlled inbound/outbound traffic using defined security policies.
* Azure Virtual Machines: Hosted application in a scalable and secure environment.
* Azure DNS: Created DNS records for routing traffic using custom domain names.
* Public and Private IP: Assigned as necessary to ensure secure server communication.
* Port Configuration: Configured for seamless data exchange between servers.

Frontend Development Tools
* Node.js: JavaScript runtime for developing and running the frontend application.
* React.js: JavaScript library for building reusable UI components and managing state.
* JavaScript, HTML, CSS: Client-side scripting for web pages.
* NPM: Node Package Manager for managing project dependencies.

Backend Development Tools
* Java: Primary language for backend development.
* JDK 17: Java Development Kit for compiling and running applications.
* Maven: Dependency management and build automation for Java projects.

Database Management
* Azure SQL Database: Managed relational database service for data storage.
* Azure Data Studio: Efficient database connection and operation management.

Methodology
Developed a secure Hospital Management System in compliance with healthcare data standards, following Agile methodologies to ensure iterative development and continuous 
feedback.

Objective
Create a secure Hospital Management System compliant with healthcare data standards.

Infrastructure Setup

1. Resource Organization: Created an Azure resource group to manage related resources.

2. Virtual Network (VNet): Created a VNet with subnets for traffic segregation and security enhancement.

3. Network Security Groups: Configured Azure NSGs for access management.

4. Virtual Machines: Provisioned Azure VMs for frontend, backend, and database tiers, ensuring SSL/TLS encryption.
<img width="955" alt="virtual machines hipaa-azure A" src="https://github.com/user-attachments/assets/f8649fe2-a77d-4a56-a115-26e27888e6ed">

Database Creation and Server Configuration

== Azure SQL Database Configuration:
* Created Azure SQL Database instance with high availability.
* Enforced SSL connections for secure communication.

== Remote Connection Configuration:
* Allowed connections from specific IP addresses for added security.

== Peering Connection:
* Established private VNet peering between backend VM and Azure SQL Database for low-latency communication.
  
<img width="934" alt="Hipaa-azure 5" src="https://github.com/user-attachments/assets/28c47797-3f49-4f4f-874b-99c1c35b0bc7">
<img width="957" alt="hipaa-azure 9" src="https://github.com/user-attachments/assets/3bc8b1e0-c0cb-4bb1-830f-5a702ec56706">

== Validation and Testing:
* Verified the database connection using Azure Data Studio.

== Security Measures:
* Enabled Azure AD roles for access control.
* Implemented best practices for database user management.

Backend Creation and Configuration
==Network Security Configuration:
* Set up NSG rules allowing TCP traffic on relevant ports (e.g., 8080 for backend communication).

== Server Access:
* Used MobaXterm with private key access for secure server management.

== Setup Steps:
* Updated VM and installed JDK 17, Maven, and SQL Client.
  
  <img width="704" alt="hipaa-azure 6 A" src="https://github.com/user-attachments/assets/5bbda751-20df-4f69-84a7-f0734725eec2">

* Cloned backend code from GitHub and configured for deployment.
* Applied CORS security to restrict domain access.

== Application Deployment:
* Packaged and executed the application using Maven.
  
<img width="960" alt="hipaa-azure A" src="https://github.com/user-attachments/assets/3b46413e-0314-4ffb-84ed-8fd60aacc81a">

<img width="933" alt="706" src="https://github.com/user-attachments/assets/a90572e3-a8cb-4221-893a-10c75000b041">

== Security Measures:
* Closed unnecessary ports and restricted backend server access.

Frontend Creation and Server Configuration
== Network Security Configuration:
* Set up NSG rules allowing TCP traffic on relevant ports (e.g., 3000 for frontend access).

== Server Access:
* Utilized MobaXterm with private key access for secure server management.

== Setup Steps:
* Updated VM with the latest security patches.
* Installed Node.js and npm for frontend development.
* Cloned frontend code from GitHub and configured with the latest version.
* Ensured communication between frontend and backend servers on port 8080.
* Verified the application functionality and secure backend connection.
  
<img width="943" alt="hipaa-azure 4 A" src="https://github.com/user-attachments/assets/668d808b-d0cc-436f-9cfb-f09325d43d98">

== Application Testing and Deployment:
* Conducted thorough testing to ensure functionality.
  
<img width="945" alt="703" src="https://github.com/user-attachments/assets/a7e1d3a8-4fb0-4467-b726-fc076fb0c59d">

<img width="909" alt="701" src="https://github.com/user-attachments/assets/0b33d00f-fc34-4ada-94f8-4189bfc86fc1">


== Security Measures:
* Closed unnecessary ports and restricted frontend server access.

DNS Configuration with Azure DNS
* Domain Purchase: Purchased a domain from a domain registrar specifically for the hospital management system.
* DNS Settings:
== Logged into the Azure Portal and navigated to the Azure DNS section.
== Created a DNS zone for the purchased domain to manage DNS records efficiently.

*Added the following records:
== A Record: Configured to point to the public IP address of the frontend Virtual Machine, ensuring that traffic is directed to the correct server.
== CNAME Record: Set up for any necessary subdomains (e.g., www) to allow users to access the application through multiple entry points.

* Propagation Check: Utilized online tools to verify DNS propagation, ensuring that the domain was resolving correctly to the application and confirming proper 
  connectivity.

* Security
Azure DevOps: Analyzed code for potential security vulnerabilities.
Code Reviews: Conducted to ensure compliance with security best practices.
Regular Security Audits: Performed to identify and address potential security risks.
Incident Response Plan: Developed a comprehensive incident response plan to address potential security breaches swiftly and effectively.
