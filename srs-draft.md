### 1. Introduction

**Product Overview**
The platform is an AI-powered, mobile-first financial management ecosystem tailored for the Egyptian market. It acts as a comprehensive digital accountant designed not just for individuals, but for entire households. By synchronizing family finances, the application empowers users to track expenses, manage both formal and informal debts, and achieve collective savings goals using an Autonomous Multi-Agent Financial System.

**Target Audience**

* **Individuals:** Users managing their personal daily income, subscriptions, and financial goals.
* **Families & Households:** Couples sharing joint budgets, and parents monitoring dependents through a secure, hierarchical sub-account structure.

### 2. Purpose

**Problem Statement**
Managing finances in Egypt often involves scattered data across physical cash, e-wallets, bank cards, and informal borrowing. Users struggle to track unrecorded peer-to-peer debts (money owed to or from friends and family), monitor household-wide spending, and manage formal bank installments without incurring penalties.

**Proposed Solution**
The application centralizes these fragmented financial channels. By utilizing localized data ingestion (SMS parsing, bilingual OCR, and Voice AI) and a Multi-Agent architecture, it transforms raw data into actionable intelligence. The system proactively tracks informal IOUs, optimizes debt repayment strategies for all liabilities, and provides holistic household financial visibility.

### 3. Scope

**In-Scope (System Capabilities)**

* **Household Financial Sync:** Hierarchical account management supporting primary users, partner linking (bi-directional sharing), and monitored kid accounts.
* **Personal Debt & IOU Tracking:** A dedicated ledger for logging informal debts owed to or from individuals (whether they are registered app users or external contacts), accompanied by AI-assisted repayment schedules.
* **Multi-Channel Ingestion:** Automated tracking via Egyptian bank/e-wallet SMS parsing, OCR receipt scanning, and AI voice notes.
* **AI Architecture:** Specialized autonomous agents (e.g., Budgeting, Debt Risk, Cash-Flow) supervised by a Verification Agent.

**Out-of-Scope (Current Phase constraints)**

* **Direct Money Transfers (e.g., Instapay Integration):** Due to strict central bank regulations and complex compliance requirements, executing direct peer-to-peer fund transfers is excluded from the current development phase. This feature is designated for a future roadmap pending official regulatory approval.
* **Direct Bank API Linking:** Financial data collection remains strictly analytical, relying on local device SMS parsing and manual uploads rather than live Open-Banking connections.

---
