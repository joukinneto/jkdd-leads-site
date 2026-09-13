# 🎯 JKDD Leads — Public Website

**JKDD TECH — Product Website & Lead Acquisition Front End**

**Category:** Website / Public Web Presence  
**Lifecycle:** Development / Test Preview  
**Production:** Untouched unless separately authorized

---

## Purpose

This repository contains the public-facing website for **JKDD Leads**. Its role is presentation, product discovery and lead acquisition — not ownership of canonical lead, pipeline or CRM data.

The operational product and canonical lead workflows belong to the `jkdd-leads` application repository and the governed JKDD TECH architecture.

---

## Website responsibilities

- explain the JKDD Leads product clearly;
- present benefits, workflows and calls to action;
- collect or route approved lead-entry interactions;
- provide a fast, mobile-first public experience;
- support technical SEO and accessibility;
- remain lightweight and inexpensive to operate.

---

## Architecture boundary

### This website may

- present public marketing content;
- host approved forms or acquisition entry points;
- route visitors into governed JKDD Leads workflows;
- publish static product information.

### This website must not

- become the canonical lead database;
- recreate CRM pipeline ownership;
- duplicate authentication/security logic unnecessarily;
- expose private credentials or backend secrets;
- present planned capabilities as Production-ready.

---

## Hosting strategy

The current public-site strategy favors a zero-cost, static-first deployment compatible with **GitHub Pages** where technically appropriate.

Key principles:

- mobile-first;
- responsive layout;
- no paid hosting dependency for the initial public site;
- simple deployment and rollback;
- public assets only;
- no privileged credentials in client-side code.

---

## Relationship to JKDD Leads

| Concern | Canonical owner |
|---|---|
| Public product website | `jkdd-leads-site` |
| Lead acquisition / qualification product logic | `jkdd-leads` |
| Shared identity / security / tenant contracts | JKDD Foundation where applicable |
| Production activation | Separate governed release decision |

---

## Repository classification

Within the professional JKDD GitHub portfolio this repository belongs to:

**Websites & Public Web Presence → Product Websites → JKDD Leads**

It is intentionally separate from the JKDD Leads application source repository.
