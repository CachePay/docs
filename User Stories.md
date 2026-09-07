# Master Product Requirements Document: Features & User Stories

A comprehensive, consolidated repository of all functional features, user stories, and acceptance criteria across the personal finance and household wealth management platform.

---

## Table of Contents
1. [Feature 1: User Authentication, Account Lifecycle & Household Management](#feature-1-user-authentication-account-lifecycle--household-management)
   - [US 1.1: Primary Account Registration](#us-11-primary-account-registration)
   - [US 1.2: Kid Sub-Account Generation](#us-12-kid-sub-account-generation)
   - [US 1.3: Partner Account Dual Sharing](#us-13-partner-account-dual-sharing)
   - [US 1.4: Account Detachment & Privacy Protocol](#us-14-account-detachment--privacy-protocol)
   - [US 1.5: Forgot Password & Account Recovery for All Account Types](#us-15-forgot-password--account-recovery-for-all-account-types)
   - [US 1.6: Account Deletion & Data Wipe for All Account Types](#us-16-account-deletion--data-wipe-for-all-account-types)
   - [US 1.7: Card-Issued Sub-Account Detachment & Account Graduation](#us-17-card-issued-sub-account-detachment--account-graduation)
2. [Feature 2: Transaction Logging, Cash Management & Automated Ingestion](#feature-2-transaction-logging-cash-management--automated-ingestion)
   - [US 2.1: Manual Expense Logging with "Add Receipt Later" Tag](#us-21-manual-expense-logging-with-add-receipt-later-tag)
   - [US 2.2: Daily Cash Audit & Pocket Reconciliation Prompt](#us-22-daily-cash-audit--pocket-reconciliation-prompt)
   - [US 2.3: Quick Cash Balance Discrepancy Logging](#us-23-quick-cash-balance-discrepancy-logging)
   - [US 2.4: Multi-Criteria Transaction Filtering & Advanced Search](#us-24-multi-criteria-transaction-filtering--advanced-search)
   - [US 2.5: Historical Bulk Data Import (PDF / CSV / Excel)](#us-25-historical-bulk-data-import-pdf--csv--excel)
   - [US 2.6: Automated Bilingual Bank & E-Wallet SMS Parsing](#us-26-automated-bilingual-bank--e-wallet-sms-parsing)
   - [US 2.7: Physical Cash Wallet Synchronization via ATM Detection](#us-27-physical-cash-wallet-synchronization-via-atm-detection)
   - [US 2.8: AI Voice Note Expense Logging (Egyptian Arabic & English)](#us-28-ai-voice-note-expense-logging-egyptian-arabic--english)
   - [US 2.9: Bilingual OCR Receipt Scanning & Itemized Category Splitting](#us-29-bilingual-ocr-receipt-scanning--itemized-category-splitting)
   - [US 2.10: GPS Mini-Map Tagging on Transaction Arrival](#us-210-gps-mini-map-tagging-on-transaction-arrival)
3. [Feature 3: Smart Budgeting & Subscription Management](#feature-3-smart-budgeting--subscription-management)
   - [US 3.1: Custom Salary Cycle Budgeting](#us-31-custom-salary-cycle-budgeting)
   - [US 3.2: Real-Time Budget Utilization Alerts](#us-32-real-time-budget-utilization-alerts)
   - [US 3.3: Automated Subscription Detection](#us-33-automated-subscription-detection)
   - [US 3.4: Subscription Price Hike & Tier Change In-App Audit Report](#us-34-subscription-price-hike--tier-change-in-app-audit-report)
   - [US 3.5: Free Trial Expiration Tracker & In-App Cancellation Hub](#us-35-free-trial-expiration-tracker--in-app-cancellation-hub)
   - [US 3.6: Category-Level "Safe-to-Spend" Daily Burn Rate](#us-36-category-level-safe-to-spend-daily-burn-rate)
   - [US 3.7: Unused & Ghost Subscription Identification](#us-37-unused--ghost-subscription-identification)
   - [US 3.8: One-Tap Category Fund Splitting for Shared Bills](#us-38-one-tap-category-fund-splitting-for-shared-bills)
   - [US 3.9: Budget Carryover and Rollover](#us-39-budget-carryover-and-rollover)
4. [Feature 4: Financial Goal Planning & Savings Tracking](#feature-4-financial-goal-planning--savings-tracking)
   - [US 4.1: Multi-Cadence Savings Goals Setup & Calculation](#us-41-multi-cadence-savings-goals-setup--calculation)
   - [US 4.2: Savings Contribution & Fund Allocation Tracking](#us-42-savings-contribution--fund-allocation-tracking)
   - [US 4.3: Real-Time Goal Health & Variance Tracking](#us-43-real-time-goal-health--variance-tracking)
   - [US 4.4: Dynamic Goal Scenario Simulation & Strategy Adoption](#us-44-dynamic-goal-scenario-simulation--strategy-adoption)
   - [US 4.5: Goal Lifecycle Management & Contingency Handling](#us-45-goal-lifecycle-management--contingency-handling)
   - [US 4.6: Milestone Tracking & Predictive Progress Alerts](#us-46-milestone-tracking--predictive-progress-alerts)
5. [Feature 5: Smart Notifications & Alerts Engine](#feature-5-smart-notifications--alerts-engine)
   - [US 5.1: Escalated Multi-Stage Debt Deadline Notifications](#us-51-escalated-multi-stage-debt-deadline-notifications)
   - [US 5.2: Unusual Transaction & Anomaly Detection Security Warning](#us-52-unusual-transaction--anomaly-detection-security-warning)
   - [US 5.3: Real-Time Budget Exceeded Alert](#us-53-real-time-budget-exceeded-alert)
   - [US 5.4: Approaching Category Limit Alert](#us-54-approaching-category-limit-alert)
   - [US 5.5: Spending Velocity Spike Alert](#us-55-spending-velocity-spike-alert)
   - [US 5.6: Upcoming Bill and Utility Reminders](#us-56-upcoming-bill-and-utility-reminders)
   - [US 5.7: Upcoming Subscription Renewal Reminders](#us-57-upcoming-subscription-renewal-reminders)
   - [US 5.8: Predicted Low Balance and Cash Shortage Warning](#us-58-predicted-low-balance-and-cash-shortage-warning)
   - [US 5.9: Savings Goal Progress Milestone Notifications](#us-59-savings-goal-progress-milestone-notifications)
   - [US 5.10: Savings Goal Delay Alert](#us-510-savings-goal-delay-alert)
   - [US 5.11: Proactive Personalized AI Recommendation Nudges](#us-511-proactive-personalized-ai-recommendation-nudges)
   - [US 5.12: Automated Weekly Spending Summary Notification](#us-512-automated-weekly-spending-summary-notification)
   - [US 5.13: Automated Monthly Financial Report Notification](#us-513-automated-monthly-financial-report-notification)
   - [US 5.14: Multi-Channel Dispatch & In-App Notification Center](#us-514-multi-channel-dispatch--in-app-notification-center)
   - [US 5.15: Configurable Do-Not-Disturb (DND) Quiet Hours](#us-515-configurable-do-not-disturb-dnd-quiet-hours)
   - [US 5.16: Critical Alert DND Bypass](#us-516-critical-alert-dnd-bypass)
   - [US 5.17: Daily Notification Rate Limiting](#us-517-daily-notification-rate-limiting)
   - [US 5.18: Granular Notification Preference Toggles](#us-518-granular-notification-preference-toggles)
   - [US 5.19: Customizable Budget Trigger Thresholds](#us-519-customizable-budget-trigger-thresholds)
6. [Feature 6: Comprehensive Financial Reporting & Analytics](#feature-6-comprehensive-financial-reporting--analytics)
   - [US 6.1: Cash Flow & Net Savings Report](#us-61-cash-flow--net-savings-report)
   - [US 6.2: Category-Wise Spending Breakdown](#us-62-category-wise-spending-breakdown)
   - [US 6.3: Budget vs. Actual Spending Report](#us-63-budget-vs-actual-spending-report)
   - [US 6.4: Savings Goal Progress Tracking](#us-64-savings-goal-progress-tracking)
   - [US 6.5: Month-over-Month Comparison](#us-65-month-over-month-comparison)
   - [US 6.6: Recurring Subscription Detection Report](#us-66-recurring-subscription-detection-report)
   - [US 6.7: Top Merchants & Largest Transactions Report](#us-67-top-merchants--largest-transactions-report)
   - [US 6.8: Unusual Transaction Alerts Report](#us-68-unusual-transaction-alerts-report)
   - [US 6.9: Natural-Language Financial Query (AI Assistant)](#us-69-natural-language-financial-query-ai-assistant)
   - [US 6.10: Exportable Financial Reports (PDF / CSV)](#us-610-exportable-financial-reports-pdf--csv)
7. [Feature 7 & 8: AI Suite & Multi-Agent Financial System](#feature-7--8-ai-suite--multi-agent-financial-system)
   - [US 7.1: Natural Language Financial Queries](#us-71-natural-language-financial-queries)
   - [US 7.2: Human-in-the-Loop Agent Authorization](#us-72-human-in-the-loop-agent-authorization)
   - [US 7.3: AI Narrative Report Summarization](#us-73-ai-narrative-report-summarization)
8. [Feature 9: Card Debts & Installment Tracking](#feature-9-card-debts--installment-tracking)
   - [US 9.1: Zero-Interest Installment Tracking](#us-91-zero-interest-installment-tracking)
   - [US 9.2: Bank Rewards Net Benefit Calculator](#us-92-bank-rewards-net-benefit-calculator)
   - [US 9.3: Hybrid Risk Debt Optimization](#us-93-hybrid-risk-debt-optimization)

---

# Feature 1: User Authentication, Account Lifecycle & Household Management

### Overview
Manages multi-tier household account hierarchies, including primary administrator accounts, dual-sharing partner accounts, and parental-supervised kid sub-accounts. Governs registration, recovery, data detachment, card-linked independence, and GDPR-compliant deletion across all account types.

---

### US 1.1: Primary Account Registration
* **User Story:** As a new user, I want to register a primary account by providing my first name, last name, email, and password so that I can gain full access to all personal finance tracking tools, household management, and budget features.
* **Acceptance Criteria:**
  * **Given** a user is on the registration screen, **when** they submit their valid name, email, and password meeting security complexity rules, **then** a primary adult account is created with full administrative access to household management.
  * **Given** an email address that is already registered in the system, **when** the user attempts registration, **then** the system prevents account creation and displays a clear error with a login/password recovery link.

---

### US 1.2: Kid Sub-Account Generation
* **User Story:** As a primary parent account user, I want to generate an invitation link or a 6-character code so that I can set up a kid-friendly sub-account to monitor my child's spending.
* **Acceptance Criteria:**
  * **Given** the primary user is in household settings, **when** they generate a kid invitation, **then** a unique 6-character code is generated that expires after 48 hours.
  * **Given** the kid sub-account is activated via the code, **when** the child's phone receives transaction SMS messages, **then** the child's ledger is updated and the parent account receives alerts for any exceeded spend thresholds.

---

### US 1.3: Partner Account Dual Sharing
* **User Story:** As a primary user, I want an explicit toggle to share my primary finances with my partner so that my partner can have full bi-directional visibility into my transaction ledger, shared goals, and budgets.
* **Acceptance Criteria:**
  * **Given** a partner sub-account is connected to the household, **when** the primary user enables the "Share Primary Finances with Partner" toggle, **then** the partner account dashboard updates immediately to display the primary user's balances, categories, and transaction ledgers.
  * **Given** active dual sharing, **when** either user logs or edits a shared transaction, **then** the change reflects synchronously across both users' dashboards.

---

### US 1.4: Account Detachment & Privacy Protocol
* **User Story:** As a sub-account user, I want to detach my account from the household hierarchy so that I can maintain my privacy and retain my personal transaction history independently.
* **Acceptance Criteria:**
  * **Given** a sub-account is connected to a parent/household, **when** the sub-account initiates the detachment protocol and confirms with password/2FA, **then** the parent account immediately loses access to the sub-account's historical and future transactions.
  * **Given** detachment is completed, **when** the sub-account user logs in, **then** their account is converted into an independent standalone account with their personal transaction ledger intact.

---

### US 1.5: Forgot Password & Account Recovery for All Account Types
* **User Story:** As a user of any account type (Primary, Partner, or Kid Sub-Account), I want a dedicated password recovery flow tailored to my account privileges so that I can regain access if I forget my credentials.
* **Acceptance Criteria:**
  * **Given** a Primary or Partner account user who forgets their password, **when** they request a password reset via the login screen, **then** a secure, time-limited reset link or 6-digit OTP is dispatched to their verified email/phone number.
  * **Given** a Kid sub-account user without an email address who forgets their PIN/password, **when** they initiate recovery, **then** the app routes the reset approval to the primary parent account dashboard, allowing the parent to set a temporary PIN or authorize a new credential.
  * **Given** an invalid or expired reset token/OTP, **when** the user attempts submission, **then** the system denies the change and provides a prompt to request a fresh recovery code.

---

### US 1.6: Account Deletion & Data Wipe for All Account Types
* **User Story:** As a user of any account type, I want the ability to permanently delete my account and purge my personal data in accordance with privacy laws so that my financial history is not retained against my wishes.
* **Acceptance Criteria:**
  * **Given** a Primary account user initiates account deletion, **when** they confirm with password re-entry and complete a 2-step verification, **then** the system offers a final data export (JSON/CSV) and schedules the entire household hierarchy and financial ledger for permanent purging within 30 days.
  * **Given** a Partner account user requests deletion, **when** confirmed, **then** only their personal profile and unshared transactions are deleted, unlinking them from the primary account without destroying the primary user's data.
  * **Given** a Kid sub-account, **when** the primary parent initiates deletion from household settings (or when the child requests deletion with parent authorization), **then** the child sub-account profile and associated metadata are immediately deactivated and purged.

---

### US 1.7: Card-Issued Sub-Account Detachment & Account Graduation
* **User Story:** As a teen or kid sub-account user who has obtained my own independent bank card or reached legal age, I want to detach from my parent's account based on my card ownership so that I graduate to a full standalone account while keeping my accumulated financial history.
* **Acceptance Criteria:**
  * **Given** a sub-account user links a verified personal debit or prepaid card registered under their own legal name, **when** the user selects "Graduate / Detach Account with Personal Card", **then** the system initiates the independence workflow.
  * **Given** the graduation workflow is approved (with parent notification delivered for minor accounts), **when** the detachment clears, **then** the sub-account transitions into a standalone primary account, parent SMS monitoring and spend caps are removed, and all past personal transaction logs remain preserved in the newly graduated account.

---

# Feature 2: Transaction Logging, Cash Management & Automated Ingestion

### Overview
Provides an omnichannel financial recording engine that supports manual input with receipt deferral, daily physical cash reconciliation, discrepancy tracking, multi-criteria filtering, bulk file imports, and automated bilingual ingestion via SMS parsing, voice notes, OCR receipt scanning, and GPS geotagging.

---

### US 2.1: Manual Expense Logging with "Add Receipt Later" Tag
* **User Story:** As a user, I want to manually log a transaction and tag it to upload the receipt later so that I can quickly record an expense on the go without losing track of the missing documentation.
* **Acceptance Criteria:**
  * **Given** a user manually inputs an expense amount, date, and category, **when** they check the "Add receipt later" toggle and save, **then** the transaction is logged immediately in the ledger and marked with an eye-catching "Pending Receipt" status badge.
  * **Given** a transaction tagged with "Pending Receipt", **when** the user later opens the transaction details, **then** an "Attach Receipt" option is presented allowing instant camera capture or image upload to resolve the tag.

---

### US 2.2: Daily Cash Audit & Pocket Reconciliation Prompt
* **User Story:** As a user, I want to receive an end-of-day prompt to verify my physical cash so that my app's cash wallet stays perfectly synced with the actual money in my pocket.
* **Acceptance Criteria:**
  * **Given** the optional daily cash audit prompt is enabled in user settings, **when** the scheduled end-of-day notification triggers (e.g., "Does your physical cash match 500 EGP?"), **then** the user is presented with a 1-tap "Confirm Balance" action and a "Quick Adjust" route.
  * **Given** the user selects "Confirm Balance", **when** tapped, **then** the app marks today's cash audit as reconciled with a timestamp in the audit log.

---

### US 2.3: Quick Cash Balance Discrepancy Logging
* **User Story:** As a user, I want to manually adjust my physical cash balance so that any lost or unrecorded money is automatically calculated and balanced in my ledger.
* **Acceptance Criteria:**
  * **Given** the user navigates to the physical cash wallet and selects "Adjust Cash Balance", **when** they input the actual physical cash currently in hand, **then** the system calculates the variance between recorded balance and actual count.
  * **Given** a calculated variance, **when** confirmed by the user, **then** the application automatically generates a balancing transaction categorized under "Cash Discrepancy / Uncategorized Cash" and updates the cash balance to match reality.

---

### US 2.4: Multi-Criteria Transaction Filtering & Advanced Search
* **User Story:** As a user, I want to search my ledger using combined criteria so that I can quickly pinpoint a specific transaction from my past.
* **Acceptance Criteria:**
  * **Given** the user opens the ledger filter engine, **when** they apply a combined search using vendor keywords, specific date intervals, payment methods (cash, card, e-wallet), categories, and minimum/maximum monetary amount ranges, **then** the app instantly filters the ledger to display only transactions matching all specified criteria.
  * **Given** active filter criteria yielding zero results, **when** evaluated, **then** the app displays an empty state with a 1-tap "Reset Filters" action.

---

### US 2.5: Historical Bulk Data Import (PDF / CSV / Excel)
* **User Story:** As a user, I want to upload bank statements or spreadsheets so that I can populate my transaction history without manually entering past data.
* **Acceptance Criteria:**
  * **Given** the user accesses the data import hub, **when** they upload a bank statement in PDF format or a CSV/Excel transaction spreadsheet, **then** the ingestion engine parses columns (Date, Merchant, Inflow/Outflow Amount, Reference).
  * **Given** the parsed rows are presented on an import preview screen, **when** the user reviews mappings and taps "Confirm Import", **then** all valid transactions are recorded in the ledger with duplicate detection applied against existing records.

---

### US 2.6: Automated Bilingual Bank & E-Wallet SMS Parsing
* **User Story:** As a user, I want the application to automatically read my bank and e-wallet SMS notifications in Arabic and English so that my expenses and ATM withdrawals are recorded without manual entry.
* **Acceptance Criteria:**
  * **Given** the app has SMS reading permissions enabled on an Android device, **when** a transaction SMS arrives from a supported Egyptian bank or telecom e-wallet (in Arabic or English), **then** the engine automatically extracts the transaction amount, currency, merchant/vendor name, transaction date/time, and card/account identifier.
  * **Given** successfully extracted data, **when** processed, **then** the transaction is added to the ledger under the smart inferred category with zero manual typing required.

---

### US 2.7: Physical Cash Wallet Synchronization via ATM Detection
* **User Story:** As a user, I want ATM withdrawals detected via SMS to automatically credit my Physical Cash Wallet balance so that my app reflects the physical money I have on hand.
* **Acceptance Criteria:**
  * **Given** the user receives an incoming bank SMS indicating an ATM cash withdrawal, **when** the SMS parsing engine detects the ATM withdrawal transaction type, **then** the bank account ledger logs a debit and the Physical Cash Wallet is automatically credited by the exact withdrawal amount.
  * **Given** the cash balance updates, **when** the user opens their wallet overview, **then** an event notification confirms: "ATM withdrawal detected: Cash wallet credited with [Amount]".

---

### US 2.8: AI Voice Note Expense Logging (Egyptian Arabic & English)
* **User Story:** As a user, I want to record short voice notes in Egyptian Arabic or English summarizing my daily spending so that the app can extract and log multiple transactions at once.
* **Acceptance Criteria:**
  * **Given** the user taps the microphone button, **when** they speak an expense summary under 60 seconds (e.g., "دفعت 150 جنيه في السوبرماركت و 50 جنيه بنزين"), **then** the speech-to-text and NLP pipeline parses the audio into structured line items with merchant, amount, date, and category.
  * **Given** parsed voice items, **when** processing finishes, **then** the app displays a batch confirmation sheet allowing the user to review, modify, and confirm all extracted transactions with one tap.

---

### US 2.9: Bilingual OCR Receipt Scanning & Itemized Category Splitting
* **User Story:** As a user, I want to upload Arabic or English receipts so that the computer vision model can extract itemized line prices and allow me to split the total across different sub-categories.
* **Acceptance Criteria:**
  * **Given** a user captures or uploads an image of an Arabic or English paper receipt, **when** the optical character recognition (OCR) model analyzes the image, **then** it extracts the merchant name, total tax, date, and individual line items with their item prices.
  * **Given** itemized receipt lines, **when** the user accesses the split screen, **then** the UI enables them to assign individual items or subsets of items to different expense categories (e.g., Groceries vs. Household supplies) before saving.

---

### US 2.10: GPS Mini-Map Tagging on Transaction Arrival
* **User Story:** As a user, I want the app to tag my GPS location the exact moment a bank SMS arrives so that I can identify cryptic or generic vendor names using a map.
* **Acceptance Criteria:**
  * **Given** location permissions are granted, **when** an incoming transaction SMS is parsed in real time, **then** the app captures current GPS coordinates and generates an interactive mini-map pin attached to the transaction details page.
  * **Given** a transaction with attached location metadata, **when** the user inspects the transaction, **then** an interactive map card displays the physical purchase location and nearest reverse-geocoded address.

---

# Feature 3: Smart Budgeting & Subscription Management

### Overview
Enables users to align budget resets with actual payroll cadences, monitor live utilization meters, forecast daily safe-to-spend limits, handle rollover balances, split shared bills, detect recurring subscriptions, and manage free trial expirations and price hikes via an in-app audit hub.

---

### US 3.1: Custom Salary Cycle Budgeting
* **User Story:** As a user, I want to align my category budget reset dates with my specific paycheck schedule so that my budget cycles match my actual cash flow rather than rigid calendar months.
* **Acceptance Criteria:**
  * **Given** a user is configuring or editing a budget, **when** they select a custom date range or pay schedule (e.g., 28th of every month, every other Thursday, or bi-weekly), **then** the budget utilization tracking and progress meters reset on that designated cycle start date.
  * **Given** a mid-cycle update to the pay schedule, **when** the user confirms the new start date, **then** the system recalculates past spending for the newly defined active window without duplicating logged transactions.

---

### US 3.2: Real-Time Budget Utilization Alerts
* **User Story:** As a user, I want to view visual meters and receive timely alerts when spending nears category limits so that I can adjust my purchasing behavior before overspending.
* **Acceptance Criteria:**
  * **Given** a budget category has a defined spending cap, **when** logged transactions cause cumulative spending to reach the 80% or 90% threshold, **then** a proactive warning notification is triggered within 60 seconds.
  * **Given** spending hits or exceeds 100%, **when** the user views the budget dashboard, **then** the meter transitions to an over-limit state (e.g., red highlight) displaying the exact overage amount.

---

### US 3.3: Automated Subscription Detection
* **User Story:** As a user, I want the AI to detect recurring payments and subscriptions from incoming transactional data so that I can view my total yearly subscription costs and anticipate upcoming charges.
* **Acceptance Criteria:**
  * **Given** a recurring payment pattern parsed from bank SMS or transaction feeds, **when** the subscription agent processes the data across repeated intervals (monthly, quarterly, annually), **then** the payment is added to the subscription dashboard with a predicted next payment date.
  * **Given** an active detected subscription list, **when** accessed by the user, **then** the interface surfaces the total monthly cost, annual projection, and renewal dates.

---

### US 3.4: Subscription Price Hike & Tier Change In-App Audit Report
* **User Story:** As a user, I want to see an in-app report and dashboard badge when a recurring subscription amount increases so that I can review the cost difference quietly without intrusive push notifications.
* **Acceptance Criteria:**
  * **Given** an actively tracked subscription, **when** a recurring charge clears at an amount higher than the previous period (excluding variable foreign exchange fees), **then** the system flags the subscription with a "Price Increase" status badge in the in-app subscription audit dashboard instead of sending a push alert.
  * **Given** a flagged subscription in the dashboard, **when** the user opens the subscription details or monthly audit report, **then** it displays a breakdown of the price delta, the historical vs. new rate, and a one-tap action to accept the update into future budget projections.

---

### US 3.5: Free Trial Expiration Tracker & In-App Cancellation Hub
* **User Story:** As a user, I want the system to track free trials in an in-app dashboard with countdown tags so that I can manage upcoming renewals without receiving external push notifications.
* **Acceptance Criteria:**
  * **Given** a $0 or $1 verification hold, or incoming transaction text containing trial keywords, **when** the parser evaluates the event, **then** a temporary subscription entry is created in the in-app subscription dashboard with an auto-calculated expiration timeline.
  * **Given** an active trial record within 48 hours of conversion, **when** the user visits the subscription hub, **then** the item displays an "Expiring Soon" badge alongside provider cancellation instructions and direct links.

---

### US 3.6: Category-Level "Safe-to-Spend" Daily Burn Rate
* **User Story:** As a user, I want to view a daily safe-to-spend allowance for discretionary categories so that I can pace my spending evenly across the remaining days of my paycheck cycle.
* **Acceptance Criteria:**
  * **Given** an active salary cycle with remaining days, **when** opening a discretionary category, **then** the UI displays the remaining balance divided by the days remaining as a daily limit.
  * **Given** an overspend occurs on day N, **when** the date rolls over to N+1, **then** the daily pacing metric recalibrates downwards dynamically across the remaining days.

---

### US 3.7: Unused & Ghost Subscription Identification
* **User Story:** As a user, I want an audit of recurring services that lack reciprocal app usage or engagement so that I can cancel subscriptions I am no longer actively using.
* **Acceptance Criteria:**
  * **Given** a recurring charge monitored by the subscription tracker, **when** no associated activity or value-add transactions appear within a 90-day rolling window, **then** the service is tagged as "Potentially Idle."
  * **Given** an idle-tagged service, **when** the user inspects the subscription view, **then** the interface calculates the cumulative capital spent since the last inferred interaction.

---

### US 3.8: One-Tap Category Fund Splitting for Shared Bills
* **User Story:** As a user, I want to exclude split or reimbursed portions of transactions from hitting my personal category budget so that my meters reflect only my actual financial share.
* **Acceptance Criteria:**
  * **Given** a settled transaction in a budgeted category, **when** the user marks it as "Shared/Split" and assigns a percentage or expected incoming credit, **then** only the user's net personal liability deducts from that category's cap.
  * **Given** an incoming peer-to-peer credit linked to that split, **when** it clears, **then** the system automatically reconciles the credit against the initial category deduction.

---

### US 3.9: Budget Carryover and Rollover
* **User Story:** As a user, I want the option to automatically transfer unspent budget balances into the next period or a different category so that I can maximize my unused funds.
* **Acceptance Criteria:**
  * **Given** a budget period concludes with a positive remaining balance in one or more categories, **when** flexible carryover is enabled for those categories, **then** the exact unspent amount is automatically rolled over and added to the subsequent month's allocation.
  * **Given** a user prefers to redirect leftover funds, **when** they configure the rollover destination, **then** the remaining funds can be directed into an emergency savings goal or alternate budget category.

---

# Feature 4: Financial Goal Planning & Savings Tracking

### Overview
Provides target-date and contribution-driven savings goal calculators, automatic fund allocation, real-time variance and health tracking, sandbox scenario simulation, milestone badges, and contingency lifecycle handling.

---

### US 4.1: Multi-Cadence Savings Goals Setup & Calculation
* **User Story:** As a user, I want to set up weekly, bi-weekly, or monthly savings targets with either a target date or a fixed periodic budget so that I can automatically calculate my required savings and visually track my progress.
* **Acceptance Criteria:**
  * **Given** the user creates a new savings goal in target-date mode, **when** they input the target amount, completion date, and cadence (weekly, bi-weekly, or monthly), **then** the required periodic contribution is calculated automatically and a progress bar and baseline timeline chart are generated.
  * **Given** the user creates a new savings goal in contribution-driven mode, **when** they input the target amount and a fixed periodic contribution, **then** the estimated completion date is calculated and displayed on the timeline.
  * **Given** the user inputs a completion date in the past or an amount less than or equal to zero, **when** they attempt to save, **then** an error message is displayed and the goal is not saved.
  * **Given** the user inputs an initial deposit equal to or greater than the target amount, **when** they submit, **then** the system marks the goal as completed immediately.

---

### US 4.2: Savings Contribution & Fund Allocation Tracking
* **User Story:** As a user, I want to log manual deposits or link account transfers to my active savings goals so that my real-world savings are credited toward my goals and update my progress in real time.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** the user logs a deposit amount, **then** the goal balance updates immediately, the progress bar advances, and the contribution is logged in the goal history.
  * **Given** an active savings goal near completion, **when** a deposit causes the saved balance to meet or exceed the target amount, **then** the goal is marked as completed, progress is set to 100%, and the user is prompted to allocate any surplus funds.
  * **Given** an active savings goal, **when** the user enters an invalid or negative deposit amount, **then** the system rejects the input and displays an error message.

---

### US 4.3: Real-Time Goal Health & Variance Tracking
* **User Story:** As a user, I want the app to compare my actual savings against my scheduled plan so that I can immediately see whether I am on track, ahead, or behind schedule.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** the user views their goal progress, **then** a status indicator shows whether the goal is on track, ahead, or behind schedule based on scheduled versus actual savings.
  * **Given** a savings goal that is behind schedule due to missed or lower contributions, **when** the user opens the goal details, **then** the shortfall amount is displayed along with an option to simulate a catch-up plan.
  * **Given** a savings goal where actual savings exceed the scheduled amount, **when** the user views the goal, **then** the goal displays an ahead-of-schedule status with an earlier projected completion date.

---

### US 4.4: Dynamic Goal Scenario Simulation & Strategy Adoption
* **User Story:** As a user, I want to simulate different contribution amounts, frequencies, or one-time deposits in a sandbox simulator so that I can see how changes affect my completion date and apply the best strategy to my active goal.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** the user adjusts contribution amounts or cadence in the scenario simulator, **then** the estimated completion timeline and date update immediately in real time.
  * **Given** a simulated scenario, **when** the user inputs a one-time lump-sum deposit, **then** the timeline recalculates showing the earlier completion date or reduced future periodic contributions.
  * **Given** a simulated scenario, **when** the user clicks to adopt the strategy, **then** the system updates the active goal settings with the new contribution amount and schedule.
  * **Given** a simulated scenario, **when** the user exits the simulator without adopting, **then** no changes are saved and the original goal remains unchanged.

---

### US 4.5: Goal Lifecycle Management & Contingency Handling
* **User Story:** As a user, I want to pause, edit, or make emergency partial withdrawals from my goal so that I can handle unexpected life events without losing my savings history.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** the user pauses the goal, **then** recurring contributions are paused and variance tracking is frozen until resumed.
  * **Given** an active savings goal with accumulated funds, **when** the user logs an emergency partial withdrawal, **then** the goal balance is reduced, the withdrawal reason is saved, and the app displays the updated timeline impact.
  * **Given** an active savings goal, **when** the user cancels the goal, **then** the goal is closed and the accumulated funds are transferred back to the user's primary wallet or reallocated to other goals.

---

### US 4.6: Milestone Tracking & Predictive Progress Alerts
* **User Story:** As a user, I want to see visual milestone badges inside my goal (at 25%, 50%, 75%, and 100%) and receive actionable notifications when I reach key milestones or fall behind on scheduled contributions, so that I can track milestone achievements directly inside that goal and correct missed savings targets.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** a contribution causes the saved balance to cross a 25%, 50%, 75%, or 100% threshold for the first time, **then** the corresponding milestone badge activates directly inside that goal's progress view and a celebratory progress notification is displayed.
  * **Given** an active savings goal where a withdrawal previously dropped the balance below a milestone, **when** a subsequent deposit crosses that milestone again, **then** the milestone badge inside that goal updates its state but duplicate notifications are suppressed.
  * **Given** an active savings goal with scheduled contributions, **when** a scheduled contribution date passes without a logged deposit, **then** the system delivers a gentle reminder showing the shortfall and provides options to log the contribution now or automatically rebalance future payments to stay on target.
  * **Given** an active savings goal, **when** the user reaches 100% completion, **then** a completed badge is displayed inside that goal, the final goal summary with total duration and contributions is generated, and recurring scheduled debits are automatically stopped.
  * **Given** the user preferences screen, **when** the user adjusts notification preferences, **then** they can customize or mute milestone alerts and overdue contribution reminders independently.

---

# Feature 5: Smart Notifications & Alerts Engine

### Overview
A centralized, intelligent notification engine providing proactive financial nudges, multi-stage debt warnings, anomaly alerts, budget threshold tracking, velocity spikes, DND quiet hour bypass rules, and anti-fatigue rate limits.

---

### US 5.1: Escalated Multi-Stage Debt Deadline Notifications
* **User Story:** As a user, I want to receive escalated multi-stage alerts prior to an installment due date or credit card grace period expiration so that I do not miss the deadline and incur severe penalty fees.
* **Acceptance Criteria:**
  * **Given** an active debt or installment obligation with a strict grace period, **when** the payment timeline reaches 7 days, 3 days, 24 hours prior, and 0 days (due date), **then** high-priority multi-stage notifications are triggered at each milestone.
  * **Given** the final 24-hour and due-day alerts are dispatched, **when** active quiet hours are configured, **then** these high-priority alerts bypass Do-Not-Disturb filters to prevent critical financial default.

---

### US 5.2: Unusual Transaction & Anomaly Detection Security Warning
* **User Story:** As a user, I want an instant security warning if a transaction deviates significantly from my normal spending baseline, exhibits duplicate charges, or shows uncharacteristic merchant behavior so that I can catch fraud or billing errors.
* **Acceptance Criteria:**
  * **Given** the anomaly detection model monitors incoming transactions, **when** an expense amount exceeds statistical Z-score thresholds for that category or exhibits a duplicate charge pattern within minutes, **then** an immediate high-priority security alert is triggered.
  * **Given** the alert is delivered, **when** the user opens it, **then** the notification presents options to "Confirm Legitimate", "Flag as Duplicate", or "Review Card Security".

---

### US 5.3: Real-Time Budget Exceeded Alert
* **User Story:** As a user, I want to receive an immediate notification when I breach a category or total monthly budget cap so that I can halt non-essential spending right away.
* **Acceptance Criteria:**
  * **Given** an active category or total budget cap, **when** a newly recorded transaction causes cumulative spending to exceed 100% of the allocated amount, **then** a real-time budget exceeded push notification and in-app alert are triggered within 60 seconds.
  * **Given** the notification is tapped, **when** opened, **then** the app navigates to the affected budget category showing the exact overage and recommendations to rebalance.

---

### US 5.4: Approaching Category Limit Alert
* **User Story:** As a user, I want to be warned when spending reaches pre-defined thresholds of my category budget so that I can moderate my expenses before exceeding my limit.
* **Acceptance Criteria:**
  * **Given** an active category budget with a configured warning threshold (e.g., 80% or 90%), **when** a logged transaction brings cumulative spending across that threshold, **then** an approaching-limit warning is dispatched.
  * **Given** the alert is sent, **when** the user views their budget, **then** the category meter highlights in yellow/amber showing remaining spendable funds.

---

### US 5.5: Spending Velocity Spike Alert
* **User Story:** As a user, I want to be alerted when my daily spending significantly outpaces my historical average for that specific day or category so that I become aware of abnormal spending patterns.
* **Acceptance Criteria:**
  * **Given** historical spending baseline data exists, **when** daily spending on a specific day or within a category significantly exceeds the historical average velocity, **then** a spending velocity spike alert is sent to the user.
  * **Given** the alert is dispatched, **when** tapped, **then** it displays a breakdown of the specific purchases driving the spike relative to the standard daily pace.

---

### US 5.6: Upcoming Bill and Utility Reminders
* **User Story:** As a user, I want advance reminders for upcoming utility bills and manual payment obligations so that I can pay them on time and avoid late fees or service disruptions.
* **Acceptance Criteria:**
  * **Given** a scheduled utility bill or manual payment obligation with an upcoming due date, **when** the system reaches the scheduled advance reminder window (e.g., 3 days prior), **then** an advance bill reminder notification is dispatched.
  * **Given** the notification is triggered, **when** opened, **then** the app provides a direct link to mark the bill as paid, log the expense, or view provider payment details.

---

### US 5.7: Upcoming Subscription Renewal Reminders
* **User Story:** As a user, I want to be notified before recurring subscriptions auto-renew so that I can review or cancel unwanted active subscriptions prior to billing.
* **Acceptance Criteria:**
  * **Given** an active manual or AI-detected subscription, **when** the billing cycle approaches the renewal date (e.g., 48 hours in advance), **then** an advance renewal reminder notification is sent to the user.
  * **Given** the alert is received, **when** inspected, **then** the user is presented with the charge amount, billing card, and a direct link to the provider cancellation instructions.

---

### US 5.8: Predicted Low Balance and Cash Shortage Warning
* **User Story:** As a user, I want to receive a predictive notification when my current spending velocity indicates a cash shortfall before my next paycheck so that I can adjust my burn rate in time.
* **Acceptance Criteria:**
  * **Given** the time-series forecasting model is running, **when** forecasted outflows exceed available liquid balances before the anticipated next income date, **then** a predictive low balance warning is dispatched.
  * **Given** the warning is viewed, **when** tapped, **then** it provides an estimated run-out date and actionable suggestions to reduce discretionary burn.

---

### US 5.9: Savings Goal Progress Milestone Notifications
* **User Story:** As a user, I want to receive positive milestone notifications when my savings reach key targets like 50% or 75% so that I stay motivated to complete my goals.
* **Acceptance Criteria:**
  * **Given** an active savings goal, **when** a contribution brings the cumulative saved amount to or beyond a defined milestone (e.g., 25%, 50%, 75%), **then** a celebratory milestone notification is delivered.
  * **Given** a milestone notification is opened, **when** viewed, **then** the goal view displays the unlocked milestone badge and the updated countdown to final completion.

---

### US 5.10: Savings Goal Delay Alert
* **User Story:** As a user, I want to be alerted when my contribution pacing falls behind my planned savings schedule so that I can adjust my deposits to meet my deadline.
* **Acceptance Criteria:**
  * **Given** an active savings goal with a target completion date, **when** recurring contributions or actual deposits lag behind the required schedule pacing, **then** a delay warning alert is triggered.
  * **Given** the alert is opened, **when** the user reviews options, **then** the app offers a one-tap catch-up deposit or recalculates the future monthly contribution needed to meet the original target date.

---

### US 5.11: Proactive Personalized AI Recommendation Nudges
* **User Story:** As a user, I want to receive proactive personalized AI nudges recommending cost-saving actions or budget adjustments so that I can optimize my personal finances.
* **Acceptance Criteria:**
  * **Given** the AI Recommendation Agent generates a tailored financial suggestion (e.g., swapping a high-cost recurring habit or switching subscription tiers), **when** the recommendation is ready for user review, **then** a proactive nudge notification is sent linking directly to an interactive Action Card.
  * **Given** an interactive Action Card, **when** the user interacts with it, **then** they can accept, snooze, or dismiss the recommendation with feedback.

---

### US 5.12: Automated Weekly Spending Summary Notification
* **User Story:** As a user, I want to receive an automated weekly spending digest so that I can stay informed about my week-over-week spending trends.
* **Acceptance Criteria:**
  * **Given** a completed calendar week, **when** the weekly scheduled report is generated, **then** an automated summary notification is dispatched delivering the total spend, top category, and week-over-week percentage change.
  * **Given** the user taps the weekly digest notification, **when** opened, **then** it transitions into the comprehensive weekly financial analytics breakdown.

---

### US 5.13: Automated Monthly Financial Report Notification
* **User Story:** As a user, I want to receive an end-of-month notification summarizing my complete monthly financial performance so that I can review total cash flow and category adherence.
* **Acceptance Criteria:**
  * **Given** the conclusion of a monthly billing or calendar cycle, **when** the monthly report is finalized, **then** a notification is delivered directing the user to their comprehensive in-app monthly summary.
  * **Given** the user opens the monthly report, **when** viewed, **then** it presents net savings, cash flow charts, category breakdowns, and export buttons.

---

### US 5.14: Multi-Channel Dispatch & In-App Notification Center
* **User Story:** As a user, I want alerts delivered simultaneously via system push notifications and stored in an in-app Notification Center so that I can review unread alerts at my convenience.
* **Acceptance Criteria:**
  * **Given** any notification is triggered, **when** it is dispatched, **then** it appears as a mobile system push notification and is simultaneously logged as an unread item in the in-app Notification Center.
  * **Given** unread notifications exist in the app, **when** the user opens the Notification Center, **then** they can view, mark as read, filter by priority, or navigate directly to the relevant transaction or budget item.

---

### US 5.15: Configurable Do-Not-Disturb (DND) Quiet Hours
* **User Story:** As a user, I want to configure custom quiet hours so that non-urgent notifications are muted during sleeping or resting periods.
* **Acceptance Criteria:**
  * **Given** quiet hours are configured (e.g., 11:00 PM to 7:00 AM), **when** a non-urgent alert (e.g., weekly digest or routine milestone) is generated during this window, **then** the mobile push sound/banner is suppressed and queued for delivery in the morning inbox.
  * **Given** the morning quiet hours expire, **when** the clock reaches the end time, **then** a digest of queued notifications is surfaced quietly in the notification center.

---

### US 5.16: Critical Alert DND Bypass
* **User Story:** As a user, I want urgent debt grace-period and suspected fraud alerts to bypass my quiet hours so that I never miss critical financial penalties or security incidents.
* **Acceptance Criteria:**
  * **Given** Do-Not-Disturb quiet hours are active, **when** a critical debt deadline (due within 24 hours) or a high-confidence fraud/anomaly alert is triggered, **then** the notification bypasses the mute filter and sounds immediately with high priority.
  * **Given** a bypassed alert, **when** received, **then** it is tagged with an urgent red badge indicating critical priority.

---

### US 5.17: Daily Notification Rate Limiting
* **User Story:** As a user, I want a daily rate cap of maximum 3 non-critical alerts per day so that I am protected from alert fatigue and notification spam.
* **Acceptance Criteria:**
  * **Given** a user has already received 3 non-critical push notifications within a 24-hour day, **when** an additional non-critical alert is triggered, **then** the system suppresses the push notification and routes it directly to the in-app inbox.
  * **Given** rate limiting is active, **when** a critical alert occurs (such as fraud or debt due), **then** it bypasses the daily rate limit and is delivered unconditionally.

---

### US 5.18: Granular Notification Preference Toggles
* **User Story:** As a user, I want independent toggle switches for each alert category so that I can enable or disable specific notification types according to my preference.
* **Acceptance Criteria:**
  * **Given** the user opens notification preferences, **when** they toggle off a specific category (such as budget warnings or weekly summaries) while keeping others active (such as bill reminders or debt alerts), **then** only enabled category notifications are generated and delivered.
  * **Given** a disabled notification category, **when** an event of that type occurs, **then** it is neither pushed to the device nor flagged in the inbox.

---

### US 5.19: Customizable Budget Trigger Thresholds
* **User Story:** As a user, I want to define custom percentage trigger thresholds for budget alerts so that I receive warnings at the exact spending percentages I prefer.
* **Acceptance Criteria:**
  * **Given** the user is in alert settings, **when** they customize the warning threshold slider (such as to 75%, 85%, or 95%), **then** approaching-limit alerts trigger only when spending crosses that specific configured percentage.
  * **Given** multiple categories, **when** configured by the user, **then** threshold percentages can be customized globally or on a per-category basis.

---

# Feature 6: Comprehensive Financial Reporting & Analytics

### Overview
A robust financial analytics suite delivering interactive time-series visualizations, category spend decompositions, budget-vs-actual analyses, savings projections, month-over-month comparisons, subscription audits, top merchant rankings, anomaly logs, natural language AI inquiries, and PDF/CSV exports.

---

### US 6.1: Cash Flow & Net Savings Report
* **User Story:** As a user, I want to view a monthly income versus expense report so that I can evaluate my net savings and total cash flow over time.
* **Acceptance Criteria:**
  * **Given** the user accesses the reporting dashboard, **when** they select the Income vs. Expense report, **then** a time-series chart renders comparing total inflows to total outflows across the selected period.
  * **Given** the chart renders, **when** inspected, **then** it displays the net savings figure (Income minus Expense) and net savings rate percentage.

---

### US 6.2: Category-Wise Spending Breakdown
* **User Story:** As a user, I want to see a breakdown of my spending by category so that I can identify which areas consume the largest share of my budget.
* **Acceptance Criteria:**
  * **Given** the user has recorded transactions across multiple categories, **when** they open the Category Breakdown report, **then** an interactive pie or bar chart renders showing the percentage and total monetary amount spent per category.
  * **Given** a specific category slice is selected, **when** tapped, **then** the report drills down into sub-categories and itemized transactions.

---

### US 6.3: Budget vs. Actual Spending Report
* **User Story:** As a user, I want to see how my actual spending compares to the budgets I set so that I can identify categories where I am overspending.
* **Acceptance Criteria:**
  * **Given** the user has defined budgets for one or more categories, **when** they open the Budget vs. Actual report, **then** each category displays the budgeted amount, actual amount spent, and the variance as both a numerical value and a color-coded progress bar.
  * **Given** an overspent category, **when** viewed, **then** it displays the overage amount highlighted in red with an alert indicator.

---

### US 6.4: Savings Goal Progress Tracking
* **User Story:** As a user, I want to track my progress toward a savings goal so that I can stay motivated and adjust my spending accordingly.
* **Acceptance Criteria:**
  * **Given** the user has created a savings goal with a target amount and date, **when** they view the Savings Goals report, **then** the system displays the current saved amount, percentage completed, and projected completion date based on the current saving rate.
  * **Given** historical contributions, **when** rendered on the report, **then** a pacing trajectory chart plots actual savings against the baseline target line.

---

### US 6.5: Month-over-Month Comparison
* **User Story:** As a user, I want to compare my spending this month against the previous month so that I can track whether my financial habits are improving.
* **Acceptance Criteria:**
  * **Given** at least two months of transaction history exist, **when** the user views the Comparison report, **then** the system displays side-by-side totals and a percentage change indicator (+/- %) for each category.
  * **Given** categories with significant increases (>15%), **when** rendered, **then** the report flags them as top contributors to spending inflation.

---

### US 6.6: Recurring Subscription Detection Report
* **User Story:** As a user, I want the app to automatically detect recurring subscriptions from my transaction history so that I can identify services I may want to cancel.
* **Acceptance Criteria:**
  * **Given** the user has at least three months of transaction history, **when** the system analyzes the data for repeating merchant charges, **then** a Subscriptions report lists each detected recurring payment with its frequency and total annual cost.
  * **Given** detected subscriptions, **when** displayed, **then** the report aggregates the cumulative yearly subscription liability.

---

### US 6.7: Top Merchants & Largest Transactions Report
* **User Story:** As a user, I want to see which merchants I spend the most at and which individual transactions were the largest so that I can identify where most of my money goes.
* **Acceptance Criteria:**
  * **Given** the user has recorded transaction history with merchant names, **when** they open this report, **then** it displays merchants ranked by total spend alongside a separate list of the top 10 largest individual transactions in the selected period.
  * **Given** a merchant in the list, **when** tapped, **then** all transactions associated with that merchant are filtered and displayed.

---

### US 6.8: Unusual Transaction Alerts Report
* **User Story:** As a user, I want to see a report of transactions flagged as unusual so that I can quickly identify potential errors or fraudulent activity.
* **Acceptance Criteria:**
  * **Given** a transaction amount significantly deviates from the user's historical spending pattern for that category, **when** the reporting engine processes the transaction, **then** the transaction appears in the Unusual Activity report with the reason it was flagged.
  * **Given** an item in the report, **when** viewed by the user, **then** action buttons allow the user to confirm it as normal or flag it for bank inquiry.

---

### US 6.9: Natural-Language Financial Query (AI Assistant)
* **User Story:** As a user, I want to ask a question about my spending in plain language (e.g., "how much did I spend on transport last week?") so that I can get answers without manually navigating reports.
* **Acceptance Criteria:**
  * **Given** the user submits a typed or spoken query to the AI assistant, **when** the system parses the query intent, entity, and timeframe, **then** it returns a direct natural-language answer along with the relevant exact figure pulled from transaction data.
  * **Given** a complex query involving comparisons (e.g., "Did I spend more on groceries in August or July?"), **when** evaluated, **then** the assistant returns a comparative summary table and chart.

---

### US 6.10: Exportable Financial Reports (PDF / CSV)
* **User Story:** As a user, I want to export my financial reports as a PDF or CSV file so that I can save or share them outside the app.
* **Acceptance Criteria:**
  * **Given** the user is viewing any generated report, **when** they tap the "Export" button and choose a format (PDF or CSV), **then** the system generates and downloads a formatted file containing the report's charts, summary statistics, and itemized data.
  * **Given** PDF export, **when** generated, **then** it includes branded headers, date range metadata, category summaries, and high-resolution chart snapshots suitable for printing or tax accounting.

---

# Feature 7 & 8: AI Suite & Multi-Agent Financial System

### Overview
Orchestrates autonomous multi-agent financial reasoning, conversational natural-language queries, interactive human-in-the-loop authorization cards, and LLM-generated narrative financial health summaries tailored to the Egyptian market.

---

### US 7.1: Natural Language Financial Queries
* **User Story:** As a user, I want to ask free-form questions like "Can I afford a 35,000 EGP laptop?" to the AI Assistant so that I receive personalized advice and feasibility calculations.
* **Acceptance Criteria:**
  * **Given** the user submits a complex query, **when** the Supervisor Agent decomposes the request, **then** the relevant specialized agents calculate cash flow and return a synthesized written explanation and charts.

---

### US 7.2: Human-in-the-Loop Agent Authorization
* **User Story:** As a user, I want all autonomous AI recommendations to require my explicit approval via Action Cards so that the AI cannot mutate my budgets or parameters without my permission.
* **Acceptance Criteria:**
  * **Given** the Budgeting Agent proposes a limit re-allocation, **when** the recommendation is presented, **then** it appears as a 1-tap Action Card requiring an explicit "Approve" or "Dismiss" input from the user before applying.

---

### US 7.3: AI Narrative Report Summarization
* **User Story:** As a user, I want my weekly and monthly financial digests converted into human-readable narrative summaries by a Large Language Model so that I can easily understand my financial health without analyzing raw data tables.
* **Acceptance Criteria:**
  * **Given** a periodic digest is generated, **when** the cloud API processes the quantitative tables, **then** a concise text summary is displayed at the top of the report in natural Egyptian Arabic or English.

---

# Feature 9: Card Debts & Installment Tracking

### Overview
Tracks bank cards, formal credit lines, zero-interest consumer installment promotions, processing fees, and bank reward points, while employing hybrid AI risk models to formulate optimal debt payoff schedules.

---

### US 9.1: Zero-Interest Installment Tracking
* **User Story:** As a user, I want to track promotional 0% interest installment schemes along with their upfront or monthly admin processing fees so that I can see the true cost of my active plans.
* **Acceptance Criteria:**
  * **Given** the user inputs a new zero-interest installment, **when** they define the duration and admin fees, **then** the Installment Ledger calculates and displays the exact monthly debt obligation.

---

### US 9.2: Bank Rewards Net Benefit Calculator
* **User Story:** As a user, I want the app to calculate the cashback and reward points I earn on an installment so that I can evaluate if the earned points offset the bank's processing fees.
* **Acceptance Criteria:**
  * **Given** an active installment plan on a tracked card, **when** the hybrid rewards engine applies the pre-configured bank template, **then** the UI displays the net benefit comparing accrued points against total interest overhead.

---

### US 9.3: Hybrid Risk Debt Optimization
* **User Story:** As a user, I want the AI to rank my debts and formulate a payoff strategy so that I can address urgent penalty deadlines first, followed by high-interest obligations.
* **Acceptance Criteria:**
  * **Given** the user has multiple active card debts, **when** the Debt Risk Agent runs its optimization algorithm, **then** a prioritized action plan is generated with urgent grace-period debts ranked as Tier 1, and Avalanche-method debts as Tier 2.
