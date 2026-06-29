# AI Prompts for Product Managers (June 2026)

15 copy-paste prompts for real PM workflows. Each prompt includes the pattern, a filled example, and a note on where it can go wrong.

**Core rule across all prompts:** Include the source data in the prompt. Never ask the model to recall information it wasn't given. This eliminates hallucination on factual claims.

---

## PRD & Spec Writing Prompts

### 1. First-Draft PRD from Feature Brief

**Pattern:**
```
Write a first-draft PRD for [feature name].

User story: [paste user story]
Acceptance criteria hints: [paste your rough notes]
Out of scope: [list what this feature does NOT do]

Format output as:
- Overview (2 sentences)
- User stories (numbered list)
- Acceptance criteria (per story)
- Open questions

Flag any missing information as [MISSING] rather than inventing it.
```

**Why it works:** The `[MISSING]` instruction forces the model to surface gaps instead of filling them with plausible-sounding guesses.

**Watch out for:** The model will sometimes write acceptance criteria that sound complete but skip non-functional requirements (performance, security, accessibility). Always add a section asking explicitly for these.

---

### 2. Convert Engineering Notes into a PRD Section

**Pattern:**
```
Convert these engineering notes into a PM-readable PRD section. 
Audience: non-technical stakeholders.
Engineering notes: [paste verbatim]

Output:
- Plain-language description of what this does
- User impact (what the user can now do that they couldn't before)
- Any constraints or limitations a PM should communicate to stakeholders
```

---

### 3. Acceptance Criteria Expansion

**Pattern:**
```
Given this user story: [paste story]
Generate acceptance criteria using the Given/When/Then format.
Include at least 2 edge cases and 1 error state.
Do not add scenarios that require new engineering scope beyond the story.
```

---

### 4. Release Note Drafting

**Pattern:**
```
Convert these PR titles and descriptions into a customer-facing release note.
Audience: non-technical business users.
Maximum length: 100 words.
Tone: factual, not marketing.

PR descriptions:
[paste list]

Do not use the words "powerful," "seamless," or "exciting."
```

---

## User Feedback & Research Prompts

### 5. Feedback Clustering

**Pattern:**
```
Here are [N] customer support tickets / survey responses:

[paste raw text, one per line or numbered]

Cluster them into 3–5 themes. For each theme:
1. Name the theme (3–5 words)
2. Write one sentence describing the core pain point
3. List which ticket numbers fall into this cluster
4. Suggest one product hypothesis this cluster supports

Do not create a cluster with fewer than 2 tickets.
```

---

### 6. Interview Debrief Summary

**Pattern:**
```
Here are my raw notes from a user interview:

[paste notes]

Summarize:
1. The user's primary job-to-be-done in 1 sentence
2. The 3 most specific pain points mentioned (quote the user's words where possible)
3. Any workarounds the user described
4. One thing that surprised me based on [expected assumption — describe it briefly]

Flag anything that is your interpretation vs. something the user explicitly said.
```

**Why the last instruction matters:** Without it, models blend inference and direct evidence in ways that corrupt research findings.

---

### 7. Competitive Intelligence from Public Page

**Pattern:**
```
Analyze the following competitor's pricing page:

[paste full text from the page]

Extract:
1. The 3 main value propositions they lead with (in their words)
2. What is conspicuously absent compared to [your product — describe it briefly]
3. The customer segment the page appears to target (evidence: what language, company sizes, and use cases appear)
4. Any pricing signals (free tier limits, enterprise tier triggers)

Do not invent features not present in the text I provided.
```

---

### 8. Persona Summary from Research Data

**Pattern:**
```
Based on these research notes across [N] user interviews:

[paste notes or synthesized themes]

Write a PM persona with:
- Name and role (fictional but grounded in the data)
- Primary goal
- Top 3 frustrations (cite which interviews surface each)
- Current workaround for the main problem
- What would make them switch from their current solution

Mark anything inferred (not directly stated) with [INFERRED].
```

---

## Roadmap & Planning Prompts

### 9. OKR-Feature Alignment Check

