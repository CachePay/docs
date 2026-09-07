# Simple Use Case Guide & Project Mapping

A simple, clear guide that explains all the **Use Cases** in our graduation project, who uses them, and how they connect to our user stories.

---

## 1. What is a Use Case? (In Plain Words)

* **A Use Case** is simply an **action** a user (or external system) performs in the app to get a real result.
  * *Example:* "Log an Expense", "Set a Budget", "Create a Savings Goal".
* **An Actor** is **who** performs the action (e.g., Parent, Partner, Child, or an external system like Android SMS reader).
* **What is `<<include>>`?**
  * A sub-step that **must** happen. (Example: To delete an account, the app *must include* password verification).
* **What is `<<extend>>`?**
  * An **optional bonus action** that only happens under certain conditions. (Example: When logging an expense, you can *optionally* choose to "Attach Receipt Later").

---

## 2. Who are the Actors?

| Actor Name | Who are they? | What can they do? |
| :--- | :--- | :--- |
| **Primary User (Parent / Admin)** | The main account owner | Controls household finances, invites kids, shares with partner, sets family budgets. |
| **Partner User** | Spouse / Co-manager | Shares budgets and expenses with the primary user with full visibility. |
| **Kid / Dependent** | Child or Teen | Has a monitored account with spending limits set by parents. |
| **Guest** | New user not logged in | Can register a new account or request a password reset. |
| **Android System (SMS)** | Phone operating system | Automatically catches bank & e-wallet SMS messages and sends them to the app. |
| **AI Assistant / Multi-Agent System** | Smart AI engine | Answers user questions in plain Arabic/English, suggests debt payoff plans, and detects recurring subscriptions. |
| **Scanner & Voice Services** | OCR & Voice engines | Scans paper receipts using the camera and turns voice notes into text. |

---

## 3. All Use Cases by Feature

Here is every valid use case in our system, grouped by feature:

### Feature 1: Accounts & Household Management
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 1** | **Register Primary Account** | Guest | A new user signs up with name, email, and password. | US 1.1 | Normal |
| **UC 2** | **Invite Kid Sub-Account** | Primary User | Parent creates a 6-character invitation code to set up a child's account. | US 1.2 | Normal |
| **UC 3** | **Turn On Partner Sharing** | Primary & Partner | Allows a couple to see and share each other's expenses and budgets. | US 1.3 | Normal |
| **UC 4** | **Detach Account from Family** | Sub-Account | A partner or teen leaves the household to become an independent account. | US 1.4 | Includes Login/2FA |
| **UC 5** | **Reset / Recover Password** | Any User | User resets forgotten password via email/SMS OTP (parents can reset kid PIN). | US 1.5 | Normal |
| **UC 6** | **Delete Account & Data** | Any User | Permanently deletes the account and all associated data. | US 1.6 | Includes Login/2FA |
| **UC 7** | **Graduate Account with Bank Card** | Kid / Teen | When a teen gets their own bank card, they graduate to an independent adult account. | US 1.7 | Extension of UC 4 |

---

### Feature 2: Logging Expenses & Cash Management
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 8** | **Log Manual Expense** | User | User enters an amount, date, and category for an expense. | US 2.1 | Normal |
| **UC 9** | **Attach Receipt Later** | User | User uploads a photo of a receipt for a transaction saved earlier without one. | US 2.1 | Extension of UC 8 |
| **UC 10** | **Check & Confirm Daily Cash** | User | User responds to the end-of-day prompt to check if physical pocket cash matches the app. | US 2.2 | Normal |
| **UC 11** | **Adjust Cash Discrepancy** | User | User types actual cash in hand; the app automatically creates a balancing transaction. | US 2.3 | Extension of UC 10 |
| **UC 12** | **Search & Filter Transactions** | User | Searches past expenses by merchant name, date range, payment method, or amount. | US 2.4 | Normal |
| **UC 13** | **Import Bank Statements** | User | Uploads an Excel, CSV, or PDF bank statement to import past transactions at once. | US 2.5 | Normal |
| **UC 14** | **Auto-Read Bank/Wallet SMS** | Android System | When a bank SMS arrives, the app reads it automatically and records the expense. | US 2.6 | System Action |
| **UC 15** | **Log Expense by Voice Note** | User + Voice AI | User speaks a short voice note (in Egyptian Arabic or English) to log expenses. | US 2.8 | Normal |
| **UC 16** | **Scan & Split Receipt with Camera** | User + Camera | User snaps a photo of a receipt; OCR reads items so user can split them into categories. | US 2.9 | Normal |

