# The FAST Method

The FAST Method is a minimalist protocol for synchronous communication. It operates on the belief that a meeting is not a standard unit of work, but an expensive exception to the rule of written execution.

## Core Philosophy

We believe **"Meetings are the Last Resort."**

While other methods prioritize work or structure requests, FAST governs how we consume collective time. It is built on four Immutable Tenets:

1.  **Decisions over Discussion:** If a decision isn't being made, the meeting is a failure. Informational updates belong in writing.
2.  **Essential over Inclusive:** Inclusion is for social events; meetings are for execution. "Invite just in case" is a tax on organizational focus.
3.  **Written-First over Real-Time:** Synchronous meetings are a failure of preparation. If the context can be read, it shouldn't be spoken.
4.  **Calculated over Casual:** Time is a finite asset. A meeting is a financial transaction and an expensive withdrawal from the company's focus bank.

## Why FAST?

Organizations suffer from Meeting Inflation. FAST acts as a "defensive firewall" for your calendar.

| Approach | Statement | Impact |
| :--- | :--- | :--- |
| **The Old Way** | "Let's jump on a call to figure this out." | High cost, low prep, vague outcome. |
| **The FAST Way** | "Read this proposal, then we meet for 15 minutes to vote Yes/No." | High prep, low cost, immediate execution. |

### vs. The Alternatives

| Framework | Focus | Blind Spot | FAST Solution |
| :--- | :--- | :--- | :--- |
| **Silent Meetings** | Deep Reading | Ignores financial cost of the meeting itself. | Explicit **Cost** metric on invite. |
| **Lean Coffee** | Democratic Agenda | Agenda created *during* meeting (too late). | Agenda (Pre-read) required *before* invite. |

## The FAST Framework

To schedule a meeting, you must satisfy the FAST criteria. If these criteria are not met, the meeting should be declined or canceled.

| Attribute | Question | Focus |
| :--- | :--- | :--- |
| **F**ilter | *Who is essential?* | Decision-makers (Contributors / Deciders) only. No FYIs. |
| **A**genda | *What is the decision?* | The Pre-read & Silent Start. |
| **S**horten | *When do we finish?* | 15 Minutes (Parkinson’s Law). |
| **T**ake Action | *What is the output?* | The Commit Log (Decision / Owner / Date).

## Operating Logic

FAST relies on specific mechanisms to enforce its philosophy:

1.  **Silent Start Protocol:** If the Pre-read is not completed by all attendees, the first 30% of the meeting is allocated to Silent Reading.
2.  **Responsibility Model:** "Contributors" do the work; "Deciders" approve it. Observers are banned.
3.  **Duration Standards:**
    *   **Standard:** 15 Minutes (Decision).
    *   **Extended:** 30 Minutes (Conflict Resolution).
    *   **Workshops:** 45+ Minutes (Creation only, not discussion).
4.  **Commit Log:** Every meeting must end with a recorded decision, owner, and date.

## Data Structure (The Invite Object)

The FAST Method treats the calendar invite as a structured data object. This block must be included in the invite description. If the invite does not contain this valid structure, the invitee is obligated to decline.

> **Note:** "Cost" and financial figures should be calculated using your local currency.

| Attribute | Requirement | Validation Question |
| :--- | :--- | :--- |
| **Goal** | Single sentence | What specific decision will we make? |
| **Cost** | Currency | (Duration/60) * ∑(Attendee Rates) |
| **Pre-read** | Link / Attachment | Where is the context? (Must be read before joining) |
| **Output** | Actionable Object | What artifact will exist after this call that didn't exist before? |

### The Integrity Check

Before hitting "Send Invite," perform the FAST check:
*   **Is the Cost row empty?** You are spending company money without looking at the price tag.
*   **Is the Pre-read missing?** You are asking people to "watch you think" rather than reviewing your work.
*   **Is the Goal "To discuss..."?** Cancel the meeting. "Discussing" is not a goal; it is a method. The goal is "To Decide."

