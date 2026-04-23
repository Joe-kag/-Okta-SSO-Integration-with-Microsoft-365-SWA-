# Okta-SSO-Integration-with-Microsoft-365-SWA-
📌 Overview

This project demonstrates the implementation of Single Sign-On (SSO) using Secure Web Authentication (SWA) with Okta for access to Microsoft 365.

Instead of federation protocols (e.g., SAML), this setup uses credential-based authentication managed securely within Okta, enabling users to access Microsoft 365 applications from a centralized dashboard.

🏗️ Architecture
Okta → Identity Provider (Credential Manager)
Microsoft 365 → Target Application
Authentication Method → Secure Web Authentication (SWA)

Authentication Flow:

User logs into Okta
User selects Microsoft 365 from the Okta dashboard
Okta securely injects stored credentials into the login form
User gains access without manually entering credentials

<img width="1915" height="937" alt="Screenshot 2026-04-14 202952" src="https://github.com/user-attachments/assets/621f1f3a-a43d-46a4-b04e-f35607a46ed6" />


🛠️ Technologies & Concepts
Okta (SWA Application)
Microsoft 365
Secure Credential Storage
Access Management
Centralized Authentication
⚙️ Implementation Steps
🔹 1. Create SWA Application in Okta
Added Microsoft 365 as a Secure Web Authentication (SWA) application
Configured login URL for Microsoft 365
Enabled secure credential handling

<img width="1906" height="940" alt="365 provision" src="https://github.com/user-attachments/assets/e954b68e-14e5-4d50-bbad-fc3f894b96e8" />


🔹 2. Configure User Credentials
Stored user credentials securely within Okta
Mapped credentials to individual users
Ensured proper username/email alignment

<img width="1920" height="968" alt="Screenshot 2026-04-14 203736" src="https://github.com/user-attachments/assets/5790c871-1ba6-42a7-bdfb-c43060636607" />


🔹 3. Assign Users to Application
Assigned Microsoft 365 app to users in Okta
Verified access permissions
Ensured only authorized users could launch the app

<img width="1920" height="958" alt="Screenshot 2026-04-14 203656" src="https://github.com/user-attachments/assets/20a8f624-249e-4ad9-a30f-6b68487a613a" />


🔹 4. Testing & Validation
Logged into Okta dashboard
Launched Microsoft 365 via SWA
Verified automatic credential injection and successful login

<img width="1920" height="1080" alt="Screenshot 2026-04-14 204354" src="https://github.com/user-attachments/assets/9c98d9ed-3b26-4ce1-af22-0f7e5368bf3b" />


✅ Key Outcomes
Centralized access to Microsoft 365 via Okta
Eliminated repeated manual logins for users
Demonstrated secure credential handling using SWA
Implemented access control through user assignment
⚠️ Challenges & Resolutions
Credential Mismatch
Issue: Login failure due to incorrect stored credentials
Fix: Updated credentials in Okta to match Microsoft 365 account
Login Page Changes
Issue: SWA failed due to UI/login form changes
Fix: Adjusted configuration to match current login fields
User Access Issues
Issue: Users unable to launch application
Fix: Verified assignment and permissions in Okta
🚀 Future Enhancements
Transition to federated SSO (SAML or OIDC) for stronger security
Enforce Multi-Factor Authentication (MFA) in Okta
Implement group-based access control (RBAC)
Enable monitoring of authentication events
💡 Project Value

This project demonstrates practical experience with:

Secure Web Authentication (SWA)
Credential management and protection
Centralized access control using Okta
Real-world application access integration

It reflects an understanding of different SSO approaches and when to apply them based on environment constraints.

👤 Author

Joseph Kageche
Cybersecurity Analyst | Cloud & IAM Enthusiast.
