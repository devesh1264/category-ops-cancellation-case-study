# Reducing Cancellations in Appliance Repair: A Category Operations Case Study

**Root-Cause Diagnosis & Fix Rollout Plan | Illustrative Home Services Marketplace ("HomeServe")**

📊 [**View the full presentation (PPTX)**](./HomeServe_Cancellation_Case_Study.pptx)

---

## Executive Summary

Diagnosed a rising booking cancellation rate (12% → 18% over two quarters) in HomeServe's Appliance & AC Repair category — a high-AOV, urgency-driven segment with low brand loyalty. Using issue-tree root cause analysis, isolated a **2–4 hour post-booking partner-confirmation gap** as the primary driver. Designed a real-time partner-matching fix, validated through a phased single-city pilot, projecting **~₹5.97L/year in recovered platform revenue** against a **~24-month payback period**.

*All figures in this case study are illustrative and clearly labeled as assumptions for demonstration purposes — not real company data.*

---

## 1. Problem Context

HomeServe's Appliance & AC Repair category — defined by urgency-driven, low-loyalty demand and the highest average order value (₹800) among comparable categories — saw cancellation rates climb from **12% to 18%** over the past two quarters.

**Why this category, why now:**
- **Seasonality** — demand spikes sharply in summer, exactly when customer patience is lowest.
- **Low brand loyalty** — one-off, urgent bookings drive multi-app hedging behavior.
- **High AOV** — each cancellation is disproportionately expensive.
- **Competitive pressure** — informal repair networks compete on confirmation speed, not price.

**Business impact:** direct GMV loss, CSAT/trust erosion suppressing future repeat bookings, and wasted partner-matching effort — a compounding, not isolated, cost.

---

## 2. Data Insights (Illustrative)

| Metric | Value |
|---|---|
| Total bookings / quarter | ~24,000 |
| Average Order Value | ₹800 |
| Overall cancellation rate | 18% |
| Customer-initiated cancellations | 65% |
| Partner-initiated cancellations (no-shows) | 35% |
| Customer cancellations within 2–4 hrs of booking | 55% |
| Cancellation drop once partner + ETA shown | ~60% |

**Key insight:** two separable problems — a larger, addressable demand-side pre-confirmation gap, and a smaller supply-side peak-hour availability gap.

---

## 3. Root Cause Analysis

Issue-tree breakdown (MECE) across Demand-side, Supply-side, and Process/Operational branches:

| Branch | Key Drivers |
|---|---|
| **Demand-side** | Multi-app booking/hedging, no post-booking status visibility, price–urgency mismatch |
| **Supply-side** | Partner unavailability, flat pay (no peak-hour incentive), late-discovered parts mismatch |
| **Process/Operational** | Slow manual assignment confirmation (2–4 hrs), no interim communication, no dynamic peak routing |

**Selected root cause:** the **2–4 hour post-booking, pre-confirmation assignment gap** — it sits at the intersection of both demand and supply symptoms, and directly matches the data's 55% cluster window.

---

## 4. Fix Prioritization (MoSCoW)

| Fix | Root Cause Addressed | Priority | Reason |
|---|---|---|---|
| Real-time automated partner matching | Slow assignment confirmation | **Must Have** | Directly attacks the highest-leverage branch |
| Interim status updates | No interim communication | **Must Have** | Cheap, immediate wait-perception reduction |
| Dynamic peak-hour partner incentive | Flat pay → no-shows | **Should Have** | Addresses secondary root cause |
| Pre-booking part/tool checklist | Late-discovered mismatch | **Could Have** | Smaller contributor, phased in later |
| Loyalty/pricing lock for repeat customers | Not tied to identified root cause | **Won't Have** | Out of scope for this fix cycle |

---

## 5. Solution Design — AS-IS / TO-BE

**AS-IS (2–4 hrs):** Booking → manual/batch partner review → manual notify/accept/decline → re-queue on decline → customer sees "Partner Assigned."

**TO-BE (<15 min):** Booking → automated real-time proximity matching → instant interim status shown to customer → best-match partner auto-notified (3-min accept window) → auto-reassignment on decline → named partner + live ETA shown.

---

## 6. Cost-Benefit & ROI Analysis (Illustrative)

| Metric | Estimated Value | Basis |
|---|---|---|
| Bookings recovered / month | ~311 | 60% reduction in confirmation-gap cancellations |
| GMV recovered / month | ~₹2.49L | 311 × ₹800 AOV |
| Platform revenue recovered / year | ~₹5.97L | At 20% take rate |
| Implementation cost | ~₹9.5L – ₹14.5L (one-time) | Matching engine + status UI build |
| Ongoing cost | ~₹50,000/year | Infra/maintenance |
| **Payback period** | **~24 months** | Realistic for an engineering build, not overclaimed |

*The ROI model deliberately excludes the longer-term trust/repeat-booking benefit rather than forcing a speculative multiplier onto it.*

---

## 7. Pilot & Go-To-Market Plan

| Phase | Timeline | Scope |
|---|---|---|
| **Phase 1 — Pilot** | Weeks 1–6 | One mid-sized city, AC repair only |
| **Phase 2 — Wave Expansion** | Months 2–4 | 4–5 similar-tier cities |
| **Phase 3 — Full Rollout** | Months 5–6 | All active cities |
| **Phase 4 — Post-Launch** | Ongoing | Standing category health metric |

**Pilot success bar (set before launch):**
- Confirmation-gap cancellations drop ≥5 points within 6 weeks
- Partner utilization does not drop >5%
- CSAT holds steady or improves
- Partner-initiated no-show rate does not rise

---

## 8. Success Metrics & Expected Impact

**North Star:** Confirmation-gap cancellation rate
**Supporting:** Overall cancellation rate, fill rate, partner utilization, CSAT, repeat booking rate (next-season cohort)

**Causal chain:** Real-time matching → confirmation-gap cancellations drop → overall cancellation rate falls → GMV/revenue recovered + CSAT improves → multi-app hedging reduces → repeat booking rate improves next season.

---

## 9. Risks & Mitigations

| Risk | Mitigation |
|---|---|
| Partner concentration (jobs routed to same top partners) | Weight matching by proximity/speed **and** fair rotation |
| Rushed/mismatched assignments | Keep skill/proximity as hard constraints before optimizing for speed |
| Partner attrition from tighter timeouts | Track no-show rate/utilization; timeout is tunable |
| Over-promised ETA | Show live/dynamic estimate, not a flat promise |
| Secondary root cause neglected | Explicitly scheduled for Phase 2/3, not abandoned |

---

## 10. Key Takeaway

Operational bottlenecks in a two-sided marketplace are rarely about "trying harder" — they're about closing structural visibility gaps. A narrow, well-diagnosed fix (real-time matching + status transparency) can resolve the majority of a rising-cancellation problem without touching pricing, partner economics, or the broader product, while explicitly sequencing secondary fixes rather than ignoring them.

---

### Methodology Note

This is an independent case study built to practice category-operations problem-solving (root cause analysis, prioritization frameworks, unit economics, GTM design). All company names, figures, and datasets are illustrative and clearly labeled throughout — not real data from any specific company.

**Author:** Devesh Rathod | B.Tech. Electrical & Electronics Engineering, VNIT Nagpur