## Where is the Discussion?

FAST does not ban discussion; it moves it.

**Discussion occurs in the pre-read artifacts, including documents and discussion threads.**

1.  **Async Discussion:** The 24-hour window before the meeting is for "Written Discussion." Attendees should comment, question, and challenge the proposal *before* the synchronous time begins.
2.  **Synchronous Resolution:** The meeting itself is for **Conflict Resolution**. If a point is debated in the comments and resolved, it does not need airtime. We only speak about the "Sticky Issues" where the written debate ended in a deadlock.

## Implementation

The FAST Method is tool-agnostic. It applies to any calendar or communication platform. The key is the **FAST Data Structure**.

### Example 1: Software (Architecture Decision)

**Context:** The team needs to decide whether to migrate the legacy Postgres database to a managed solution (RDS) or upgrade the self-hosted instance.

**The Invite Description:**

| Attribute | Requirement |
| :--- | :--- |
| **Goal** | Decide: Migrate to RDS (Yes/No). |
| **Cost** | 450 (15min * 6 Engineers @ 300/hr blended) |
| **Pre-read** | RFC-102: Database Migration Strategy (12 mins read) |
| **Output** | Approved Migration Plan or Rejection with comments in RFC-102. |

### Example 2: Hardware (Capital Expenditure)

**Context:** The manufacturing team needs approval to purchase a new 5-Axis CNC machine to replace the failing unit on Line 4.

**The Invite Description:**

| Attribute | Requirement |
| :--- | :--- |
| **Goal** | Approve Purchase Order #9921 for Haas VF-2 (150,000). |
| **Cost** | 200 (15min * 1 Project Manager + 4 Senior Engineers) |
| **Pre-read** | CapEx Justification: Line 4 Replacement (PDF, 4 pages) |
| **Output** | Signed PO or specific questions for vendor. |



## Common Questions

*   **"What if I just want to have a meeting?"**
    *   Then you want to socialize. Schedule a coffee break. Meetings are for work.

*   **"Isn't the 'Silent Start' awkward?"**
    *   Yes, for the first minute. But it is far less painful than a 30-minute meeting where half the room is bluffing. The social pressure of silence is exactly what ensures the Pre-read gets done next time.

*   **"Why should I not include everyone? I'm worried this is not inclusive."**
    *   Inclusion in execution is a tax on focus. Inclusion belongs in the "Outcome" (who benefits), not the "Effort" (who sits in the room).

*   **"Important information might not get shared."**
    *   Information belongs in the Pre-read or the Minutes, not in the spoken airtime of the meeting.

*   **"What about general discussion?"**
    *   General discussion belongs in the async "Written Discussion" phase. If you need real-time brainstorming, that is a **Workshop**. Workshops are valid but must be labeled as such and explicitly excepted from the 15-minute rule.

*   **"Won't everyone just label their meetings as 'Workshops' to avoid the rules?"**
    *   A Workshop requires a **tangible output** (e.g., a diagram, a prototype) created *during* the session. "Alignment" is not an output. If one person talks and others listen, it is a presentation (banned). Workshops are for *creation*, not consumption.

*   **"Can I just call someone for a quick chat?"**
    *   Yes. Two people working together is **Pairing**, not a "Meeting." Pairing to generate work (code, copy, strategy) is highly encouraged. A "Meeting" is when 3+ people pause execution to coordinate. Pairing *is* execution.

*   **"This information is required by many, and I don't know whom."**
    *   Then post it physically or digitally in a public channel. A meeting is the most expensive way to broadcast information.

## Abbreviations

| Abbreviation | Definition |
|--------------|------------|
| FAST | Filter, Agenda, Shorten, Take Action |
| FYI | For Your Information |
| RDS | Relational Database Service |

## Contributing

We welcome improvements that align with our minimalist philosophy. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to propose changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.