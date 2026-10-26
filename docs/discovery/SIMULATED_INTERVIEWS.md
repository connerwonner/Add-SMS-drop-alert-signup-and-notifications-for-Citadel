# Simulated Interviews: SMS Drop Alerts for Citadel

> **ALL CONTENT BELOW IS SIMULATED.** Interviewees are fictional instructor-style personas. No real person was contacted. No real names, phone numbers, or client data appear here. Replace with real notes only if your instructor approves live outreach.

**Purpose:** Replaces Section 4 of DISCOVERY_PACKAGE.md. Note IDs match the package (N-P1-#, N-S1-#).
**Method:** Same eight neutral questions, with sponsor wording for the second interview. Minimal notes only (not verbatim transcripts).
**Consent script (read aloud at start, simulated):** "This is a voluntary student project interview, about 20 minutes. You can skip any question or stop anytime. I'll take brief notes without your name. Please don't share private client information. Is it okay to continue?" → *Simulated participant agreed.*

---

## Interview 1: Property Professional (P1, simulated)

**Persona basis:** Independent listing agent at a small local brokerage (fictional).


| Q | Question (short) | Simulated notes |
|---|------------------|-----------------|
| 1 | Publishing workflow | **N-P1-1:** Writes the listing in the platform dashboard, adds photos, then also posts separately to social media. Does the same info twice. |
| 2 | Audience / how they find out | **N-P1-2:** Interested buyers mostly check the site or get an email. Some ask her to "let me know" by text, but she does that by hand from her own phone. |
| 3 | Time-sensitive updates | **N-P1-3:** Price drops and open-house changes often reach people a day or more late. Email gets buried. |
| 4 | Review / approval | **N-P1-4:** Her broker reads listing text before it goes live, usually same day or next day. Corrections are sent back by email. |
| 5 | Success after 30 days | **N-P1-5:** Would look at how many people signed up and whether they clicked through to the listing. Not interested in tracking individuals. |
| 6 | Concerns about phones | **N-P1-6:** Worried about texting people who did not agree to it, and about being unable to stop messages quickly if there's a mistake. |
| 7 | Accessibility | **N-P1-7:** Some clients are older and prefer larger text and plain language. A few ask for phone calls instead of online forms. |
| 8 | One thing to change | **N-P1-8:** Wants one place to publish instead of posting the same thing in several places. |

**Interviewer observations (not stakeholder claims):** Participant hesitated on Q6 and spoke longest on Q3. Did not mention cost.

---

## Interview 2: Local Sponsor (S1, simulated)

**Persona basis:** Owner of a small neighborhood business (fictional café) that wants to reach newcomers.
*

| Q | Question (short) | Simulated notes |
|---|------------------|-----------------|
| 1 | Current promotion | **N-S1-1:** Uses printed flyers, a window sign, and a couple of online neighborhood listings. |
| 2 | Audience | **N-S1-2:** Wants to reach people who just moved to the area. Doesn't know how to find them. |
| 3 | Time-sensitive promos | **N-S1-3a:** Seasonal offers are time-limited, so timing matters more than volume. |
| 4 | Review / approval | **N-S1-3:** Needs to approve the exact wording of anything with the business name on it. Currently approves by email or text. |
| 4 (follow-up) | Claims | **N-S1-4:** Doesn't want words like "best" or "cheapest" unless they can be backed up. Had a past complaint about an ad claim. |
| 5 | Success measures | **N-S1-5:** Would count offer redemptions (e.g., a code mentioned at the counter). |
| 6 | Concerns about phones | **N-S1-6:** Unsure whether sponsor messages belong in text alerts at all. Worried customers would find it intrusive. |
| 7 | Accessibility | **N-S1-7:** Hasn't thought about it much. Guesses short, clear messages are better for everyone. *(Participant guess, low confidence.)* |
| 8 | One thing to change | **N-S1-8:** Would like a simple way to be seen by new residents without paying for large ads. |

**Interviewer observations (not stakeholder claims):** Participant was enthusiastic about reach, cautious about intrusiveness. Did not state a budget.

---

## De-identified Notes → Themes (AI step: simulated and labeled)

> **Honesty note:** This transformation was produced by Claude during preparation, not by ChatGPT, Gemini, or AI Studio. If your assignment requires those tools, run the prompt in Section 5 of the package with the notes above and record the real output in the AI log. Do not claim these outputs came from those tools.

**Prompt pattern:** "Convert these de-identified interview notes into themes, uncertainties, and candidate requirements. Quote no more than necessary. Mark every inference as an inference and list questions that require stakeholder confirmation."

| # | Theme | Evidence | Inference (marked) | Candidate requirement |
|---|-------|----------|--------------------|-----------------------|
| T1 | Time-sensitive updates arrive late | N-P1-2, N-P1-3, N-S1-3a | *Inference:* a faster channel like SMS could help | Alert sent when an approved drop is published |
| T2 | Consent and ability to stop | N-P1-6, N-S1-6 | *Inference:* explicit opt-in and STOP are essential for trust | Opt-in with terms; STOP honored immediately |
| T3 | Review before publishing | N-P1-4, N-S1-3, N-S1-4 | *Inference:* review must happen before any send, not after | Approval workflow for listings and sponsor text |
| T4 | Sponsor wording control and claim accuracy | N-S1-3, N-S1-4 | *Inference:* approval should reset on edits | Sponsor approval; unsupported claims removed |
| T5 | Uncertain sponsor role in SMS | N-S1-6 | *Inference:* sponsor line may need to be optional | Sponsor content off by default pending decision |
| T6 | Aggregate success measures | N-P1-5, N-S1-5 | *Inference:* counts, not individual tracking, fit stated needs | Signup and click counts; sponsor redemption count |
| T7 | Plain-language, accessible access | N-P1-7, N-S1-7 | *Inference:* short alerts and an accessible signup form; phone-call alternative is unconfirmed | Plain-language alerts; accessible form |
| T8 | Duplicate publishing effort | N-P1-1, N-P1-8 | *Inference:* one-step publish would save time | Publish and alert from one action (post-MVP) |

**Uncertainties requiring stakeholder confirmation**
- U-1: What exactly counts as a "drop"?
- U-2: Should sponsor content appear in SMS at all? (N-S1-6 is unsure)
- U-3: Who is the final approver: the broker or the professional?
- U-4: Alert frequency limits per subscriber?
- U-5: Which SMS provider and cost are acceptable?
- U-6: Legal or carrier consent requirements the team must follow? (Ask instructor; not legal advice.)
- U-7: Is a non-online signup option (e.g., phone) needed? (N-P1-7 hint only)

**Things the notes do NOT support (do not add to requirements):** subscriber demographics, budgets, pricing, conversion rates, any claim that SMS "increases sales."

---

## Line-by-Line Verification (summary vs. source notes)

| Summary claim | Source note | Verified? | Action |
|---------------|-------------|-----------|--------|
| Updates reach people late | N-P1-3 | ✅ Supported | Keep |
| Email gets buried | N-P1-3 | ✅ Supported | Keep |
| Broker reviews before live | N-P1-4 | ✅ Supported | Keep |
| Sponsor must approve wording | N-S1-3 | ✅ Supported | Keep |
| Sponsor avoids unsupported superlatives | N-S1-4 | ✅ Supported | Keep |
| Sponsor unsure about SMS | N-S1-6 | ✅ Supported | Keep as U-2 |
| Success = signups/clicks (pro), redemptions (sponsor) | N-P1-5, N-S1-5 | ✅ Supported | Keep |
| Older clients prefer large text | N-P1-7 | ✅ Supported (one participant, limited evidence) | Keep, flag low confidence |
| Phone-call alternative needed | N-P1-7 ("a few ask for calls") | ⚠️ Partly supported | Moved to U-7 |
| SMS will increase leads | none | ❌ Not in notes | Removed |
| Sponsors want paid placement | none | ❌ Not in notes | Removed |
| Broker is final approver | N-P1-4 says broker reads text; not "final" | ⚠️ Overstated | Kept as U-3 |

---

## Updated Personas (simulated evidence)

**Dana, Property Professional (working hypothesis)**
Evidence: N-P1-1 to N-P1-8. Wants fast, accurate delivery of time-sensitive updates; frustrated by duplicate publishing and late reach; wary of texting people without consent. Open: U-1, U-3, U-4, U-7.

**Sam, Local Sponsor (working hypothesis)**
Evidence: N-S1-1 to N-S1-8. Wants to reach newcomers with time-limited offers; needs wording approval; cautious about claims and intrusiveness. Open: U-2.

*Both personas rest on one simulated interview each. Treat as hypotheses to test, not facts about all professionals or sponsors.*

---

## AI Collaboration Log (this simulated run)

| Field | Entry |
|-------|-------|
| Prompt | Pattern prompt above, applied to the de-identified notes |
| Tool | Claude (preparation). **ChatGPT / Gemini / AI Studio: not run; fill in if your course requires them.** |
| Useful output | Theme table, uncertainty list, verification table |
| Rejected output | Claims about increased leads and paid sponsor placement (not in notes) |
| Verification | Each summary claim checked against note IDs above |
| Commit | _(add hash after committing)_ |
| Privacy | No names, phone numbers, keys, or client data used |
