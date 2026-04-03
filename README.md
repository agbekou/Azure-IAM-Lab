# Azure-IAM-Lab

### Objective
To establish a secure identity foundation within a Microsoft Azure environment by configuring User Identities and implementing Role-Based Access Control (RBAC). 

### Core goal
The core goal was to mitigate the risk of credential compromise by enforcing the **Principle of Least Privilege (PoLP)** and reducing the potential "blast radius" within the cloud infrastructure.

### **Skills Learned**
* **Identity & Access Management (IAM):** Designing and managing cloud-based user identities.
* **Role-Based Access Control (RBAC):** Understanding the hierarchy of permissions and scope (Subscription vs. Resource Group).
* **Cloud Security Governance:** Applying the Principle of Least Privilege (PoLP) to administrative roles.
* **Administrative Efficiency:** Using built-in Azure roles to streamline security operations.

### **Tools Used**
* **Microsoft Azure Portal**
* **Microsoft Entra ID** (formerly Azure Active Directory)
* **Azure RBAC Engine**

### **Steps Taken**

#### **1. Identity Provisioning**
Created unique user accounts within Microsoft Entra ID. This step established the "Who" of the environment, ensuring every action can be audited back to a specific identity rather than using shared administrative accounts.


![Azure AIM](https://github.com/user-attachments/assets/2dc9d0cd-76f5-4030-b86a-07e7ca5ab7b2)



#### **2. Defining Administrative Scope**
Identified the specific resources and management groups requiring oversight. Instead of granting broad access, I defined the boundaries where specific permissions were necessary to prevent unauthorized lateral movement.

#### **3. Role Assignment & Implementation**
Assigned specific administrative roles (e.g., Global Administrator, User Administrator, or Contributor) based on the tasks required for each user.

![Azure IAM 2](https://github.com/user-attachments/assets/7a6cb404-8f2e-41ad-b095-1b62ce75c905)


#### **4. Enforcing the Principle of Least Privilege (PoLP)**
Audited the assigned roles to ensure users were granted only the access necessary to perform their functions. This involved opting for "granular" roles over "broad" roles to ensure that if a credential were compromised, the attacker’s access would be strictly limited.

![Azure IAM](https://github.com/user-attachments/assets/df7d175c-2c5e-4eef-9b05-1ae185c5dc6b)


#### **5. Verification & Validation**
Tested the access levels by logging in as the newly created users to verify that they could perform their assigned duties but were restricted from unauthorized configurations, effectively validating the security perimeter.
