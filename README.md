# MarTech Architecture & CDP Strategy — Threadline Apparel

**Rutgers MSMAI Consulting Engagement | Spring 2026**
**Role: Engagement Lead, 6-person team**
**Budget: $200,000 | Timeline: 90-Day Impact Plan**

---

## Project Overview

A multi-channel apparel retailer ("Threadline") had a fully-assembled MarTech stack — Shopify, Klaviyo, Meta, Google Ads, GA4, Gorgias, Yotpo, and Square POS — but none of it was properly connected. The result was three specific, measurable failures costing the business real revenue every month.

This engagement delivered a full MarTech architecture proposal: stack assessment, Segment CDP design, 3 customer journey maps, a plain-language BRD, activation strategy with suppression rules, a 7-KPI measurement plan, and a sequenced 30/60/90-day implementation roadmap.

---

## The Three Core Problems

| Problem | Hard Number | Business Impact |
|---|---|---|
| **Identity Fragmentation** | 3–5 profiles per customer | Same customer exists across Shopify, Square, and Klaviyo as separate records. Every segment is built on wrong data. |
| **Data Timing Gaps** | 24–72 hr store lag | In-store purchase data arrives late. Customers receive cart-abandon emails for items they already bought. |
| **No Single Source of Truth** | 3 conflicting dashboards | Shopify, GA4, and Klaviyo report different revenue numbers. Leadership cannot make confident budget decisions. |

**The fix (one sentence):** CDP + 3 automated journeys + 1 reporting layer = measurable impact in 90 days within $200K.

---

## Deliverables

### 1. Customer Journey Maps
Three end-to-end journeys mapped with current failure points, the fix, and 90-day KPI targets:

- **Journey 1 — Cart Abandonment:** Sub-45-min trigger via Shopify webhook → Klaviyo. Target: +10–15% cart recovery rate, +$7.5K–$15K/month revenue lift.
- **Journey 2 — First Purchase to Repeat Buyer:** 6-touchpoint post-purchase flow (Day 0–45). Target: +5–8 pts in 30-day repeat rate, support tickets down 20%.
- **Journey 3 — Lapsed Customer Winback:** CDP-segmented 3-email sequence with auto-exit. Target: 8–12% winback conversion.

### 2. Prioritized Use Cases (P0/P1/P2)
Business problems translated into concrete requirements with priority levels. Four P0 requirements must work at launch: unified profile within 24hrs, suppression auto-fires within 2hrs, full cart line items in email, no engineering required for day-to-day ops.

### 3. Current Stack Assessment
Eight tools audited. Seven stay with fixes. One retired (spreadsheet reporting). One added (Segment CDP).

| System | Decision |
|---|---|
| Shopify | KEEP + FIX |
| Klaviyo | KEEP + UPGRADE |
| Meta + Google Ads | KEEP + FIX |
| GA4 | KEEP + FIX |
| Gorgias | KEEP + INTEGRATE |
| Yotpo | KEEP + CONNECT |
| Square / Lightspeed | KEEP + FIX |
| Spreadsheet Reporting | **RETIRE** |
| **Segment CDP** | **ADD — NEW** |

### 4. Business Requirements Document (BRD)
Four business outcomes with supporting functional requirements:
- **BR-01:** Stop wasting ad spend — suppress purchasers within 2 hrs (ecomm) / 24 hrs (store)
- **BR-02:** Increase repeat purchase rate — 3 automated journeys
- **BR-03:** One KPI source of truth — Looker Studio, agreed definitions
- **BR-04:** No single-person bottleneck — documented flows with named secondary owners

### 5. Future-State Stack Design (Segment CDP Architecture)
Segment CDP as the identity resolution hub connecting all data sources to all destinations. Architecture diagram included in the presentation deck.

| Layer | System | Cost |
|---|---|---|
| Identity Hub | Segment CDP (NEW) | ~$36–60K/yr |
| Email + SMS | Klaviyo (Upgraded) | ~$20–25K/yr |
| Reporting | Looker Studio + Supermetrics | ~$12–15K/yr |
| All others | Existing stack (fixed) | Existing costs |

### 6. Information Flow Map
Every data connection mapped: source → destination, data type, speed, and integration method.

Key SLAs:
- Shopify order events → CDP: **< 5 minutes**
- POS suppression: **< 24 hours**
- Paid media suppression list refresh: **< 2 hours**

### 7. Activation Strategy
Four audience segments + six suppression rules with specific trigger windows. Notable rules: online purchasers suppressed from all retargeting within 2 hrs; customers with open support tickets suppressed from all promos in real-time; full-price buyers excluded from discount promos for 21 days.

### 8. Measurement Plan — 7 KPIs, 1 Source of Truth Each

| KPI | 90-Day Target | System of Record |
|---|---|---|
| Cart Recovery Rate | +10–15% lift | Klaviyo |
| Suppression Overlap Rate | <2% overlap | Meta Ads Manager + Google Ads |
| 30-Day Repeat Purchase Rate | +5–8 pts | Shopify |
| Support Ticket Rate (Order Status) | Down 20% | Gorgias |
| Winback Conversion Rate | 8–12% of lapsed | Shopify + Klaviyo |
| Email Unsubscribe Rate | <0.3% per send | Klaviyo |
| Identity Resolution Rate | 85%+ matched | Segment CDP |

Attribution rule: if Shopify revenue and any attribution tool differ by >8%, the discrepancy is investigated before any budget decision is made.

### 9. 30/60/90-Day Roadmap

| Phase | Days | Milestone |
|---|---|---|
| Stop the Bleeding | 1–30 | CDP live, suppression <2 hrs, ~$8K/mo wasted spend stopped |
| Build the Machine | 31–60 | Single customer view live, first journey active, one dashboard |
| Prove the ROI | 61–90 | Three journeys live, KPI dashboard, attribution governance enforced |

---

## Financial Case

| | Monthly | Annual |
|---|---|---|
| **Cost of inaction** | $22.5K–$40K/mo | $180K–$360K/yr |
| **Total investment** | — | $200K (one time) |
| **Projected return** | — | **$270K–$480K annualized** |
| **Payback period** | — | **Under 90 days** |

---

## Files in This Repo

| File | Description |
|---|---|
| `Threadline_Report_Updated.docx` | Full written report — executive summary, all 9 outputs, financial case |
| `Threadline.pdf` | Presentation deck — 24 slides delivered to client stakeholders |

---

## Skills Demonstrated

`CDP Architecture` · `MarTech Stack Assessment` · `Customer Journey Mapping` · `Business Requirements (BRD)` · `KPI Framework Design` · `Segment CDP` · `Klaviyo` · `Looker Studio` · `Data Governance` · `Lifecycle Marketing` · `Audience Segmentation` · `B2C Retail Analytics` · `ROI Modeling`

---

## Context

- **Course:** Rutgers MSMAI — Marketing Technology, Spring 2026
- **Engagement type:** 12-week B2B consulting project
- **Role:** Engagement lead, 6-person team
- **Client:** Multi-channel apparel retailer (anonymized as "Threadline")
- **Anonymization:** All client identifiers have been removed. "Threadline" is the approved pseudonym used throughout.
