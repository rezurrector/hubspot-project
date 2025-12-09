# HubSpot CMS Local Development & Deployment

This guide outlines how to set up your local HubSpot development environment, authenticate with multiple portals, and upload content using the HubSpot CLI.

---

## 1. HubSpot Developer Accounts

To get started, you’ll need HubSpot portals for development, staging, and production. You can create or access test accounts here:

- [HubSpot Developer Test Accounts](https://developers.hubspot.com/developer-test-accounts)  
- [My HubSpot Accounts](https://app-na2.hubspot.com/myaccounts)  
- [Sign up for HubSpot CRM](https://app.hubspot.com/signup-hubspot/crm?step=existing_user)

> Each portal requires its **own Personal Access Key (PAK)** for CLI authentication.

---

## 2. HubSpot CLI Authentication

Authenticate your local machine with each portal using:

```bash
hs auth

hs cms upload test-01 --account dev-portal
hs cms upload test-01 --account stage-portal
hs cms upload test-01 --account prod-portal
```