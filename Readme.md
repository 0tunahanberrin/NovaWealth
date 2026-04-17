# NovaWealth: Payment Systems & Digital Wallet Orchestration 🚀

**NovaWealth** is a mobile banking and payment platform designed to combine different financial services into one ecosystem. This project is a practical application of the concepts I learned from my specializations:

* **FinTech: Foundations, Payments, and Regulations** – University of Pennsylvania
* **The Future of Payment Technologies** – University of Michigan

## 🏗️ Architectural Overview & Scope
The project covers the two main parts of the payment lifecycle: **Inflow (Funding)** and **Outflow (Processing)**. I followed global standards such as **PCI-DSS, ISO 8583, and EMV 3D Secure 2.0**.

### 1. Digital Wallet & Funding Infrastructure (Inflow)
This section focuses on moving funds from external bank accounts into the NovaWealth wallet safely.
* **Bank Transfers:** I managed the workflows for linking bank accounts and processing ACH/EFT settlement batches.
* **Risk Scoring:** The system runs a "Fraud and Risk Analysis" to give each transaction a risk score (Low, Medium, or High).
* **User Authentication:** Depending on the risk, the system uses Token Authentication or SMS/OTP codes to verify the user.

### 2. Payment Lifecycle & Gateway Operations (Outflow)
This part manages how a payment moves from the merchant to the final bank approval.
* **Tokenization:** I designed the flow where the "Tokenization Service" converts sensitive card data (PAN) into secure tokens for PCI-DSS compliance.
* **3D Secure 2.0 (RBA):** The system uses Risk-Based Authentication (RBA) and ACS (Access Control Server) cycles to provide a smooth user experience.
* **The Authorization Loop:** I mapped the message routing between the Merchant, Gateway, Acquirer, Card Scheme, and Issuer using ISO 8583 standards.
* **Clearing & Settlement:** The flow includes calculating Interchange Fees and the Merchant Discount Rate (MDR) before the final fund transfer.
* **Exception Handling:** I detailed the processes for **Void** (canceling a transaction) and **Refund** (returning money) to keep the balance correct.

## 🛠️ Methodology & Tools
* **Product Management:** I organized the project in **Jira** using Epics, User Stories, and Acceptance Criteria in the "Given/When/Then" format.
* **Process Modeling:** I used **BPMN 2.0** and flowcharts to show the technical steps of how money and data move through the system.
* **Technical Compliance:** The project integrates payment regulations like PSD2 and Open Banking concepts.

