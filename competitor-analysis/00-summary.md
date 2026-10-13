# 00 · Summary: Competitor Analysis & Feature Ideas

*Prepared 2026-10-03. Scope: product idea and features only (no tech or implementation).*

## ⚠️ Ambiguities found in our own files (and what we assumed)
| # | Conflict | Where | Interpretation used |
|---|---|---|---|
| 1 | **Product name** is unclear: "Personal Finance Advisor" in the docx, while the LICENSE copyright says "CachePay" | docx title, LICENSE | Treated "CachePay" as the team/brand name and "Personal Finance Advisor" as the working product title. We say "our app" throughout |
| 2 | **Bank account linking**: the SRS says it's *out of scope*, but the docx lists "connecting a bank account through an authorized aggregation service" plus a "simulated bank connection" as supplementary channels | srs-draft.md §3 vs docx §4.2.5 | **SMS-first, no live bank linking.** Statement import stays as a secondary option |
| 3 | **Report export**: US 6.10 and US 1.6 include PDF/CSV/JSON export, but docx §8.5 says "no external file exports… are required" | User Stories vs docx | Export kept as a **later-phase, parity feature** (Say has it) |
| 4 | **Informal IOU / peer debt ledger**: a headline capability in the SRS (problem statement + scope), but **no user story or use case** defines it. Feature 9 only covers formal card debt and installments | srs-draft.md vs User Stories / use-case-mapping | Treated as **planned but unspecified**, and recommended as a **Must-have** to write up |
| 5 | **Kid accounts and email**: the docx requires an email for kids, while US 1.5 assumes kids may have no email | docx §3.2 vs US 1.5 | Minor. No impact on competitor analysis |
| 6 | **Subscription alerts**: US 3.4/3.5 say "no push" for price hikes and trials, but US 5.7 pushes renewal reminders | User Stories | Treated as intentional: renewals push, audits stay in-app |
| 7 | **Platform**: SMS reading works only on Android, and iOS isn't addressed | All docs | Assumed **Android-first** (supported by Egypt's 69% Android share) |
| 8 | **Target market**: "Egyptian market" throughout, nothing about expanding beyond it | SRS, docx | **Egypt first**, with MENA as a possible later step |
| 9 | Registration diagram 1.1 (PlantUML version) includes "Username", but the stories don't | Diagrams/1.1/1.png vs US 1.1 | Minor |

## What our product is (from Step 0)
- **Idea:** an AI-powered, Arabic-first, mobile **household finance app for Egypt**. It acts as a "digital accountant" for individuals **and families**.
- **Problem:** Egyptians' money is scattered across cash, e-wallets, bank cards, informal IOUs and installments, and nobody tracks household spending or installment penalties.
- **Target users:** (1) individuals managing salary, subscriptions and goals; (2) couples sharing budgets; (3) parents monitoring kids through sub-accounts.
- **Planned features:** 9 feature areas, 67 user stories and 37 use cases:
  1. Household accounts: primary, partner, kid, detach, graduate.
  2. Capture: SMS, voice, OCR, cash wallet + ATM sync, GPS, import.
  3. Salary-cycle budgets and subscription audit.
  4. Goals with a simulator.
  5. Smart notifications (DND, rate limits).
  6. Reports.
  7. AI chat with "can I afford it?".
  8. Multi-agent system with approval cards.
  9. Installments, rewards and debt strategy.
- **Market:** Egypt first (EGP, Egyptian banks and wallets: CIB, NBE, Banque Misr, QNB, HSBC, InstaPay, Vodafone/Etisalat/Orange Cash).

## Key findings
1. **"Say" is Say – Hands free budget app (sayapp.net)**, an Egypt-focused bank-SMS + voice expense tracker. It has a 4.8★ rating from about 2.6k ratings on the Egyptian App Store and charges **EGP 99.99/month or EGP 699.99/year**. It's our closest and strongest direct competitor (High confidence).
2. **Say's weak spots come from its own users.** They ask for ATM → cash automation, correct SMS-to-account routing, more than 3 accounts, debt entries, goals tied to budgets, installments and **investment tracking**. **Our plan already covers most of these**, except investments.
3. **Say has no household, kid, IOU, AI-advisor or goals-engine features.** Our household + IOU + advisor combination is the clearest gap.
4. The **other Egyptian PFM apps** (Masareef, Masareefy, Flosy) are very early (1–2 ratings each). Masareefy is the only one with a family plan.
5. **Neobanks** (Telda, Klivvr) and **product apps** (valU, Money Fellows, InstaPay) are large, but each only sees its *own* money. Nobody aggregates installments or gam'eyas.
6. **In MENA, Masrofi** has the most culturally native feature set (190+ MENA bank SMS, Jameya, Zakat, offline AI) but isn't Egypt-specific. **Gulf apps rely on open banking**, which Egypt lacks.
7. **Global leaders** (YNAB, Monarch, Copilot, Rocket Money, Cleo) cost about **$95–110/year**, rely on aggregators that don't cover Egypt, and are mostly English-only. Copilot has no Android at all. **They're effectively absent in Egypt.**
8. On paper, **our planned feature set is a superset of Say's**. The real gaps in our plan are an **IOU user story**, **gam'eya tracking**, **investments/net worth**, **app lock**, and **widgets**.