**Pattern:**
```
Our current OKRs for this quarter are:
[paste OKRs]

Our current feature backlog includes:
[paste backlog items]

For each backlog item, assess:
1. Which OKR it most directly supports
2. Estimated contribution (High / Medium / Low / None) — explain the reasoning in 1 sentence
3. Flag items with no clear OKR link

Do not add or remove backlog items. Only analyze what I've listed.
```

---

### 10. Sprint Goal Draft

**Pattern:**
```
We are planning sprint [number]. 

Selected stories:
[paste story list with rough sizes]

Draft a sprint goal that:
- Is a single sentence
- Focuses on user or business outcome, not output
- A non-engineer could understand in 5 seconds

Then explain: why would a PM reject this sprint goal? What assumption is it making?
```

---

### 11. Prioritization Rationale (RICE-style)

**Pattern:**
```
Score the following features for prioritization using RICE.

My definitions:
- Reach: number of users affected per quarter (use my estimates below)
- Impact: 1 (minimal) to 3 (massive) effect on the primary metric
- Confidence: % I trust my Reach and Impact estimates
- Effort: person-weeks of engineering

Features and my estimates:
[paste feature + your Reach / Impact / Confidence / Effort estimates]

Calculate the RICE score for each.
Then flag any feature where my Confidence is below 50% and suggest what data I'd need to raise it.
```

---

## Stakeholder Communication Prompts

### 12. Roadmap Update Email for Leadership

**Pattern:**
```
Write a 150-word roadmap update email for a leadership audience.

Last quarter commitments: [paste]
Delivered: [paste]
Slipped and why: [paste]
Next quarter priorities: [paste]

Tone: direct, no hedging. Acknowledge slippage clearly. Do not use "learnings," "bandwidth," or "synergy."
```

---

### 13. Engineering Kickoff Brief

**Pattern:**
```
Write a 1-page engineering kickoff brief for [feature].

Context to include:
- User problem being solved: [paste]
- Proposed solution: [paste]
- Out of scope: [paste]
- Success metric: [paste]
- Open technical questions I don't have answers to: [paste]

Format: short prose paragraphs, no bullet points except for the open questions section.
Audience: senior engineers who will push back on anything unclear.
```

---

### 14. Exec Narrative for a Feature Decision

**Pattern:**
```
I need to explain why we deprioritized [feature] this quarter.

Facts:
- The feature has [N] customer requests
- It was originally scoped for [timeline]
- We deprioritized it because: [paste real reason]
- What we prioritized instead: [paste]

Write a 3-sentence exec-facing explanation that:
- Acknowledges the customer request volume
- Explains the tradeoff without blaming engineering
- States when we will revisit it
```

---

### 15. Post-Mortem Summary

**Pattern:**
```
Write a post-mortem summary for this incident or failed launch:

Timeline of events: [paste]
Root cause: [paste your team's assessment]
Customer impact: [paste]
What worked well: [paste]
What didn't: [paste]
Action items already agreed: [paste]

Format:
- Executive summary (3 sentences)
- Timeline (keep as-is)
- Root cause (1 paragraph — do not soften or hedge)
- What we're changing (numbered list, owners in brackets)

Do not write "we will strive to" or "going forward." Write what specifically will change.
```

---

## Prompt Anti-Patterns to Avoid

| Bad Prompt | Why It Fails | Better Pattern |
|---|---|---|
| "Write a PRD for a notifications feature" | No source data — model invents user stories | Include user story + acceptance hints |
| "Summarize our user feedback" | No feedback provided — model hallucinates | Paste the actual feedback text |
| "What does our competitor do?" | Model recalls training data (possibly outdated) | Paste the competitor's actual page text |
| "Prioritize our backlog" | No scoring criteria provided | Include your RICE estimates or weighting rubric |
| "Make this executive-friendly" | No audience context | Specify: exec role, familiarity level, decision they need to make |

---

*Source: [ChatGPT for PMs: Prompts Top Managers Hide](https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/chatgpt-for-product-managers.html) — Updated June 2026*