---

### Feature 3: Smart Budgeting & Subscriptions
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 17** | **Set Up Salary-Cycle Budget** | User | Sets budgets that reset on payday (e.g. 28th of every month) instead of the 1st. | US 3.1 | Normal |
| **UC 18** | **View & Manage Subscriptions** | User + AI | Tracks recurring monthly/yearly payments (Netflix, gym, bills) detected by the app. | US 3.3 | Normal |
| **UC 19** | **Review Subscription Price Hike** | User | When a service raises its price, user reviews the change and updates their budget. | US 3.4 | Extension of UC 18 |
| **UC 20** | **Track Free Trials & Cancellations** | User | Shows countdown timers for free trials with instructions on how to cancel them. | US 3.5 | Normal |
| **UC 21** | **Audit Idle / Ghost Subscriptions** | User + AI | Lists services the user pays for but hasn't used in 90 days so they can cancel them. | US 3.7 | Extension of UC 18 |
| **UC 22** | **Split Bill with Friends / Family** | User | Marks part of an expense as "shared" so only the user's actual share affects their budget. | US 3.8 | Extension of UC 8 |
| **UC 23** | **Set Up Budget Rollover Rules** | User | Automatically transfers unspent budget money into next month or into a savings goal. | US 3.9 | Normal |

---

### Feature 4: Financial Savings Goals
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 24** | **Create a Savings Goal** | User | Sets a target amount and target date (e.g., "Save 50,000 EGP for Vacation by July"). | US 4.1 | Normal |
| **UC 25** | **Add Money to Savings Goal** | User | Deposits money toward a goal and watches the progress bar move forward. | US 4.2 | Normal |
| **UC 26** | **Simulate Savings Scenarios** | User | Uses interactive sliders to see: "What if I save 500 EGP more per month?" | US 4.4 | Extension of UC 24 |
| **UC 27** | **Pause, Withdraw, or Cancel Goal** | User | Temporarily pauses a goal, takes out emergency money, or cancels it completely. | US 4.5 | Normal |

---

### Feature 5: Notifications & Preferences
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 28** | **View Notification Center** | User | Opens the in-app inbox to read past alerts, mark them as read, or tap to view details. | US 5.14 | Normal |
| **UC 29** | **Change Notification Settings** | User | Turns alert types on/off, sets quiet hours (DND), and changes warning sliders (e.g., 85%). | US 5.15, 5.18, 5.19 | Combined Settings |

---

### Feature 6: Financial Reports & Analytics
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 30** | **View Financial Reports & Charts** | User | Views monthly breakdown, cash flow, top spending merchants, and month-over-month charts. | US 6.1 to 6.7 | Normal |
| **UC 31** | **Review Flagged Transactions** | User | Inspects suspicious or duplicate transactions flagged by the system and marks them normal or fraud. | US 6.8 | Normal |
| **UC 32** | **Export Report to PDF or CSV** | User | Downloads or shares a clean PDF or Excel spreadsheet of their financial reports. | US 6.10 | Extension of UC 30 |

---

### Feature 7 & 8: AI Suite & Multi-Agent Financial System
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 33** | **Ask AI Financial Questions** | User + AI | User types/speaks questions like *"Can I afford a 35,000 EGP laptop?"* and gets an instant feasibility answer. | US 6.9, US 7.1 | Normal |
| **UC 34** | **Approve or Dismiss AI Action Cards** | User | When AI suggests moving money between budgets, user gets a 1-tap card to approve or reject it. | US 5.11, US 7.2 | Normal |

---

### Feature 9: Card Debts & Installment Tracking
| Use Case # | Use Case Name | Actor | What does it do? | From Story | Type |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UC 35** | **Add & Track an Installment Plan** | User | Logs 0% interest retail installment schemes with duration and bank admin fees. | US 9.1 | Normal |
| **UC 36** | **Calculate Rewards vs. Fees on Installments** | User | Compares cashback/points earned from the bank against processing fees to see the net benefit. | US 9.2 | Extension of UC 35 |
| **UC 37** | **Get AI Debt Payoff Strategy** | User + AI | AI ranks all credit card debts and creates an optimal payoff plan (urgent deadlines first, then high interest). | US 9.3 | Normal |

---

## 4. Why are Some User Stories NOT Use Cases?

> **Important note for your Doctor / Supervisor:**  
> In Software Engineering, you **should never** turn every single user story into a use case bubble. That is a famous beginner mistake called **"Functional Decomposition"**.  
> Out of **67 total user stories**, we have **37 clean use cases**. Here is why the other 22 stories are not separate use cases:

### 1. They are Math Formulas / Calculations (Not User Actions)
* **US 3.6 (Daily Safe-to-Spend Burn Rate):** The app simply divides remaining budget by remaining days. The user doesn't click a button to "calculate"; they just see the number on the screen.
* **US 4.3 (Goal Variance Health):** The app checks if you are ahead or behind schedule. It's an internal math calculation, not a user action.

### 2. They are Automated Notifications (Sent by System, Not Done by User)
* **US 3.2, 4.6, 5.1 to 5.10, 5.12, 5.13:**  
  * E.g., alert when budget reaches 80%, alert 24h before debt penalty, weekly digest, milestone unlocked badge.
  * **Why not use cases?** A push notification popping up on your phone is a **system background alert**, not an action the user takes. The user's action is simply **UC 28: View Notification Center**.

### 3. They are Automated Background Rules
* **US 2.7 (ATM detection auto-adds to cash wallet):** When the app reads an ATM withdrawal SMS, it automatically credits your cash wallet. The system does this behind the scenes.
* **US 2.10 (GPS tagging on SMS arrival):** The app quietly tags location coordinates in the background.

### 4. They are Combined into One Settings Screen
* **US 5.15 (Quiet hours), US 5.18 (Alert toggles), US 5.19 (Threshold sliders):**  
  * Instead of making 3 separate use case bubbles for 3 checkboxes, they are all handled inside one clean use case: **UC 29: Change Notification Settings**.

### 5. They are Background Security / Filtering Rules
* **US 5.16 (Critical alert bypasses quiet hours):** This is a priority rule inside the app code, not a button the user presses.
* **US 5.17 (Max 3 alerts per day):** This is an anti-spam rate limiter in the code.

### 6. Automated Text Summaries
* **US 7.3 (AI Narrative Summary):** The LLM writes a 2-sentence summary at the top of the monthly report. This is part of viewing the report (**UC 30**), not an independent use case.

---

## 5. Master Quick-Reference List (Cheat Sheet)

If your supervisor asks for the list of Use Cases in your graduation project, here is the complete 37-item list:

1. **UC 1:** Register Primary Account
2. **UC 2:** Invite Kid Sub-Account
3. **UC 3:** Turn On Partner Sharing
4. **UC 4:** Detach Account from Family
5. **UC 5:** Reset / Recover Password
6. **UC 6:** Delete Account & Data
7. **UC 7:** Graduate Account with Bank Card *(Extends UC 4)*
8. **UC 8:** Log Manual Expense
9. **UC 9:** Attach Receipt Later *(Extends UC 8)*
10. **UC 10:** Check & Confirm Daily Cash
11. **UC 11:** Adjust Cash Discrepancy *(Extends UC 10)*
12. **UC 12:** Search & Filter Transactions
13. **UC 13:** Import Bank Statements
14. **UC 14:** Auto-Read Bank/Wallet SMS
15. **UC 15:** Log Expense by Voice Note
16. **UC 16:** Scan & Split Receipt with Camera
17. **UC 17:** Set Up Salary-Cycle Budget
18. **UC 18:** View & Manage Subscriptions
19. **UC 19:** Review Subscription Price Hike *(Extends UC 18)*
20. **UC 20:** Track Free Trials & Cancellations
21. **UC 21:** Audit Idle / Ghost Subscriptions *(Extends UC 18)*
22. **UC 22:** Split Bill with Friends / Family *(Extends UC 8)*
23. **UC 23:** Set Up Budget Rollover Rules
24. **UC 24:** Create a Savings Goal
25. **UC 25:** Add Money to Savings Goal
26. **UC 26:** Simulate Savings Scenarios *(Extends UC 24)*
27. **UC 27:** Pause, Withdraw, or Cancel Goal
28. **UC 28:** View Notification Center
29. **UC 29:** Change Notification Settings
30. **UC 30:** View Financial Reports & Charts
31. **UC 31:** Review Flagged Transactions
32. **UC 32:** Export Report to PDF or CSV *(Extends UC 30)*
33. **UC 33:** Ask AI Financial Questions
34. **UC 34:** Approve or Dismiss AI Action Cards
35. **UC 35:** Add & Track an Installment Plan
36. **UC 36:** Calculate Rewards vs. Fees on Installments *(Extends UC 35)*
37. **UC 37:** Get AI Debt Payoff Strategy
