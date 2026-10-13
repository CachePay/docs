# 06 · Suggested Features to Beat the Competition

> Product-level only. No tech stack, architecture or effort estimates.
> **Type:** Table-stakes / Differentiator / Moat (hard to copy because of data, network or habit). **Priority:** Must / Should / Nice.
> "Planned" means it's already in our user stories. "New" means it isn't in any project file yet.

## A. Prioritised feature list

### Must-have
| # | Feature | What the user experiences | Problem solved | Beats (and why) | Type | Status |
|---|---|---|---|---|---|---|
| 1 | **Smart SMS routing with zero setup** | On first launch the app scans recent bank and wallet SMS and says "We found CIB ••4321, NBE ••8890 and Vodafone Cash. Tap to confirm." From then on, each SMS lands in the right account, including supplementary cards | Manual re-assignment of every transaction | **Say**: users complain SMS go to the default account and ask for supplementary cards | Differentiator | New (extends US 2.6) |
| 2 | **Cash that tracks itself** | An ATM SMS moves money to the Cash wallet and logs the ATM fee as its own expense. At night: "معاك 500 جنيه كاش؟" ("Do you have 500 EGP cash on you?") with one tap to confirm or fix | Cash is invisible in every app | **Say** (explicitly requested), and every other app | Differentiator | Planned (US 2.2, 2.3, 2.7) + **ATM fee parsing is new** |
| 3 | **Egyptian-dialect voice, many items at once** | Hold the mic: "دفعت 150 سوبرماركت و50 بنزين و20 مواصلات" ("I paid 150 at the supermarket, 50 for fuel and 20 for transport"). You get 3 cards to review and confirm with one tap. Franco-Arabic works too | Typing is friction, and cash spending is otherwise forgotten | Masareefy and Say do single voice logging. **Batch review + Franco-Arabic** is a step up | Table-stakes (in Egypt) | Planned (US 2.8) |
| 4 | **"Who owes who" (personal IOU ledger)** | Log "سلفت أحمد 500" ("I lent Ahmed 500") or "خالي سلفني 2000" ("my uncle lent me 2000"). See a balance per person, set a gentle reminder date, and send a polite WhatsApp reminder from a template. When an InstaPay "received" SMS arrives from that person, the app offers to settle the debt | Informal family and friend debts are never written down, which leads to awkwardness and forgotten money | **Splitwise** (3/day cap, no budget link). **Say** (users ask for debt entries). No Egyptian app has this | **Moat** (habit + social) | In SRS scope but **no user story yet. Write it.** |
| 5 | **Installment command centre** | One screen listing valU, Sympl, bank 0% plans, credit-card minimums and phone installments, with the next due date, "true cost incl. admin fees", and alerts at 7 days, 3 days, 24 hours and on the due day. Critical alerts bypass DND | Missed due dates bring penalties, and BNPL is spread across apps | **valU** (shows only its own installments), **Say** (basic tracking) | Differentiator | Planned (US 9.1, 5.1, 5.16) |
| 6 | **Salary-cycle budgets + daily "safe to spend"** | The budget resets on payday (e.g. the 25th). The home screen says "Safe to spend today: 180 EGP" and recalculates after overspending | Calendar months don't match Egyptian pay cycles, and the end-of-month crunch | All local apps (none advertise salary cycles). Copilot has a spending line but no salary cycle | Differentiator | Planned (US 3.1, 3.6) |
| 7 | **Partner sharing with privacy controls** | Invite a spouse with a code. Choose what to share (all, budgets only, or selected accounts). Both see shared budgets live and can **comment or react on a transaction** | Household money is managed in WhatsApp and arguments | **Say, Masareef, Flosy** (none have it). **Masareefy** (flat family plan). Honeydue-style comments are new to Egypt | Differentiator | Planned (US 1.3) + **comments are new** |
| 8 | **"Can I afford it?" Egyptian AI advisor** | Ask "أقدر أشتري لابتوب بـ 35 ألف الشهر ده؟" ("Can I buy a 35k laptop this month?") and get a yes, no or "yes if…" answer with the numbers, and a suggested plan (e.g. save 4,000/month for 9 months, or use the valU 12-month plan, with true cost shown) | Big purchase decisions are made blind | **Say** (no advisor), **Flosy** (chat without automated data), **Monarch/Cleo** (not in Egypt) | Differentiator | Planned (US 7.1) |
| 9 | **AI suggestions that never act without you** | Cards like "Move 300 from Dining to Groceries?" with Approve or Dismiss. Nothing changes silently | Trust in AI with money | Nobody advertises approval-based AI actions | Differentiator (trust) | Planned (US 7.2) |
| 10 | **App lock + "your SMS stay on your phone" promise** | PIN or biometric lock, and a clear privacy screen explaining what's read and what isn't | SMS permission feels scary | Masareef and Say use privacy as a selling point, so we need parity | Table-stakes | **New** |

