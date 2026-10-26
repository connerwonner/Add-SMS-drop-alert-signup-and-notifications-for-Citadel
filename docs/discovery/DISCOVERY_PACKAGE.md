# Discovery Package: SMS Drop Alerts for Citadel

**Status:** DRAFT. Interview results below are **SIMULATED** until real, instructor-approved interviews replace them.
**Team / author:** _(your names)_  **Date:** _(date)_

---

## 1. Stakeholders: Facts vs. Assumptions

**Known facts** (from the repo name and issues; verify against your issue list)
- The project is a student project to add SMS drop-alert signup and notifications to the Citadel platform.
- The platform serves property professionals and local sponsors (per the lab brief).

**Assumptions** (A-#; none are confirmed with a stakeholder)

| ID | Assumption | Stakeholder | How to confirm |
|----|-----------|-------------|----------------|
| A-1 | A "drop" is a new listing or listing update that interested people want to hear about quickly. | Both | Ask in interview Q3 |
| A-2 | Property professionals publish listings and want faster reach to interested people. | Property pro | Interview Q1-Q3 |
| A-3 | Local sponsors want visibility next to listings or neighborhood content, but only if their claims are reviewed. | Sponsor | Sponsor Q1, Q4 |
| A-4 | Alert recipients (end users) are a third group whose consent matters most. | End user | Instructor / later research |
| A-5 | Someone must approve listing and sponsor text before it is sent to phones. | Both | Interview Q4 |

| Group | Role | Primary goal (assumed) |
|-------|------|------------------------|
| Property professional | Publishes listings, drops, price changes | Reach interested people quickly with accurate info |
| Local sponsor | Pays for or supplies local promotion | Visible, accurate, approved sponsor messaging |

---

## 2. Discovery Questions

### AI step (you run this, then record results in Section 12)
**ChatGPT prompt:** "I'm a student building an SMS drop-alert feature for a property platform with two stakeholders: property professionals and local sponsors. Suggest 12 neutral, open-ended discovery interview questions about workflow, audience, content approval, success measures, and accessibility."

**Gemini prompt:** "Review these interview questions. Flag any that are leading, assume an answer, are double-barreled, or ask for private or sensitive information. Suggest neutral rewrites."

### Final eight neutral questions
Property professional version (sponsor wording in brackets):

1. Walk me through how you currently publish a new listing from start to finish. [How do you currently promote offers or messages alongside local property content?]
2. Who are you most trying to reach with new listings, and how do they usually find out today? [Who are you most trying to reach with your promotion?]
3. When something is time-sensitive, such as a new listing or price change, how do you share it, and what works or doesn't about that?
4. Who reviews or approves listing content before it goes live, and how long does that usually take? [Who reviews your claims or wording before they are published?]
5. If a new alert feature were working well after 30 days, what would you see or measure?
6. What concerns, if any, would you have about messages reaching people's phones?
7. What accessibility needs have you seen among the people you serve, such as readability, assistive tech, or language?
8. If you could change one thing about how updates reach people, what would it be?

### Questions to avoid (examples of what Gemini should flag)
- "Wouldn't text alerts help you sell faster?" (leading)
- "Can you share your clients' phone numbers?" (privacy-invasive)
- "How much do you earn per deal?" (sensitive, off-topic)
- "Do you want alerts to be fast and easy?" (leading, double-barreled)

---

## 3. Interview Invitation (draft; send ONLY after instructor approval)

> **Subject: 20-minute student project interview (voluntary)**
>
> Hello _(name)_,
>
> I'm _(your name)_, a student in _(course, school)_. For a class project, our team is designing a feature that would let people opt in to text alerts about new property listings. The project is for coursework only. It is not a commercial product.
>
> **What I'm asking:** a 20-minute conversation (phone or video) about how you currently share listings or promotions.
> **Your participation is completely voluntary.** You can skip any question, stop at any time, or decline with no consequence.
> **Data use:** I will take brief notes without your name or contact details. I won't record unless you agree. Notes are shared only with my team and instructor, and de-identified summaries may appear in class materials. Please don't share private client or personal information.
> **AI use:** My team may use AI tools to help organize de-identified notes. We will not enter your name or contact details into them.
>
> If you're willing, reply with a time that works. If not, no reply is needed.
>
> Thank you,
> _(name, school email, instructor name and contact)_

**Outreach rules:** no automated calling, no bulk email, no scraped contacts, no AI impersonation. Contact only people you know or who your instructor approves. Instructor approval: ☐ received on _(date)_

---

## 4. Interview Notes (**SIMULATED**)

> Use these only if no live client is available. They are invented to practice the method. Replace with real notes after an approved interview.

**P1: Simulated property professional (instructor persona)**
- N-P1-1: Publishes listings through the platform dashboard; also posts to social media separately.
- N-P1-2: Interested buyers currently find out by checking the site or by email.
- N-P1-3: Time-sensitive changes (price drops) often reach people late.
- N-P1-4: Broker reviews listing text before publishing; takes about a day.
- N-P1-5: Would judge success by how many people sign up and whether they click through.
- N-P1-6: Worried about texting people who did not agree to it.
- N-P1-7: Some of their audience prefers large text and plain language.

**S1: Simulated local sponsor (instructor persona)**
- N-S1-1: Currently promotes through flyers and a few online listings.
- N-S1-2: Wants to reach people moving into the neighborhood.
- N-S1-3: Needs to approve exact wording of any message that carries their name.
- N-S1-4: Does not want claims like "best" or "cheapest" unless they can back them up.
- N-S1-5: Would measure success by offer redemptions.
- N-S1-6: Unsure whether sponsors should appear in text alerts at all.

---

## 5. Themes, Inferences, and Uncertainties

(AI prompt to run: "Convert these de-identified interview notes into themes, uncertainties, and candidate requirements. Quote no more than necessary. Mark every inference as an inference and list questions that require stakeholder confirmation.")

| Theme | Evidence | Inference (marked) | Candidate requirement |
|-------|----------|--------------------|-----------------------|
| Late delivery of time-sensitive updates | N-P1-2, N-P1-3 | *Inference:* SMS may close the gap | Send alert when a drop is published |
| Consent and trust | N-P1-6 | *Inference:* explicit opt-in and easy opt-out are required | Opt-in with clear terms, STOP support |
| Content must be reviewed | N-P1-4, N-S1-3, N-S1-4 | *Inference:* review step belongs before any alert is sent | Approval workflow for listing and sponsor text |
| Sponsor control of wording | N-S1-3, N-S1-6 | *Inference:* sponsor text may be optional or limited | Sponsor approval; sponsor line off by default |
| Success measured by engagement | N-P1-5, N-S1-5 | *Inference:* need basic counts, not individual tracking | Signup and click counts |
| Accessibility | N-P1-7 | *Inference:* short, plain messages and accessible signup | Plain-language alerts; accessible form |

**Uncertainty list** (needs stakeholder confirmation)
- U-1: What exactly counts as a "drop"?
- U-2: Should sponsor content appear in SMS at all?
- U-3: Who is the final approver, broker or the professional?
- U-4: Alert frequency limits per subscriber?
- U-5: Which SMS provider and cost are acceptable? (instructor / team decision)
- U-6: Are there legal or carrier consent requirements the team must follow? (Check with instructor; this is not legal advice.)

---

## 6. Personas (evidence-based working hypotheses)

### Persona A: "Dana," Property Professional *(hypothesis)*
- **Basis:** N-P1-1 to N-P1-7; assumptions A-1, A-2, A-5.
- **Goals:** Get time-sensitive listing news to interested people quickly; keep content accurate.
- **Frustrations:** Updates reach people late (N-P1-3); review takes about a day (N-P1-4).
- **Needs:** Simple way to publish a drop and trigger an alert; confidence that only consenting people are texted.
- **Open questions:** U-1, U-3, U-4.
- **Not claimed:** age, income, tech skill, or personal traits. Not supported by notes.

### Persona B: "Sam," Local Sponsor *(hypothesis)*
- **Basis:** N-S1-1 to N-S1-6; assumption A-3.
- **Goals:** Reach people new to the neighborhood; protect brand wording.
- **Frustrations:** Unsure about sponsor role in alerts (N-S1-6); needs claim accuracy (N-S1-4).
- **Needs:** Approve wording before it is sent; see simple results.
- **Open questions:** U-2.
- **Not claimed:** business size, budget, or marketing sophistication.

---

## 7. User Stories

| ID | Story | Priority | Size | Owner | Source |
|----|-------|----------|------|-------|--------|
| US-1 | As a **subscriber**, I want to sign up for SMS drop alerts with clear terms, so that I only get texts I agreed to. | High | M | _(name)_ | N-P1-6, A-4 |
| US-2 | As a **subscriber**, I want to reply STOP to opt out, so that I can end alerts at any time. | High | S | _(name)_ | N-P1-6 |
| US-3 | As a **property professional**, I want to publish a drop and trigger an SMS alert, so that interested people hear about it quickly. | High | L | _(name)_ | N-P1-3 |
| US-4 | As a **property professional**, I want my listing text approved before an alert is sent, so that inaccurate info never reaches phones. | High | M | _(name)_ | N-P1-4 |
| US-5 | As a **local sponsor**, I want to approve any message that carries my name, so that my brand wording stays accurate. | High | M | _(name)_ | N-S1-3 |
| US-6 | As a **reviewer**, I want to reject sponsor claims I can't verify, so that we avoid unsupported statements. | Medium | S | _(name)_ | N-S1-4 |
| US-7 | As a **property professional**, I want to see how many people signed up and clicked, so that I can judge whether alerts help. | Medium | M | _(name)_ | N-P1-5 |
| US-8 | As a **subscriber who prefers plain language**, I want short alerts and an accessible signup form, so that I can read and use them easily. | Medium | S | _(name)_ | N-P1-7 |
| US-9 | As a **local sponsor**, I want to see how many people viewed or redeemed my offer, so that I can judge value. | Low | M | _(name)_ | N-S1-5 |
| US-10 | As a **property professional**, I want a limit on alerts per subscriber per week, so that people don't feel spammed. | Low | S | _(name)_ | U-4 (assumption) |

---

## 8. Acceptance Criteria (high-priority stories)

**US-1 Signup with consent**
- *Given* a visitor on the signup page, *when* they enter a phone number and tick an unchecked consent box, *then* the system sends a confirmation text and records consent with a timestamp.
- *Given* the consent box is unchecked, *when* they submit, *then* no signup is created and an error explains why.
- *Given* an invalid phone number, *when* they submit, *then* they see a clear message and nothing is stored.

**US-2 Opt-out**
- *Given* an active subscriber, *when* they reply STOP, *then* they get one confirmation text and receive no further alerts.
- *Given* an opted-out number, *when* a drop is published, *then* no message is sent to it.

**US-3 Drop alert**
- *Given* an approved drop, *when* the professional clicks "Send alert", *then* all active subscribers receive the message and the send is logged.
- *Given* a drop not yet approved, *when* the professional clicks "Send alert", *then* the system blocks the send and shows the reason.

**US-4 Listing approval**
- *Given* a drafted listing, *when* the reviewer approves it, *then* its status becomes "Approved" and the approver and time are recorded.
- *Given* a rejected listing, *when* the professional edits it, *then* it returns to "Pending review".

**US-5 Sponsor approval**
- *Given* a message containing a sponsor name, *when* the sponsor has not approved it, *then* it cannot be included in any alert.
- *Given* the sponsor approves exact wording, *when* that wording is later edited, *then* approval is reset.

---

## 9. Work Estimates and Week 8 MVP

**Sizes:** S = under 1 day, M = 1-3 days, L = 3-5 days (adjust to your team).

**Week 8 MVP (proposed):** US-1, US-2, US-3, US-4, with US-5 as a manual (non-automated) check if time is short.
- Subscribers can opt in and out.
- A professional can send one approved alert.
- Nothing is sent without approval.

**Post-MVP:** US-6 to US-10.

**Out of scope for MVP:** sponsor content in SMS (pending U-2), analytics dashboards, per-subscriber frequency limits.

---

## 10. Content Approval Workflow (listings and sponsor claims)

```
Draft → Pending Review → (Approved | Changes Requested)
                              ↓
        If sponsor named → Sponsor Review → (Approved | Changes Requested)
                              ↓
                       Ready to Send → Sent (logged)
```

| Step | Who | Check | Record |
|------|-----|-------|--------|
| 1. Draft | Property professional | Facts match the listing source | Draft saved |
| 2. Review | Designated reviewer (U-3) | Accuracy, tone, length, no unsupported claims | Reviewer + timestamp |
| 3. Sponsor review (if applicable) | Sponsor | Exact wording approved | Approval + wording version |
| 4. Send | Property professional | Only approved text; only opted-in numbers | Send log |

**Rules**
- Any edit after approval resets approval.
- Superlatives ("best," "cheapest," "guaranteed") need a stated source or are removed.
- Every alert includes the sender name and opt-out instructions.
- Any sponsor claim an AI tool suggests that no stakeholder stated is removed and added to the uncertainty list.

---

## 11. Requirements Traceability Matrix (extension)

| Requirement | Story | Source | Type | Acceptance test | Status |
|-------------|-------|--------|------|-----------------|--------|
| Explicit opt-in with terms | US-1 | N-P1-6 | Evidence | US-1 AC1-3 | Planned |
| STOP opt-out honored | US-2 | N-P1-6 | Evidence | US-2 AC1-2 | Planned |
| Alert on drop publish | US-3 | N-P1-3 | Evidence | US-3 AC1-2 | Planned |
| Review before send | US-4 | N-P1-4 | Evidence | US-4 AC1-2 | Planned |
| Sponsor wording approval | US-5 | N-S1-3 | Evidence | US-5 AC1-2 | Planned |
| Claim verification | US-6 | N-S1-4 | Evidence | TBD | Backlog |
| Engagement counts | US-7 | N-P1-5 | Evidence | TBD | Backlog |
| Plain, accessible alerts | US-8 | N-P1-7 | Evidence | TBD | Backlog |
| Sponsor results | US-9 | N-S1-5 | Evidence | TBD | Backlog |
| Weekly alert cap | US-10 | U-4 | **Assumption** | TBD | Backlog |

---

## 12. AI Collaboration Log (fill in as you go)

| Field | ChatGPT | Gemini | AI Studio |
|-------|---------|--------|-----------|
| Prompt used | _(paste)_ | _(paste)_ | _(paste)_ |
| Useful output | | | |
| Rejected output and why | | | |
| How I verified it | | | Compared summary to notes line by line |
| Commit hash | | | |

**Rules:** no names, phone numbers, API keys, or private data in prompts. Mark inferences. Remove any invented stakeholder claim and add it to the uncertainty list.

---

## 13. Verification Checklist

- [ ] Invitation and consent language are transparent
- [ ] Instructor approval for outreach recorded
- [ ] Every requirement traces to a note ID or is labeled an assumption
- [ ] Backlog items have acceptance criteria and owners
- [ ] No unapproved outreach; no sensitive data stored
- [ ] Simulated results are labeled SIMULATED