## Top 10 recommended features (details in [06](06-suggested-features.md))
| # | Feature | Type | Priority |
|---|---|---|---|
| 1 | Smart SMS routing with zero setup (auto-detects banks, cards, supplementary cards) | Differentiator | Must |
| 2 | Cash that tracks itself (ATM → cash + **ATM fee parsing** + nightly cash check) | Differentiator | Must |
| 3 | **Personal IOU ledger** with polite WhatsApp reminders and InstaPay settlement matching | **Moat** | Must |
| 4 | Installment command centre (valU, Sympl, bank 0%, cards) with escalating alerts | Differentiator | Must |
| 5 | Egyptian-dialect multi-item voice logging with batch confirm | Table-stakes (Egypt) | Must |
| 6 | Salary-cycle budgets + daily "safe to spend" | Differentiator | Must |
| 7 | Partner sharing with privacy controls + comments on transactions | Differentiator | Must |
| 8 | "Can I afford it?" Egyptian AI advisor with approve-only action cards | Differentiator | Must |
| 9 | **Gam'eya tracker** (counted as savings, with turn reminders) | **Moat** | Should |
| 10 | Kid accounts without a bank card, plus graduation | Differentiator | Should |

## Positioning
> **"The only Egyptian money app that sees *all* your family's money (bank SMS, cash, installments, gam'eyas and the money friends owe you) and gives you an advisor who speaks your dialect and never moves a pound without your OK."**

Short version against Say: **Say tracks your card spending. We run your household's whole financial life.**

## MVP in one line
Smart SMS capture · self-tracking cash · Egyptian voice · **IOU ledger** · installment centre · salary-cycle budgets + safe-to-spend · subscriptions · partner sharing · "can I afford it?" advisor with approval cards · app lock + Arabic-first UI.

## Honesty notes
- **Reddit was blocked** to our crawler, so user complaints come from App Store reviews and review-analysis sites instead.
- **Google Play pages didn't render**, so Android ratings and downloads for Say and others aren't captured.
- **Telda's rating** came back identical to Say's, so it's treated as unverified.
- **"❌" in the matrix means "not found in public sources"**, not proven absent.
- Masrofi's country is inferred, and the Egyptian bank apps weren't analysed.

## Files
- [01-egypt-competitors.md](01-egypt-competitors.md): Say (deep dive), Masareef, Masareefy, Flosy, Telda, Klivvr, Money Fellows, valU, InstaPay, Splitwise, plus market context
- [02-mena-competitors.md](02-mena-competitors.md): Masrofi, Wally, Tadbeer, Zywa, Hakbah, Tarabut
- [03-global-competitors.md](03-global-competitors.md): YNAB, Monarch, Copilot, Rocket Money, Cleo, Goodbudget, Honeydue, Splitwise, Greenlight, Wallet, Money Manager, axio
- [04-feature-matrix.md](04-feature-matrix.md): 50+ features × 17 products, including ours
- [05-market-gaps-and-opportunities.md](05-market-gaps-and-opportunities.md)
- [06-suggested-features.md](06-suggested-features.md)
- [07-sources.md](07-sources.md)

---

## Step 0: files read (32 total: 5 text, 1 Word, 1 Excel, 25 images; all readable)
| # | File | How it was read | Content |
|---|---|---|---|
| 1 | `README.md` | Text | Placeholder heading only ("# docs") |
| 2 | `LICENSE` | Text | MIT, © 2026 CachePay |
| 3 | `srs-draft.md` | Text | Product overview, problem, scope, out-of-scope |
| 4 | `use-case-mapping.md` | Text | Actors, 37 use cases, mapping to stories |
| 5 | `User Stories.md` | Text | 9 features, 67 user stories with acceptance criteria |
| 6 | `Personal_Finance_Advisor_Requirements-1.docx` (untracked) | Text extracted from the Word XML with Python | Full requirements spec v1.0 (Sep 2026) |
| 7 | `Gantt Chart.xlsx` | **Deleted in the working tree.** Recovered from git `HEAD` with `git show`, then parsed with Python | 34 tasks, P0–P6 phases (127 days). Includes "Requirement gathering & competitor research" |
| 8–9 | `Diagrams/Use Case/1.1/1.png`, `2.png` | Image | Registration use case (two styles) |
| 10–11 | `Diagrams/Use Case/1.2/1.png`, `2.png` | Image | Kid sub-account |
| 12 | `Diagrams/Use Case/1.3/1.png` | Image | Partner sharing |
| 13 | `Diagrams/Use Case/1.4/1.png` | Image | Detachment |
| 14 | `Diagrams/Use Case/1.5/1.png` | Image | Account recovery |
| 15 | `Diagrams/Use Case/1.6/1.png` | Image | Account deletion |
| 16 | `Diagrams/Use Case/1.7/1.png` | Image | Account graduation |
| 17–20 | `Diagrams/Use Case/2/2.1.png` – `2.4.png` | Image | Manual expense, cash check, cash adjust, search |
| 21 | `Diagrams/Use Case/2.5/1.png` | Image | Bulk import |
| 22 | `Diagrams/Use Case/5.11/5.11.png` | Image | AI recommendation nudges |
| 23–29 | `Diagrams/Use Case/6/6.1.png` – `6.7.png` | Image | Reports (cash flow, category, budget vs actual, goals, MoM, subscriptions, top merchants) |
| 30 | `Diagrams/Use Case/6.9/6.9.png` | Image | AI natural-language query |
| 31 | `Diagrams/Use Case/7.1/7.1.png` | Image | AI affordability query |
| 32 | `Diagrams/Use Case/7.2/7.2.png` | Image | AI action-card authorization |

**Files that couldn't be read: none.** The docx and xlsx were extracted with Python's standard library (no extra packages were installed), and the docx contained no embedded images. All 25 diagrams match the user stories; only the Username difference (ambiguity #9) stood out.
