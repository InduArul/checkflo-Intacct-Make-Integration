✅ Checkflo ↔ Sage Intacct Integration via Make.com

This project demonstrates an end-to-end automation solution using **Make.com** to integrate **Checkflo** (a check disbursement platform) with **Sage Intacct** (a cloud-based ERP system).

It was designed to eliminate manual effort in invoice processing, file preparation, and status tracking — resulting in faster payouts, fewer errors, and full process transparency for the finance team.

---

## 🧩 What This Integration Does

- 📂 Reads batch numbers from an Excel tracker stored in SharePoint
- 🔄 For each batch, it retrieves posted checks and linked invoices via the Checkflo API
- 🔎 Searches for corresponding open bills in Sage Intacct via API
- ✅ Approves and pays the bills in Intacct using the transaction amount from Checkflo
- 📄 Generates a reconciliation file for all processed checks
- ☁️ Updates the reconciliation file back into SharePoint
- 📬 Emails the stakeholders with confirmation and attachments
- 🛡️ Fully equipped with error handling and exception logic to manage edge cases, failed lookups, and API timeouts

---

## 💼 Real-World Use Case

A mid-sized finance team was managing their Checkflo disbursements and Sage Intacct billing manually — copying batch numbers, cross-referencing checks with invoices, approving bills, and generating reconciliation files by hand.

The process was slow, error-prone, and involved multiple systems, spreadsheets, and people — every single time checks were issued.

This Make.com automation replaced all of that with a fully integrated solution that:
- Pulled batch check data from Checkflo
- Matched and paid corresponding bills in Intacct
- Generated a reconciliation file automatically
- Updated SharePoint records and emailed the finance team
- Handled errors gracefully with built-in exception logic

The result?
👉 80%+ time savings, zero manual errors, and a fully auditable, API-driven finance ops flow that now runs quietly in the background.

---

## 🛠 Tools & Technologies

- **Make.com (formerly Integromat)** — for workflow orchestration
- **Sage Intacct API** — to fetch and update billing data
- **SharePoint Excel Online** — for workbook and table updates
- **Email module / Storage upload** — for sending Checkflo files
- **Custom filters & conditions** — for error handling and dynamic logic

---

## 📁 Files Included

| File | Purpose |
|------|---------|
| `Make.com flow.json` | Exported scenario (Make.com flow blueprint) |
| `Checkflo_Payload_sample.json` | Sample webhook or invoice data (dummy data) |
| `/assets` | (screenshots of the flow, sample file formats, etc.) |
| `/docs/flow-description.md` | Detailed step-by-step explanation of the automation |

---

## 🔄 Workflow Overview

![Flow Diagram](assets/integration-diagram.png)

1. **Trigger:** Scheduled or webhook-based pull from Intacct  
2. **Transform:** Format data for Checkflo + write to Excel tracker  
3. **Conditionals:** Filter approved items, manage batch tracking  
4. **Action:** Generate CSV, email/upload it  
5. **Close Loop:** Update Intacct record post-payment

---

## 🔐 Security Notes

- All credentials are stored securely within Make.com and not exposed
- Client-identifying data and internal links have been redacted for open-source publishing

---

## 👋 About the Developer

Hi, I’m Indu — a freelance Automation Consultant & Builder with 6+ years of success on Upwork. I specialize in:
- AI Agents & No-Code Workflows  
- RPA with UiPath, Power Automate  
- Deep API Integrations & Data Automation

📬 Let’s automate your finance ops, CRM flows, or internal tools:  
👉 [Connect with me on Upwork]([https://www.upwork.com/freelancers/~yourprofilelink](https://www.upwork.com/freelancers/~01c1dc6f01258034ab))

---

## 📌 License

This repo is for portfolio and educational purposes. Please do not use in production without customizing and securing sensitive endpoints and flows.
