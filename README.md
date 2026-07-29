# 🛠️ E-Commerce & IT Help Desk - Jira Service Management Lab

## 📌 Project Overview
This repository contains a full-featured L1/L2 IT Help Desk and E-Commerce Support Desk simulation built using **Jira Service Management**. It demonstrates hands-on experience in incident triage, root cause analysis (RCA), identity and access management (IAM), web application troubleshooting, and API integration handling.

---

## 🛠️ Key Technical Incidents Handled

### 1. Network & Access Management | `KAN-6`
* **Issue:** User unable to connect to the corporate VPN from a remote location.
* **Root Cause:** Expired credentials in Active Directory / incorrect authentication format.
* **Resolution:** Forced credential reset via admin console and provided client re-configuration guidance.
* **Verification:** Confirmed successful VPN handshake and network drive mapping.

### 2. E-Commerce & API Integrations | `KAN-7`
* **Issue:** Web store orders failed to update inventory in the primary database.
* **Root Cause:** Expired Bearer API token on Shopify following a platform update.
* **Resolution:** Regenerated API Token in Shopify Developer Console and updated server environment variables.
* **Verification:** Processed test order (`#9999`); stock decremented accurately across systems.

### 3. Critical Web Infrastructure & Payments | `KAN-8`
* **Issue:** End-users encountered `HTTP 500 Internal Server Error` during checkout.
* **Root Cause:** Webhook call timeout to Stripe payment gateway under high traffic load.
* **Resolution:** Escalated to L2 to restart the payment worker service and adjusted timeout limits to 30 seconds.
* **Verification:** Payment logs confirmed `200 OK` status codes across subsequent transactions.

### 4. CMS & Web Front-End | `KAN-9`
* **Issue:** Promotional banners failing to render on mobile devices.
* **Root Cause:** Unsupported legacy image format (`.webp`) and unclosed HTML syntax in the CMS container.
* **Resolution:** Converted assets to `.png`, fixed inline HTML markup, and purged CDN cache.
* **Verification:** Cross-device inspection passed on Android and iOS viewports.

### 5. Identity & Access Provisioning (IAM) | `KAN-10`
* **Issue:** Onboarding request for new support agent from HR.
* **Root Cause:** Standard employee onboarding workflow.
* **Resolution:** Provisioned corporate email, assigned Microsoft 365 / Google Workspace licenses, and granted role-based access to Slack and Drive.
* **Verification:** Successful user login confirmed; welcome protocol completed.

---

## 📸 Documentation & Evidence
All workflow screenshots and detailed incident logs are available in the repository PDF document:
* **[View Full PDF Report][./Jira_Service_Management_Lab_Melissa_2.pdf](https://drive.google.com/file/d/1mB3-zvEFiPadJy61kMaJZ5SjcQx2T6Nw/view?usp=sharing)**
