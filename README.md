# Azure-Entra-ID-IAM-Lab-2-Single-Sign-On-SSO-
This lab demonstrates hands-on experience with **Identity and Access Management (IAM)** in Azure Entra ID, focusing on **Single Sign-On (SSO)** using **SAML** and **OIDC**.   The lab covers configuring test applications, assigning users and groups, and understanding authentication flows.

---

## Lab Objective
- Configure SAML-based SSO for a test application
- Configure OIDC-based SSO for a modern application
- Assign users and groups to applications
- Understand authentication flows (SAML assertions, OIDC ID tokens)

---

## SAML Lab

### Steps Completed

1. Created a **non-gallery enterprise application**: IAM-SAML-Test-App  
<img width="1376" height="682" alt="01-saml-app-created" src="https://github.com/user-attachments/assets/d7f6efc4-0ae4-4cd1-a1a9-d6416b97c17d" />


2. Configured **SAML SSO**:
     - Identifier (Entity ID)
     - Reply URL (ACS URL)  
   Verified **user attributes & claims** (UPN, name, email) 
<img width="1037" height="610" alt="02-saml-basic-config" src="https://github.com/user-attachments/assets/4c6d8fd3-106f-4065-95a0-4be169a21153" />

3. Assigned **users and groups** to the application
<img width="1607" height="448" alt="03-saml-user-assignment" src="https://github.com/user-attachments/assets/61753900-221d-45c0-aa87-371ca776c31a" />

4. Reviewed **certificate thumbprint** (used to sign SAML assertions)
<img width="708" height="360" alt="04-saml-cert" src="https://github.com/user-attachments/assets/c0f3dcfb-6b5e-4eea-b911-5fac1479d997" />

### Notes
- Federation metadata is available and was reviewed conceptually
- Tenant ID and any secrets were **not included**
- This demonstrates understanding of SAML authentication flows in Azure

---

## OIDC Lab

### Steps Completed
1. Registered a **new OIDC app**: IAM-OIDC-Test-App
<img width="932" height="394" alt="05-oidc-app-overview" src="https://github.com/user-attachments/assets/4b5093d1-cced-4c3c-b611-8b4760988f1e" />

2. Configured **authentication settings**:
   - Redirect URI
   - ID tokens enabled
<img width="1078" height="964" alt="06-oidc-auth-config" src="https://github.com/user-attachments/assets/aafe4ec1-0377-4445-a8d8-abc2f65b52e7" />

3. Assigned **users and groups** to the app
<img width="1514" height="342" alt="07-oidc-user-assignment" src="https://github.com/user-attachments/assets/dc51742d-e105-4e7b-9e4c-3bd0e8bb7be9" />

4. Reviewed OIDC concepts (ID tokens, claims) conceptually — **no live tokens were exposed**

### Notes
- No live ID tokens or secrets were generated for safety  
- Demonstrates understanding of modern authentication flows and app-level access control

---

## Lessons Learned
- SAML and OIDC are core protocols for enterprise SSO  
- Configuring test applications demonstrates authentication flow and claims mapping  
- Assigning users/groups shows authorization management in Azure Entra ID  
- Even free-tier labs can demonstrate professional IAM knowledge

---

## Safety Note
- All emails, tenant names, and sensitive identifiers in screenshots are **fake or blurred**  
- No client secrets, live tokens, or tenant IDs are exposed