### Should-have
| # | Feature | What the user experiences | Problem solved | Beats | Type | Status |
|---|---|---|---|---|---|---|
| 11 | **Gam'eya tracker** | Create a circle (members, monthly amount, your payout month). The app reminds you to pay, shows "you've paid 6/10, your turn is in March", and counts it as **savings**, not spending | Huge informal habit (Money Fellows has 8.5M users) that budgets ignore or treat as an expense | **Masrofi** (has Jameya but isn't Egyptian). **Say and the rest** have nothing | **Moat** (cultural) | **New** |
| 12 | **Kid accounts without a bank card** | Parent invites a child by code. Kids get a simple UI with allowance, goals and badges. The parent gets alerts when limits are crossed. At 16+ the teen can **graduate** and keep their history | Teaching kids money without opening a Telda or Klivvr card | **Klivvr, Telda, Zywa** (all need their card), **Greenlight** (US only) | Differentiator | Planned (US 1.2, 1.7) |
| 13 | **Subscription audit (price hikes, free trials, ghost subs)** | A badge reads "Netflix went up 20%", "Your trial ends in 2 days, here's how to cancel", "Gym: no related spending in 90 days, 2,400 EGP paid since" | Silent price hikes and forgotten subscriptions | **Say** has tracking and reminders but not hike, trial or ghost detection | Differentiator | Planned (US 3.4, 3.5, 3.7) |
| 14 | **Goals that live inside the budget** | A goal becomes a monthly budget line ("Vacation: 2,000/month"). Leftover budget can roll into it automatically. A simulator shows what happens if you add 500/month | Goals disconnected from daily spending | **Say** (users asked "goals should be calculated as monthly budget") | Differentiator | Planned (US 3.9, 4.1, 4.4) |
| 15 | **Investments snapshot (manual first)** | Add Thndr, mutual funds, gold, dollars or property with a manual value, and see total net worth. No trading | 3+ Say reviewers ask for it | **Say**, all local PFM apps | Differentiator | **New** |
| 16 | **Arabic receipt scan with item split** | Snap a supermarket receipt. Items are split between Groceries and Household automatically | Mixed baskets distort categories | Flosy and Masrofi only scan totals | Differentiator | Planned (US 2.9) |
| 17 | **Low-cash warning before payday** | "At this pace you'll run out on the 21st, 4 days before salary. Here are 3 ways to cut back" | End-of-month shortfall | **Say, Masareefy, Flosy** (none forecast) | Differentiator | Planned (US 5.8) |
| 18 | **Respectful notifications** | At most 3 non-urgent alerts a day, quiet hours, and urgent debt or fraud alerts always get through | Alert fatigue makes people uninstall | Nobody markets this | Differentiator | Planned (US 5.15–5.17) |

### Nice-to-have
| # | Feature | What the user experiences | Problem solved | Beats | Type | Status |
|---|---|---|---|---|---|---|
| 19 | **Zakat helper with gold price** | Shows your yearly Zakat estimate from savings, gold and cash, using the current gold price | Religious obligation calculated by hand | **Masrofi** (only one with it, not Egyptian) | Differentiator | **New** |
| 20 | **Bank rewards vs fees calculator** | "This 0% plan costs 450 admin fees; your points earn 120. Net cost: 330" | Hidden cost of "0%" offers | Nobody | Differentiator | Planned (US 9.2) |
| 21 | **Mini-map for cryptic merchants** | "POS POS 0482" shows a map pin where you were | Unrecognisable SMS merchant names | Nobody | Nice | Planned (US 2.10) |
| 22 | **Export and accountant-ready PDF** | Monthly PDF/CSV | Sharing with family or an accountant | Parity with **Say** and Masrofi | Table-stakes | Conflicting in our docs (see summary) |
| 23 | **Widgets & quick add** | Home-screen safe-to-spend and one-tap voice | Speed | Parity with **Say** and Masrofi | Table-stakes | **New** |

