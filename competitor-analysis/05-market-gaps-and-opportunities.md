# 05 · Table Stakes, Differentiators, Market Gaps & Egypt Opportunities

> Evidence links point to sources listed in [07-sources.md](07-sources.md). "Evidence strength" reflects how directly users asked for the thing.

## 1. Table-stakes features (everyone has them, so we must too)
| Feature | Who has it | Our plan |
|---|---|---|
| Automatic transaction capture (SMS in Egypt, bank sync globally) | Say, Masareef, Masareefy, Masrofi, all global leaders | ✅ US 2.6 |
| Auto-categorisation with editing | Almost all | ✅ |
| Category budgets with progress bars and over-limit alerts | Almost all | ✅ US 3.2, 5.3, 5.4 |
| Subscription and recurring-payment detection with renewal reminders | Say, Masareef, Masrofi, Rocket, Monarch, Copilot | ✅ US 3.3, 5.7 |
| Spending reports (category, period, trends) | All | ✅ Feature 6 |
| Arabic RTL + English UI (in Egypt) | All local apps | ✅ global requirement |
| Fast manual and cash entry | All | ✅ US 2.1 |
| Privacy promise and app lock | Say, Masareef, Flosy, Masrofi | 🟡 not explicit in our docs. **Add app lock (PIN/biometric).** |
| Widgets / quick add | Say, Masrofi | ❌ not in our docs. **Add.** |
| Free tier + cheap Pro in EGP | Say (EGP 99.99/month) | ❓ not defined |

## 2. Differentiators (only 1–2 competitors have them)
| Feature | Who has it | Our plan |
|---|---|---|
| Egyptian-dialect voice logging | Say, Masareefy | ✅ US 2.8, plus multi-item batch review |
| Household / partner sharing | Masareefy (flat family plan), Monarch, Goodbudget, Honeydue | ✅ US 1.3, with role hierarchy |
| Kid accounts with parent oversight | Klivvr, Telda, Zywa, Greenlight (all card-based) | ✅ US 1.2, SMS-based with no card needed |
| AI chat about my money | Flosy, Masrofi, Wally, Monarch, Cleo | ✅ US 6.9 / 7.1 |
| Gam'eya / Jameya tracking | **Masrofi only** | ❌ **gap in our plan** |
| Zakat + gold | **Masrofi only** | ❌ gap |
| Subscription cancellation done for you | **Rocket Money only** | ❌ not suited to Egypt; we provide instructions instead (US 3.5) |
| Installment & credit-card tracking | Say (basic) | ✅ Feature 9, much deeper |
| Personality / humour in the AI | Cleo | ❌ opportunity |
| In-app chat / comments on shared transactions | Honeydue | ❌ opportunity |

