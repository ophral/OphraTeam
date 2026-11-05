# Legal Before / After

> What a real person in this department gets BEFORE the system vs. AFTER.

---

## The Situation

Rachel is the General Counsel at a mid-stage company. Procurement sent over a $80K/year vendor SaaS contract for review. It is a standard MSA + Order Form. Standard means nothing. Rachel has 30 minutes before her next call. The COO wants to sign by Friday.

---

## ❌ Before: What They Wrote Without the System

> **Memo: Vendor SaaS Agreement Review (Vendor X)**
>
> I have reviewed the proposed Master Services Agreement and Order Form between the Company and Vendor X dated October 15, 2026. Below is a summary of the principal terms and considerations.
>
> Section 3 (Term and Termination): The agreement provides for an initial term of twelve (12) months with automatic renewal for successive twelve (12) month periods unless terminated by either party. The Company should consider whether the renewal mechanics align with its preferred contracting practices.
>
> Section 7 (Fees and Payment): Fees of $80,000 annually, payable in advance. The agreement permits the Vendor to increase fees upon renewal. The Company should consider negotiating a cap on fee increases.
>
> Section 9 (Limitation of Liability): The agreement caps each party's liability at fees paid in the preceding twelve (12) months. The Company should consider whether this allocation is appropriate.
>
> Section 11 (Intellectual Property): The agreement contains provisions regarding ownership of pre-existing intellectual property and work product. The Company should consider the scope of these provisions.
>
> Section 14 (Indemnification): The Vendor provides certain indemnities to the Company. The Company should consider whether the scope and carve-outs are acceptable.
>
> Section 18 (Governing Law): Delaware. Acceptable.
>
> Overall, the agreement is a market-standard vendor SaaS agreement. The Company should consider the items noted above prior to execution.

The COO reads "consider, consider, consider" and signs. He has no idea that the auto-renewal locks him into a second year if he forgets to send notice 90 days out, or that the IP clause assigns custom configurations to the vendor.

---

## ✅ After: What the System Produced

> **Memo: Vendor X SaaS Agreement (Order Form #VX-2026-1015). Risk Review**
>
> **Recommendation: Do not sign as-is. 3 red flags below. With the fixes, this is a sign.**
>
> ---
>
> **🔴 RED FLAG 1: Auto-renewal trap (Section 3.2)**
>
> Severity: HIGH
>
> The contract auto-renews for 12 months unless we give written notice **90 days before expiry**. Renewal date is October 15, 2027. That means our internal deadline to decide is **July 15, 2027**.
>
> If we miss that window, we are locked in for another 12 months at whatever fee Vendor X sets (see Red Flag 2).
>
> **Fix:** Negotiate to either (a) 30-day notice window, or (b) opt-in renewal instead of opt-out. If Vendor X refuses, accept it but I am putting a calendar reminder on the IT Director and CFO for July 1, 2027.
>
> ---
>
> **🔴 RED FLAG 2: Uncapped fee increase on renewal (Section 7.4)**
>
> Severity: HIGH
>
> The contract allows Vendor X to raise fees "to the then-current list price" on each renewal. No cap. Last year we saw a 22% jump from this same vendor across the industry.
>
> **Fix:** Insert a fee cap of CPI + 3%, or a hard cap of 5% per renewal. Standard ask. They will agree.
>
> ---
>
> **🔴 RED FLAG 3: Asymmetric IP assignment (Section 11.3)**
>
> Severity: MEDIUM-HIGH
>
> The clause assigns to Vendor X any "improvements, configurations, or derivative works" created during the engagement. Translation: the custom dashboards and workflow automations our team builds inside their platform become their IP.
>
> This is unusual for SaaS. Most vendors leave customer configurations with the customer.
>
> **Fix:** Strike Section 11.3, replace with: "Customer retains ownership of all configurations, dashboards, integrations, and customizations created within the Vendor platform." Non-negotiable from our side.
>
> ---
>
> **🟡 Smaller items (worth raising, not deal breakers)**
>
> - Section 9 liability cap is at 12 months of fees. Industry standard is 12 to 24 months. Push for 24, accept 12.
> - Section 14 indemnity carves out "third-party data." Make sure that does not include data we provide to the platform. Clarify with one sentence.
> - Section 6 SLA is 99.5%. We need 99.9% if this becomes business-critical. Today it is not, so 99.5% is fine.
>
> ---
>
> **Action plan**
>
> 1. I send the redline to Vendor X today with Red Flags 1 to 3.
> 2. Expected turnaround: 3 business days.
> 3. If Red Flags 2 and 3 are accepted, we sign. If Red Flag 1 is rejected, I accept it and own the calendar reminder.
> 4. Total estimated turnaround: 5 business days. Friday signing is realistic.
>
> Saved approximately 6 hours of partner counsel time by handling the redline in-house.

---

## What Changed (and Why)

| Element | Before | After | Why It Matters |
|---------|--------|-------|----------------|
| Framing | "Consider" everything | Risk-rated red flags | "Consider" gives no signal. Severity ratings make the call obvious. |
| Specificity | "The Company should consider negotiating a cap" | "CPI + 3% or 5% hard cap" | Recommendations without numbers force a second round of analysis. |
| Auto-renewal | One sentence | Specific dates, calendar action, owner named | This is the single most common contract trap. Has to be loud. |
| IP issue | "Consider the scope" | Quoted clause, plain-English translation, redline text | The COO does not know what "derivative works" means. Translate it. |
| Action plan | None | Step-by-step with owners and timing | Legal memos that end without next steps land back on Legal's desk. |
| Tone | Lawyerly hedging | Direct, prioritized, plain language | Plain language is not unlawyerly. It is the work product clients pay for. |

---

## How the System Did It

The pipeline:
- Pre-flight: Read all 7 C-core files (about-me, company-context, project-brief, voice-dna, icp-profile, team-roster, company-glossary)
- Specialist: Commercial Contracts Specialist applied SaaS contract patterns, flagged the asymmetric IP and auto-renewal trap from a library of 200+ reviewed vendor agreements
- Voice: Copywriter rewrote the memo in plain English without losing legal precision
- Compliance: Risk Reviewer cross-checked liability cap against company policy, confirmed redline language was clean
- Quality: Gatekeeper approved

The whole thing took 5 minutes instead of 2 hours.

---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
