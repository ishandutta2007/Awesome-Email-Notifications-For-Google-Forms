# Awesome-Email-Notifications-For-Google-Forms

# Top Email Notifications for Google Forms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Form Submission Alerts, Approval Workflows & Personalized Email Automation*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Email Notifications for Google Forms**. These tools enable anyone to send personalized, automated emails when a Google Form is submitted—from simple respondent confirmations to multi-step approval chains with conditional routing.

**Examples** include Email Notifications for Google Forms, Form Mule, Form Director, Form Approvals, BoloForms, Form Publisher, Automate.io, Make, Zapier, and Sheetgo (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, Google Apps Script automation, and open workflow platforms—ideal for teams, educators, and developers seeking transparent, vendor-independent form notification solutions.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Form Mule (New Visions Cloudlab)](https://www.newvisions.org/formmule)**  
  Popular Google Sheets add-on for turning form responses into personalized emails. Supports **up to 15 different email templates**, each with its own send conditions based on form responses . Uses column headers as merge tags for personalization—subject lines and body can pull unique data per recipient . Triggers include form submission, time-based, or manual execution . Tracks send status in a dedicated sheet column to prevent duplicates .

- **[Form Approvals](https://formapprovals.com/)**  
  Google Forms add-on purpose-built for approval workflows. **Sequential multi-step approvals** where each approver is notified only after the previous one responds . Features **AI Form + Workflow Builder**—describe your process in natural language and it generates the Google Form with approval routing, conditional logic, and quorum settings automatically . Dynamic and static recipients can be mixed (e.g., manager from form field, finance team fixed). Real-time dashboard for tracking pending approvals .

- **[BoloForms Approvals](https://approval-docs.boloforms.com/)**  
  Google Forms add-on for multi-level approval workflows. Features **role-based workflows** (Approver, Receive a Copy, Send Final Email Only), **conditional logic** so approvers only receive relevant requests, and **one-click approvals** from notification emails . Custom dashboard tracks all approvals from a single place. Data stored in your spreadsheet with end-to-end encryption .

- **[Form Publisher](https://form-publisher.com/)**  
  Generates documents (PDFs, Docs, Sheets, Slides) from Google Forms submissions with branded notifications. Free tier: 20 submissions/month, 1 user, unlimited approvers. Paid tiers unlock unlimited submissions and unbranded notifications . Features include multi-template generation, dynamic recipients/approvers, and legally compliant eSignature .

- **[Form Director](https://workspace.google.com/marketplace)**  
  Google Forms add-on for directing form submissions to multiple recipients with conditional logic and email notifications.

- **[Sheetgo](https://www.sheetgo.com/)**  
  Workflow automation platform connecting Google Sheets with approval workflows. Features **form approval**—activate "Require approval for form responses" and approvers receive email with approve/reject buttons . Approved responses are added to the master sheet automatically. Use cases include budget requests, time-off approvals, and HR workflows .

- **[Zapier](https://zapier.com/)**  
  Workflow automation platform with Google Forms triggers. Zaps can send emails (Gmail, Email by Zapier) when a new form response is created, optionally creating a spreadsheet row first . No coding required; 1.5-minute setup for simple flows .

- **[Make (Integromat)](https://make.com/)**  
  Visual workflow automation with Google Forms trigger. Supports **AI Toolkit integration**—use Make AI Toolkit to generate personalized email content from form responses before sending via Gmail . Filters prevent errors when no new submissions exist .

- **[Automate.io](https://automate.io/)**  
  Workflow automation platform (acquired by Notion) with Google Forms email notification integrations.

- **[Google Forms Email Notifications (built-in)](https://developers.google.cn/workspace/add-ons/editors/forms/quickstart/forms-notifications)**  
  Native Google Forms feature for email notifications to form creator. Configurable via the three-dot menu. For notifications to multiple recipients, add-ons like Form Notifier are required .

## Open-Source GitHub Projects

- **[Automatic Formatted Mail Sending by Google Apps Script](https://github.com/saidulislam00/Automatic-Formatted-Mail-Sending-by-Google-Apps-Script)**  
  Open-source Google Apps Script for automating email notifications triggered by Google Forms submissions. Features **dynamic email templates using Google Docs**—customize content with merge fields. **Status logging** tracks sent emails in the corresponding Google Sheet . Simple setup and seamless integration with Google Workspace tools. **The most practical open-source starting point for custom Google Forms email automation.**

- **[Ikiform](https://peerlist.io/preetsuthar17/project/ikiform)**  
  Open-source, AI-native alternative to Google Forms (built with Next.js, Supabase, Upstash). Features **email notifications** on form submission, AI form builder, AI analytics, rate limiting, and form customization . **A complete open-source replacement** rather than an add-on—ideal for teams wanting full control over the form platform itself.

- **[OhMyForm](https://research.tedneward.com/presentation/ohmyform.html)**  
  Open-source form builder positioned as alternative to TypeForm, TellForm, and Google Forms. Features **customizable notifications on form submission**, **webhooks on form submission**, multi-language support, 11 question types, and export to XLS/JSON/CSV . Deployable with Heroku and DockerHub. PostgreSQL and SQLite support. **The most feature-complete open-source form platform with native notification support.**

- **[n8n Google Forms Workflows](https://n8n.io/workflows/)**  
  Open-source workflow automation platform (Sustainable Use License) with community-contributed Google Forms templates. **Automated Lead Response** template sends personalized confirmation to leads and notifies internal team—runs every minute watching the linked Google Sheet . **Instant Gmail Notifications** template sends clean, readable email within a minute of form submission . Self-hostable, no per-task fees.

- **[Email Automation KPIs (Make + Power BI)](https://github.com/Adriano-goes/email-automation-kpis)**  
  Open-source reference architecture connecting Google Forms → Google Sheets → Make → Gmail → Power BI. **Logs email success/failure to Automation_Log sheet** with error details (SMTP Error, Invalid Recipient, Quota Exceeded) . Power BI dashboard visualizes KPIs: total emails sent, success rate, failure rate, average per day, unique recipients . **The most complete open-source pattern for monitoring and measuring email notification reliability.**

- **[Google Apps Script Form Notifications](https://developers.google.cn/workspace/add-ons/editors/forms/quickstart/forms-notifications)**  
  Official Google sample code for building Form add-ons that send email notifications. Features **creator notification** (configurable response step—e.g., every 10 responses), **respondent notification** (confirmation to submitter), and **re-authorization alerts** capped at one per day . Uses `MailApp.sendEmail()` with quota awareness. **The canonical reference implementation for Google Forms email notifications.**

### Additional Strong Open-Source Options

- **[Form Notifier](https://workspace.google.com/marketplace)** — Google Forms add-on for sending notifications to multiple recipients beyond the form owner .
- Community **n8n** workflows for multi-step approval routing and conditional email logic.
- Community **Google Apps Script** snippets for time-triggered digest emails (batch notifications instead of per-submission).

**Frameworks for building custom systems**: Combine **Automatic Formatted Mail Sending** for dynamic Doc-based templates with **n8n** for workflow orchestration and conditional routing, **Email Automation KPIs** for delivery monitoring, and **Google Sheets** as the data layer—creating a fully self-hosted, observable Google Forms email notification system.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Email notification systems handling form responses must comply with Google Workspace acceptable use policies, data protection regulations (GDPR, CCPA, etc.), and CAN-SPAM requirements.
- **Open-source Google Forms automation is mature via Apps Script.** The official Google sample provides production-grade patterns for creator notifications, respondent confirmations, and re-authorization handling . GitHub projects like saidulislam00/Automatic-Formatted-Mail-Sending extend this with Doc-based templates and status logging . **The primary constraint is Google's MailApp daily quota**—notifications are capped by your Workspace tier.
- **Add-ons dominate the approval workflow space.** Form Approvals, BoloForms, and Sheetgo all provide multi-step approval chains with conditional routing . **Open-source alternatives for approval workflows are limited**—Apps Script can be extended, but requires custom development.
- **Self-hosted form platforms offer full control.** Ikiform and OhMyForm provide complete form builders with native notification support . **Choose this path when you need data sovereignty or want to avoid Google Workspace dependency entirely.**
- Self-hosted open-source solutions require proper security hardening, email deliverability configuration, and ongoing maintenance. Form data may contain PII—ensure storage and transmission comply with applicable regulations.

---

**Made for teams, educators, operations managers, and developers building transparent form notification solutions.**  
Let's make Email Notifications for Google Forms more open, data-driven, and reliable.