## 3. Market gaps: unmet needs with evidence
| # | Unmet need | Evidence | Strength | Who fails today |
|---|---|---|---|---|
| G1 | **ATM withdrawal should move money to a cash wallet automatically; parse ATM fees** | Say review: "ATM withdrawals need automatic cash account transfers… ATM fees should parse from bank SMS" (App Store EG, 9 May) | **Strong (direct ask)** | Every app. We plan it (US 2.7) |
| G2 | **SMS from different banks and cards must land in the right account automatically** | Say review: "All bank SMS messages are automatically assigned to the default account… I have to manually move almost every transaction" (2 Aug). Another reviewer asked for supplementary card support | Strong | Say (the feature exists but users don't discover it) |
| G3 | **Debts, assets and more accounts** | Say review: "Can we allow above 3 accounts?" plus debt and asset entries (1 Aug) | Strong | Say (3-account cap, no debts) |
| G4 | **Scheduled payments, installments, semi-annual bills; goals as part of the monthly budget** | Say review "APP MUST DO MODIFICATIONS" (24 Jul) | Strong | Say |
| G5 | **Investment tracking** (Thndr, mutual funds, stocks, crypto, real estate) | 3 separate Say reviews (Cherifefarid 6 Jun, Anas S 23 May, ItsMoWaly 24 Jul) | **Strong (repeated)** | All Egyptian PFM apps. Only Telda shows its own investments |
| G6 | **One view of all installments** across valU, Sympl, bank 0% plans and cards | valU shows only valU installments (902k users, 23% share). Our docx lists ValU/Sympl/CIB/NBE 0% as targets | Medium (structural) | valU, banks, Say (basic) |
| G7 | **Personal IOUs that also hit my budget correctly** | Splitwise's free tier is capped at ~3 expenses/day with ads, and users complain (Kimola report). No Egyptian PFM app has an IOU ledger | Medium | Splitwise, all local apps |
| G8 | **Tracking family and colleague gam'eyas** (informal ROSCAs) | Money Fellows has 8.5M users for digital circles, which shows the habit is huge. Informal circles outside apps are untracked. Only Masrofi offers Jameya tracking | Medium (behavioural, indirect) | Everyone except Masrofi |
| G9 | **Household view without needing a new bank card** | Klivvr/Telda family features require their cards. Masareefy's family plan is flat. No Egyptian PFM app has a role hierarchy | Medium | Klivvr, Telda, Masareefy |
| G10 | **Affordable pricing** | Global leaders cost $95–110/year. Say is ≈ EGP 700/year, and reviewers still ask for more value | Medium | Global apps |
| G11 | **Budgets that follow the salary date** | Our docx: Egyptian salaries often run 25th → 24th. No local competitor advertises this | Low–Medium (our own insight) | All local apps |
| G12 | **Bank sync that doesn't break** | The top complaint for YNAB, Monarch and Wallet | Strong (global) | Aggregator-based apps. SMS avoids this |

## 4. Egypt-specific opportunities

### Where global players fail locally
1. **No data source.** Plaid, Finicity and PSD2 don't cover Egyptian banks, so YNAB, Monarch, Copilot, Rocket and Cleo are basically manual apps in Egypt.
2. **iOS-first.** Copilot has no Android, yet Android is about 69% of Egyptian traffic vs about 6.7% for iOS.
3. **USD pricing.** $100/year is a large share of an Egyptian monthly salary (inferred, Low).
4. **No Arabic, no Egyptian dialect, no cash culture.** Cash wallets and ATM logic are missing everywhere.
5. **US-specific services** (bill negotiation, credit score, cancellation concierge) don't transfer to Egypt.

### Where local players are weak
| Local player | Weakness we can exploit |
|---|---|
| **Say** | No family features, no IOUs, no real goals engine, no AI advisor, 3-account free cap, ATM/cash gap, SMS routing friction. Investments requested but missing. UI language listed as English only |
| Masareef / Masareefy / Flosy | Tiny traction (1–2 ratings), single-feature focus. Flosy is iOS only |
| Telda / Klivvr | Only see their own card, with no budgets across all money |
| Money Fellows / valU | Product-specific, no holistic view |
| Masrofi (MENA) | Not Egypt-specific: no Egyptian dialect, no cash/ATM, no installments. Priced in USD |

### Opportunities ranked
1. **"All my money, including cash and what people owe me"**: SMS + ATM-to-cash + IOU + gam'eya in one ledger. Nobody has all four.
2. **Family finance without a new bank card**: partner + kids built on the SMS data the family already gets.
3. **Installment command centre**: valU, Sympl, bank 0% and cards, with penalty-first alerts. Egyptians widely use BNPL (valU alone has 902k users), and nobody aggregates it.
4. **Egyptian-voiced AI advisor**: "أقدر أشتري لابتوب بـ 35 ألف؟" ("Can I afford a 35k laptop?"), with approval cards. Say has no advisor, Flosy has chat but no automation.
5. **Culture-native money moments**: Ramadan, Eid (eidiya), back-to-school, summer (Sahel), wedding prep (gehaz), Zakat. Only Masrofi touches Zakat.
6. **Inflation-aware goals.** EGP volatility makes fixed EGP goals go stale. Goals could track real value, e.g. pegged to gold or USD (opportunity, Low evidence: no user quote found).
