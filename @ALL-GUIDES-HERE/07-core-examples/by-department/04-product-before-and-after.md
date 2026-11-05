# Product Before / After

> What a real person in this department gets BEFORE the system vs. AFTER.

---

## The Situation

Maya is a Senior PM at a 100-person Series A developer tools company. The CEO asked for a customer-facing analytics dashboard "by end of next quarter." Maya needs a PRD that engineering will not laugh at, that design can scope from, and that won't get torn apart in the roadmap review on Tuesday.

---

## ❌ Before: What They Wrote Without the System

> **PRD: Analytics Dashboard**
>
> **Overview**
> We will build a customer-facing analytics dashboard. Users have been asking for this. It is a P0 for next quarter.
>
> **Problem**
> Customers do not have visibility into how they are using the platform. They want to see their usage data and understand trends.
>
> **Solution**
> A dashboard inside the product that shows users their key metrics. The dashboard will have charts and visualizations that allow users to track their usage over time and identify patterns.
>
> **Features**
> - Usage charts
> - Filters by date range
> - Export to CSV
> - Customizable views
> - Email reports
>
> **Success Metrics**
> - Adoption
> - User satisfaction
> - Reduction in support tickets
>
> **Timeline**
> End of Q2.
>
> **Open Questions**
> - What charts to include?
> - Pricing implications?
> - Mobile?

Engineering will read this and ask the same five questions Maya did not answer. Design has nothing to scope from. The CEO will love it because it is short. The roadmap review will eat it alive because it does not address the obvious overlap with the BI integration already in development.

---

## ✅ After: What the System Produced

> **PRD: Customer-Facing Analytics Dashboard (v1)**
> **Owner:** Maya. **Eng Lead:** Tomás. **Design:** Priya. **Status:** Draft for roadmap review.
>
> ---
>
> **Problem Statement**
>
> 7 of our top 20 customers raised "no visibility into our own usage" in Q3 QBRs (source: CS interview log, weeks 36 to 39). Specifically:
>
> 1. Admins cannot see which teammates are using the product.
> 2. Finance buyers cannot tie usage to ROI at renewal time.
> 3. Power users cannot self-serve "am I close to my quota" questions, which generates ~40 support tickets per week (source: Zendesk tag report).
>
> This is a renewal risk. 3 of those 7 customers are up for renewal in Q1.
>
> ---
>
> **Goal**
>
> Give customers self-serve visibility into their own usage, framed around the three jobs above (admin oversight, ROI evidence, quota self-check).
>
> ---
>
> **Success Metrics (90 days post-launch)**
>
> 1. **Adoption:** 40% of paid customers have an active user view the dashboard at least once per month.
> 2. **Job 3 (quota self-check):** Reduce "usage / quota / am I close" support tickets by 50% (baseline: 160/month).
> 3. **Renewal signal:** 3 of 3 at-risk renewal accounts cite the dashboard as positive in renewal call notes.
>
> Anti-metric: dashboard becomes a vanity surface that doesn't move support volume. Kill criterion at 90 days.
>
> ---
>
> **Scope**
>
> **In v1:**
> - Per-account usage by user, by feature, by week
> - Quota tracking with threshold alerts
> - 90-day historical view
> - CSV export (one button)
>
> **Out of v1 (parking lot, not "no"):**
> - Custom dashboard builder
> - Email digest reports
> - Mobile app view (web responsive only)
> - Cross-account benchmarking
>
> **Explicitly NOT in scope:**
> - BI tool replacement. The Looker integration on the Q3 roadmap covers deep analytics. This dashboard is for everyday self-serve, not analyst workflows.
>
> ---
>
> **Tradeoffs (build vs. buy)**
>
> | Option | Time to ship | Cost | Lock-in | Decision |
> |--------|--------------|------|---------|----------|
> | Build in-house | 10 weeks | 1.5 eng | None | **Recommended for v1.** Fits our data shape. |
> | Embed Metabase | 4 weeks | $1.2K/mo | Medium | Faster, but data model export creates a 2-week prep job and the UX won't match our design system. |
> | Embed Looker (Google) | 12 weeks | $4K/mo | High | Already chosen for the BI integration. Different use case. |
>
> ---
>
> **Tech Constraints (flagged with Tomás)**
>
> - Our event pipeline currently retains 30 days of granular events. 90-day view requires extending retention or building a daily rollup table. Tomás recommends rollup table. 1 week of work.
> - Multi-tenancy: dashboard data isolation must pass the same security review as the API. SOC 2 boundary.
> - Performance: dashboards over 50K events/account need pagination or pre-aggregation. ~12 customers exceed this today.
>
> ---
>
> **Open Questions (with owners and dates)**
>
> | Question | Owner | Decision by |
> |----------|-------|-------------|
> | Pricing: free for all paid plans, or gated to Pro+? | Daniel (Finance) | Nov 12 |
> | Design system: extend existing token set or new dashboard primitives? | Priya | Nov 10 |
> | Beta cohort: which 5 customers? | Maya + CS | Nov 8 |
>
> ---
>
> **Devil's Advocate caught**
>
> The Q4 roadmap already has the Looker integration ($4K/mo embed). At first read, this PRD looks like overlap. It is not. Looker serves the analyst persona (5% of users, deep queries). This dashboard serves the everyday persona (95% of users, three specific jobs). The PRD now says this explicitly in the Scope section.
>
> ---
>
> **Timeline**
>
> - Nov 8 to Nov 22: design, beta cohort selection
> - Nov 25 to Jan 17: build (8 weeks, 1.5 eng)
> - Jan 20 to Feb 3: closed beta with 5 customers
> - Feb 4: GA
>
> Buffer for security review and launch comms is built in.

---

## What Changed (and Why)

| Element | Before | After | Why It Matters |
|---------|--------|-------|----------------|
| Problem | "Users have been asking" | 7 named customers, source-cited, renewal risk quantified | "Users want this" is the lowest-quality signal in product. Replace with evidence. |
| Success metrics | "Adoption, satisfaction" | 40% MAU, 50% ticket reduction, 3/3 renewal accounts | Vague metrics make a feature impossible to kill. Numbers create accountability. |
| Scope | Bullet list of features | In, Out (parking lot), Explicitly NOT in scope | "Out of scope" is what protects the team. Three-way scope is the difference between shipping and scope creep. |
| Tradeoffs | None | Build vs. buy table with named alternatives | Engineering reviews any PRD that skips this with "did you consider Metabase?" Answer it before they ask. |
| Tech constraints | Missing | 3 flags pre-vetted with eng lead | PRDs that surprise engineering die in review. |
| Cross-team awareness | Missing | Looker overlap addressed explicitly | The Devil's Advocate pass caught a fatal collision the author missed. |
| Open questions | "What charts?" | Specific questions, owners, decision dates | Questions without owners are wishes. |

---

## How the System Did It

The pipeline:
- Pre-flight: Read all 7 C-core files (about-me, company-context, project-brief, voice-dna, icp-profile, team-roster, company-glossary)
- Specialist: Product Specialist applied Amazon-style PRD structure, pulled the customer interview citations from the CS log, named team members from team-roster
- Devil's Advocate: Reviewer caught the Looker overlap and forced an explicit scope clarification
- Voice: Copywriter matched the company's direct, evidence-first PM voice from voice-dna
- Compliance: SOC 2 reviewer flagged data isolation as a security review checkpoint
- Quality: Gatekeeper approved

The whole thing took 5 minutes instead of 2 hours.

---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
