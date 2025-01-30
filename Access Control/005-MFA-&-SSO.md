# Multi-Factor Authentication (MFA)

Multi-Factor Authentication (MFA) is a security mechanism that requires users to provide two or more independent authentication factors to verify their identity before accessing a system, application, or network.

## MFA Factors: The Three Categories
MFA consists of three primary authentication factors. At least two of these must be used to complete authentication.

### A. Something You Know (Knowledge Factor)
This refers to information that only the user should know.

**Examples:**
- **Passwords** - A secret combination of characters set by the user.  
  - Example: Logging into a corporate email requires a strong password (e.g., `P@ssw0rd123`).
- **PIN (Personal Identification Number)** - A numeric code known only to the user.  
  - Example: ATM withdrawals require a 4 or 6-digit PIN after inserting a debit card.
- **Security Questions** - A pre-set question answered by the user for identity verification.  
  - Example: "What is the name of your first pet?"

### B. Something You Have (Possession Factor)
This includes physical or digital items the user owns and must use for authentication.

**Examples:**
- **Smart Cards** - A card with a microchip used for authentication.  
  - Example: Employees use a smart card to log into their work computer.
- **One-Time Passwords (OTP)** - A temporary, unique code generated for each login attempt.  
  - Example: Online banking systems send a 6-digit OTP via SMS or email.
- **Hardware Security Tokens** - A small physical device (USB or key fob) that generates OTPs or stores cryptographic keys.  
  - Example: YubiKey for logging into secure applications.
- **Authenticator Apps** - Mobile apps like Google Authenticator or Microsoft Authenticator generate time-sensitive OTPs.  
  - Example: A 30-second OTP is required for logging into a cloud service.

### C. Something You Are (Inherence Factor)
This includes biometric authentication based on the user’s unique physical traits.

**Examples:**
- **Fingerprint Recognition** - Uses fingerprint scans for authentication.  
  - Example: Unlocking a smartphone using a fingerprint sensor.
- **Iris or Retina Scans** - Scans the unique patterns in a person's iris or retina.  
  - Example: High-security government buildings use iris scanners for entry.
- **Facial Recognition** - Uses AI to match a user’s facial features with stored data.  
  - Example: Apple Face ID for unlocking an iPhone.
- **Voice Recognition** - Analyzes a person’s voice patterns to verify identity.  
  - Example: Some banks allow customers to authenticate via voice commands.

---

# Single Sign-On (SSO)
Single Sign-On (SSO) is an authentication process that allows users to log in once and gain access to multiple applications without needing to enter credentials again for each service. It improves convenience and security by centralizing authentication through an identity provider (IdP) like Okta, Microsoft Azure AD, or Google Workspace.

## Key Features:
- Shares one sign-in session across multiple systems.
- Avoids logging in multiple times.

**Example:**
- Logging into the **Intune portal** automatically signs the user into Microsoft Teams and Outlook without requiring additional login steps.
