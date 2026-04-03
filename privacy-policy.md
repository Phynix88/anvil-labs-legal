# Privacy Policy — Time-to-Invoice for Jira

**Vendor:** Anvil Labs
**Last updated:** 2026-04-03

---

## 1. Introduction

Time-to-Invoice for Jira ("the App") is a Jira Cloud application developed by Anvil Labs and built on the Atlassian Forge platform. It reads Jira worklogs and creates invoices in QuickBooks, helping consulting firms and agencies turn tracked time into billable invoices without leaving Jira.

This Privacy Policy explains what data the App accesses, how it is used and stored, and what rights you have as a user or administrator.

---

## 2. Data We Collect

The App accesses the following data from your Jira instance:

- **Jira worklogs** — time entries including duration, start time, and the associated issue
- **Issue data** — issue keys, summaries, and project associations
- **Project data** — project names and keys, used to configure billing rules
- **User display names** — to identify who logged time on a given worklog

The App also stores configuration data you provide:

- QuickBooks connection settings (realm ID, company info)
- Project-level billing configuration (rates, customer mappings)
- Invoice records created by the App (for audit trail purposes)

The App does **not** collect passwords, email addresses, IP addresses, or any data beyond what is listed above.

---

## 3. How We Use Your Data

Data accessed by the App is used exclusively to:

- Read worklogs and assemble them into invoice line items
- Create invoices in your connected QuickBooks account
- Display worklog summaries and invoice history within the App UI
- Store your configuration so settings persist between sessions

We do **not** use your data for analytics, advertising, profiling, or any purpose other than the core invoice workflow described above.

---

## 4. Data Storage & Security

The App runs entirely on the **Atlassian Forge platform**, which means all compute and storage is hosted and managed by Atlassian. The App uses:

- **Forge KVS (Key-Value Store)** — for settings, project configurations, and invoice records. Data is scoped to your Atlassian site and inaccessible to other tenants.
- **Forge Secrets** — for storing QuickBooks OAuth tokens. Tokens are stored encrypted and are never exposed in logs or to the App's frontend.

No data is stored on Anvil Labs servers. Atlassian's infrastructure security, including encryption at rest and in transit, applies to all stored data. Atlassian's own privacy and security practices are documented at [atlassian.com/trust](https://www.atlassian.com/trust).

---

## 5. Third-Party Services

The only external services the App communicates with are:

- **QuickBooks Online (Intuit)** — to create invoices on your behalf, using OAuth 2.0 tokens you authorize. Data sent is limited to invoice line items derived from your worklogs.
- **Intuit OAuth endpoints** — for authenticating your QuickBooks connection.

No data is sent to any other third party. No analytics services, crash reporters, or tracking tools are used. The App contains no cookies and no external scripts — it runs inside Jira's sandboxed iframe environment.

---

## 6. Data Retention

- **Settings and project configurations** persist in Forge KVS until an administrator explicitly deletes them or uninstalls the App.
- **Invoice records** are retained indefinitely as an audit trail. Administrators can delete individual records through the App's interface.
- **QuickBooks OAuth tokens** are retained until you disconnect your QuickBooks account or uninstall the App, at which point they are deleted.

When the App is uninstalled from a Jira site, Atlassian's Forge platform garbage-collects all associated KVS data according to their data retention policies.

---

## 7. Your Rights (GDPR)

If you are located in the European Union or European Economic Area, you have the following rights under the General Data Protection Regulation (GDPR):

- **Access** — You may request a summary of what data the App holds about your site.
- **Correction** — You may update or correct configuration data directly within the App.
- **Deletion** — You may delete invoice records within the App, or uninstall the App to remove all stored data.
- **Portability** — Invoice records can be exported from the App interface.
- **Objection** — You may stop using and uninstall the App at any time.

To exercise these rights or submit a data-related request, contact us at the address in Section 9.

---

## 8. Changes to This Policy

We may update this Privacy Policy as the App evolves. When changes are material, we will update the "Last updated" date at the top of this document and, where appropriate, notify users through the Atlassian Marketplace listing. Continued use of the App after changes constitutes acceptance of the updated policy.

---

## 9. Contact

For privacy-related questions, data requests, or concerns:

**Anvil Labs**
Email: wefers.dominik@gmail.com

We aim to respond to all privacy inquiries within 5 business days.