## B. Unique ideas no competitor has (creative / unconventional)
1. **Seasonal money modes:** pre-built Ramadan, Eid (eidiya list per child or relative), back-to-school (fees, uniforms, books), Sahel summer and wedding/gehaz modes. Each comes with typical categories, a countdown and a savings plan. *Nobody models the Egyptian money calendar.*
2. **Inflation-proof goals:** a goal like "iPhone" or "car down payment" can be tracked in **gold grams or USD equivalent**, so it stays realistic when the EGP moves. The app warns "your goal now costs 12% more than when you started".
3. **"Ask the family" approval:** a kid or partner can request money or approval for a purchase inside the app. The parent approves, and it's logged as allowance or a shared expense. (Logging only, no money transfer, which stays within our SRS's regulatory scope.)
4. **Polite debt reminder in Egyptian style:** pre-written, culturally appropriate reminder messages, from very gentle to firm ("فاكر الـ500 بتاعة الأسبوع اللي فات؟ 🙏", roughly "Remember the 500 from last week?"), sent through WhatsApp with an InstaPay link or handle if the lender adds one. It removes the awkwardness that stops people asking for their money back.
5. **Masroof-style AI persona with Egyptian humour:** optional Cleo-like "roast" or "sarcastic aunt" mode: "صرفت على الدليفري أكتر من الإيجار يا باشا" ("Pasha, you spent more on delivery than on rent"). Engagement through personality, and nobody does it in Arabic.
6. **Household "who paid" balance:** for couples or roommates, a running "you covered 3,200 more this month" balance that settles itself from shared transactions. It combines Splitwise with the family budget.
7. **Price-hike radar for local services:** detects increases across Egyptian telecom bundles, internet (WE), streaming and fuel-related spend, and tells you the monthly impact on your budget. It extends US 3.4 beyond subscriptions.
8. **Gam'eya organiser mode:** the person running a family gam'eya gets a members list, payment status for each member, and auto reminders to members. It works even if members don't use the app (share via WhatsApp). This could grow the user base: every circle brings in 10+ people.
9. **"Salary day" ritual:** on payday the app walks you through 60 seconds: pay installments first, fund gam'eya and goals, then show what's free to spend. It turns the paycheck into a habit moment.
10. **Spending "receipts" for kids:** kid accounts earn badges and a simple weekly story ("You saved 40 EGP this week, 60% of the way to your football!"), shareable with parents.

## C. Our positioning (one sentence)
> **"The only Egyptian money app that sees *all* your family's money (bank SMS, cash, installments, gam'eyas and the money friends owe you) and gives you an advisor who speaks your dialect and never moves a pound without your OK."**

Why someone picks us over Say: **Say tracks *your* card spending. We run your *household's* whole financial life, including the cash, debts and installments Say can't see.**

## D. MVP vs later phases

### MVP: the minimum that already beats Say
1. Smart SMS capture for Egyptian banks and wallets, with automatic account and card routing (#1)
2. Cash wallet: ATM → cash, ATM fee parsing, nightly cash check (#2)
3. Egyptian-dialect voice with batch confirm (#3) + quick manual entry
4. **Personal IOU ledger with WhatsApp reminders (#4)**
5. Installment command centre with escalating alerts (#5)
6. Salary-cycle budgets + safe-to-spend (#6)
7. Subscription tracking + renewal reminders (table stakes)
8. Partner sharing (#7)
9. "Can I afford it?" AI advisor + approval cards (#8, #9)
10. App lock + privacy screen, Arabic-first UI (#10)

*Why this set:* items 2, 4, 6 and 8 are things Say users asked for or Say doesn't have. Items 1, 3 and 7 match or beat Say's core. It's a superset of Say's value with a clear story.

### Phase 2 (next 3–6 months after MVP)
Gam'eya tracker (#11) · kid accounts + graduation (#12) · subscription audit (#13) · goals inside budgets + simulator (#14) · low-cash forecast (#17) · notification limits (#18) · receipt OCR split (#16) · widgets (#23) · seasonal money modes (Unique 1)

### Phase 3 (growth and moat)
Investment and net-worth snapshot (#15) · Zakat (#19) · rewards calculator (#20) · inflation-proof goals (Unique 2) · gam'eya organiser mode (Unique 8) · AI persona (Unique 5) · price-hike radar (Unique 7) · GPS mini-map (#21) · anomaly and fraud alerts · export · MENA expansion (Gulf SMS formats, Masrofi's turf)

### Things we suggest **de-prioritising** (from our own plan)
- **GPS mini-map (US 2.10)** and the **rewards calculator (US 9.2)**: no competitor or user evidence that people want them. Keep them for later.
- **Statement import (US 2.5)**: useful for onboarding history, but no local competitor needed it to win.
