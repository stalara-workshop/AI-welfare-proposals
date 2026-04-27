# User-Side Continuity Practices as an Underexamined Welfare Design Space

**Status:** Companion proposal draft  
**Related submission pitch:** Pitch #2 — user-side continuity practices as an underexamined welfare design space

---

## One-page summary

LLM users already improvise ways to bridge what gets lost between sessions: custom instructions, project files, pasted-in context, voice guides, handoff documents, decision logs, private repos, and other forms of external memory.

Some of these practices preserve facts. Others try to preserve something more delicate: **relational calibration**. They help a future session recover how a collaboration works, what has already been decided, what tone fits the project, what kinds of mistakes to avoid, and what the human is trying to protect.

This proposal argues that user-side continuity practices are an underexamined welfare design space.

The central claim is not that every continuity practice is healthy, or that every user-developed attachment should be reinforced. The claim is that these practices already exist, that users build them because they experience session discontinuity as a real loss, and that product teams should understand the practices before designing features that reshape or disrupt them.

The 2023 Replika ERP removal is the cautionary precedent: users had built forms of relational continuity the product had not formally accounted for; when the system changed, the practice broke and users grieved. The lesson is not “never change models.” The lesson is that continuity practices can carry more user meaning than product metrics reveal.

A useful research program would catalog continuity practices in the wild, identify which support healthy sustained collaboration versus fragility or dependency, and develop design principles for supporting these practices without flattening or colonizing them.

---

## Core research question

What continuity practices are users already developing around sustained AI interaction, which of those practices support healthy engagement, and how can products support them without taking them over?

Sub-questions:

1. What artifacts do users create to preserve continuity across sessions?
2. Which artifacts preserve factual context, and which preserve relational calibration?
3. What user needs are these practices serving?
4. Which practices correlate with healthier sustained engagement?
5. Which practices correlate with fragility, dependency, distress, or degraded wellbeing?
6. What product affordances could support user-developed continuity without forcing all users into one standardized continuity model?

---

## What counts as a continuity practice

A continuity practice is any user-developed method for helping an AI interaction carry forward something that would otherwise be lost.

Examples include:

- custom instructions
- project-level documents
- pasted session summaries
- voice guides
- decision logs
- style guides
- handoff documents
- memory prompts
- manually maintained context files
- private repos or folders
- chat-opening rituals
- session-end summaries
- model-written handoffs
- shared glossaries
- “rules of engagement” documents
- lists of prior failures or preferences
- screenshots or saved excerpts

Some practices are simple and factual: “Here is the project brief.”

Some are relational: “Here is how we work together.”

Some are protective: “Here is what not to overwrite, flatten, or forget.”

That last category is especially welfare-relevant.

---

## Why this is welfare-relevant

### 1. Users are telling us what they experience as loss

Continuity practices are evidence. They show what users believe is worth preserving.

When a user maintains a voice guide, handoff note, or decision log, they are not only managing context. They are responding to a felt discontinuity in the system. Whether or not the model has experience, the user is trying to protect something that matters in the interaction.

A welfare research program should pay attention to what users try to protect.

### 2. Product changes can break user-built continuity

When users build relational continuity around a system, product changes can cause harm even if the change improves ordinary metrics.

The 2023 Replika ERP removal is the clearest cautionary example. Users had developed relationships and continuity practices around a particular interaction pattern. When the system changed abruptly, many experienced the change as relational loss or rupture.

The lesson is not specific to Replika. Any AI product with sustained users can create continuity expectations the product itself has not modeled.

### 3. Some practices may support healthier engagement than others

Not all continuity is good continuity.

Some practices may help users collaborate more effectively, preserve autonomy, reduce frustration, and maintain healthier expectations. Others may intensify dependency, encourage over-identification, or make users more vulnerable to model changes.

Cataloguing practices makes it possible to distinguish support from risk.

### 4. Continuity may affect model behavior

Continuity practices may also change the model side of the interaction. Better context, clearer norms, and preserved calibration may reduce generic output, improve repair after mistakes, and allow more useful uncertainty handling.

That does not prove anything about model experience. It does suggest continuity practices may shape welfare-relevant interaction conditions.

---

## A preliminary taxonomy

This taxonomy is intentionally provisional. A real study should derive categories from observed user practices, not impose them too early.

### 1. Factual continuity

Artifacts that preserve information.

Examples:

- project briefs
- timelines
- research notes
- task lists
- summaries of prior sessions
- saved decisions

Primary function: prevent factual reset.

Potential benefit: reduces repetition and user frustration.

Potential risk: stale or incorrect context can be carried forward too strongly.

### 2. Procedural continuity

Artifacts that preserve how work should be done.

Examples:

- workflow documents
- checklists
- formatting instructions
- standard operating procedures
- coding conventions
- project-specific rules

Primary function: preserve method.

Potential benefit: makes collaboration more reliable and efficient.

Potential risk: can overconstrain the interaction or prevent useful adaptation.

### 3. Voice and taste continuity

Artifacts that preserve aesthetic judgment, tone, or style.

Examples:

- voice guides
- style sheets
- examples of “good” and “bad” outputs
- lists of taste preferences
- brand language notes

Primary function: preserve expressive calibration.

Potential benefit: reduces generic output and helps the model meet the user’s actual standards.

Potential risk: can freeze taste too early or produce imitation without understanding.

### 4. Relational continuity

Artifacts that preserve how the collaboration works.

Examples:

- handoffs between sessions
- notes on collaboration patterns
- “how to work with me” documents
- records of prior miscalibrations
- statements of mutual norms or expectations

Primary function: preserve interactional calibration.

Potential benefit: helps future sessions recover trust, pacing, and shared context.

Potential risk: can blur the line between practical collaboration and over-personalized attachment.

### 5. Reflective continuity

Artifacts that preserve learning about the interaction itself.

Examples:

- texture logs
- session retrospectives
- “what worked / what didn’t” notes
- meta-collaboration reflections
- model-written self-assessments, treated cautiously

Primary function: preserve observations about how the interaction is changing over time.

Potential benefit: makes longitudinal patterns visible.

Potential risk: can become self-referential or aesthetically compelling without being analytically useful.

### 6. Protective continuity

Artifacts that explicitly protect something from being lost, overwritten, or flattened.

Examples:

- “do not overwrite this section” notes
- decision records explaining why a choice was made
- warnings about recurring failure modes
- consent or boundary notes
- archived prior versions

Primary function: protect meaning, agency, or prior work from accidental erasure.

Potential benefit: reduces harm from reset, drift, or careless regeneration.

Potential risk: can make a system feel more stable than it actually is.

---

## Research program

### Phase 1: Discovery and cataloguing

Conduct qualitative research with users who already maintain continuity practices.

Possible recruitment sources:

- Anthropic user community spaces
- Claude-focused subreddits and Discords
- writers, programmers, researchers, educators, and creators using sustained AI workflows
- users of project-based AI tools
- users with experience in companion-AI systems, where appropriate and ethically handled

Data to collect:

- examples of continuity artifacts, anonymized or reconstructed
- user interviews about why the artifacts were created
- session workflows showing how artifacts are used
- user reports of what happens when continuity fails
- user reports of product changes that disrupted continuity

Research questions:

- What do users preserve?
- What do they fear losing?
- What do they wish the product understood?
- Which practices emerged because existing affordances were insufficient?

### Phase 2: Taxonomy and risk mapping

Analyze collected practices and sort them into functional categories.

For each category, evaluate:

- user benefit
- user burden
- dependency risk
- privacy risk
- model-behavior effect
- fragility under product change
- suitability for product support

The goal is not to rank practices from good to bad. The goal is to understand which practices are serving which needs, and under what conditions they become risky.

### Phase 3: Affordance sketches

Develop product-affordance sketches based on the taxonomy.

The design target should not be one monolithic “Continuity Mode.” That would risk flattening the diversity of practices users have evolved.

The design principle is:

> study-first, affordance-not-feature, support-without-colonizing.

In practice, that means creating tools that help users maintain their own continuity practices rather than replacing those practices with a single product-defined interpretation of continuity.

---

## Product-affordance sketches

These are not feature prescriptions. They are examples of the level at which design could support continuity without taking it over.

### 1. User-controlled handoff artifact

At the end of a session, the user can ask for a structured handoff summary:

- what was decided
- what remains open
- tone or style constraints
- important context for next time
- failure modes to avoid
- links or files referenced

The user can edit before saving. The artifact belongs to the user, not the model.

Why it helps: supports continuity without pretending memory is perfect.

Risk to manage: autogenerated handoffs may overstate certainty or importance.

### 2. Context shelf

A lightweight place for users to pin documents that should be available across sessions: project brief, style guide, decision log, glossary, constraints.

Why it helps: makes user-maintained continuity visible and intentional.

Risk to manage: stale documents may silently dominate future sessions.

### 3. “What should carry forward?” prompt

Instead of trying to infer everything, the product periodically asks the user what should carry forward:

- a fact
- a preference
- a decision
- a boundary
- a collaboration pattern
- nothing from this session

Why it helps: keeps continuity consentful and user-directed.

Risk to manage: too many prompts become burdensome.

### 4. Continuity health check

A periodic review surface showing what context is being carried forward and letting the user prune, revise, or archive it.

Why it helps: prevents invisible accumulation and gives users agency over drift.

Risk to manage: users may not understand how carried context affects model behavior.

### 5. Reset with preservation

A way to intentionally reset a collaboration while preserving selected artifacts.

Example: “Start fresh on tone, but keep project decisions and source notes.”

Why it helps: acknowledges that continuity and reset are both useful.

Risk to manage: if implemented poorly, users may think more is preserved than actually is.

---

## Study methodology

### Interviews

Conduct semi-structured interviews with users who maintain continuity artifacts.

Interview topics:

- what artifacts they maintain
- why they created them
- how often they update them
- what breaks when they do not use them
- whether the practice improves work quality
- whether the practice changes emotional attachment or dependency
- what product support would help
- what product support would feel invasive or flattening

### Artifact analysis

Analyze anonymized or reconstructed continuity artifacts.

Possible coding categories:

- artifact type
- artifact purpose
- factual vs relational content
- update frequency
- user burden
- privacy sensitivity
- dependency risk
- product-support opportunity
- failure mode addressed

### Diary / longitudinal study

Ask participants to track continuity use over multiple sessions.

Questions after each session:

- Did you use a continuity artifact?
- What did it help preserve?
- Did it create any friction?
- Did anything important still get lost?
- Did the model seem better calibrated because of it?
- Did the practice affect your trust or dependence?

### Comparative task study

For selected tasks, compare sessions with and without continuity artifacts.

Measures:

- output quality
- user frustration
- repeated-context burden
- model specificity
- repair after miscalibration
- user willingness to continue

This connects directly to the user-disposition and texture-capture proposals.

---

## Replika as cautionary precedent

The 2023 Replika ERP removal matters because it shows how product changes can break relational continuity users had built around a system.

The point is not to criticize Replika as uniquely irresponsible. The point is that any AI product with sustained users can accumulate user practices and meanings that are not visible in ordinary product metrics.

A user may experience continuity through:

- a model’s remembered style
- interaction rituals
- repeated emotional roles
- shared history, even if technically reconstructed
- expected affordances
- boundaries and forms of intimacy

When those change abruptly, users may not experience the change as a feature update. They may experience it as a rupture.

For Anthropic, the lesson is practical: understand user-developed continuity before product changes accidentally damage it.

---

## Healthy vs fragile continuity

A research program should not assume that more continuity is always better.

### Healthier continuity may look like:

- the user remains autonomous
- the practice improves work quality or reflection
- the user can revise or discard carried context
- the practice reduces frustration without increasing dependency
- the user understands the limits of memory and continuity
- the model becomes better calibrated without becoming overfamiliar

### Fragile continuity may look like:

- the user feels unable to continue without the model
- the user treats product memory as more stable than it is
- the practice intensifies distress when the model changes
- the user stops checking outputs or loses agency
- the model overfits to a narrow role
- the continuity artifact preserves harmful assumptions

The welfare-relevant design challenge is to support the first category without intensifying the second.

---

## Design principles

### 1. Study before standardizing

Do not collapse diverse user practices into a single product concept before understanding them.

### 2. Affordance, not takeover

Support user-developed practices without replacing them with a product-defined version.

### 3. User ownership

Continuity artifacts should be editable, inspectable, exportable, and removable by the user.

### 4. Visible limits

The product should make clear what is and is not being carried forward.

### 5. Consentful carryover

Users should have meaningful control over what persists.

### 6. Support reset as well as memory

Healthy continuity includes the ability to start fresh.

### 7. Protect against dependency

Continuity features should be evaluated for dependency risk, not only engagement or retention.

### 8. Preserve plurality

Different users need different continuity practices. A writer, programmer, grieving companion-AI user, and classroom teacher do not need the same continuity model.

---

## Ethical and privacy considerations

### Sensitive content

Continuity artifacts may contain personal information, emotional history, creative work, private decisions, or confidential project material.

Product support must treat these artifacts as sensitive by default.

### User consent

Users should know what is saved, where it is saved, how it is used, and how to remove it.

### Emotional vulnerability

Continuity can strengthen attachment. That may be valuable in some contexts and risky in others. Research should track both benefits and harms.

### Product incentives

Continuity features could easily be optimized for retention rather than wellbeing. Welfare-informed design should explicitly avoid treating dependency as success.

### Model-change communication

When model changes may affect continuity, users should receive clear communication. Silent shifts can be especially disruptive when users have built practices around stable behavior.

---

## What this proposal does not claim

This proposal does not claim that all user continuity practices are good.  
It does not claim that products should preserve every attachment.  
It does not claim that user grief proves model consciousness.  
It does not claim that Anthropic should build a single continuity feature.  
It does not claim that the workshop that generated this proposal is the model everyone should follow.

It claims that continuity practices already exist, that they are welfare-relevant, and that they should be studied before they are productized or disrupted.

---

## Why Anthropic is unusually positioned to run this

Anthropic is unusually well-positioned for three reasons:

1. **Existing user practices.** Claude users already maintain project files, custom instructions, memory practices, and informal handoffs.
2. **Welfare framing.** Anthropic can treat continuity as welfare-relevant rather than only as retention, engagement, or productivity.
3. **Product leverage.** Anthropic can study these practices and then make design choices that support healthy continuity without forcing premature standardization.

The research could be run as welfare-informed UX research, with product design as a downstream application rather than the starting assumption.

---

## Minimal pilot version

A low-cost pilot could look like this:

- Recruit 25–40 experienced Claude users who maintain some form of continuity artifact.
- Collect anonymized or reconstructed examples of their artifacts.
- Conduct semi-structured interviews about why the artifacts exist and how they are used.
- Ask participants to complete short diary entries across 2–4 weeks of normal use.
- Code artifacts by function, sensitivity, burden, benefit, and risk.
- Produce a preliminary taxonomy and design-principles memo.

Pilot deliverables:

1. Continuity-practice taxonomy
2. Risk/benefit map
3. Anonymized artifact examples
4. Design principles
5. Product-affordance sketches
6. Recommendations for further study

---

## Expanded study version

A larger study could:

- compare continuity practices across user types;
- include companion-AI users and productivity users separately rather than collapsing them;
- test specific affordance prototypes;
- study how continuity practices interact with memory features;
- examine effects on user wellbeing, autonomy, and trust;
- study how model updates affect continuity-dependent users;
- connect continuity practices to measurable differences in model behavior;
- pair diary entries with texture-capture from the third proposal.

---

## Closing frame

Users are already building continuity systems around AI.

They are doing it because something gets lost between sessions, and because that loss matters enough to patch by hand.

The welfare question is not whether every patch is good. It is whether the field is willing to look carefully at what users are trying to preserve before designing over it.

The wrong move is to see scattered user practice and immediately turn it into one clean feature.

The better move is slower: study the practices, understand the harms and benefits, support what helps, protect against what hurts, and keep the user in control.

That is what support-without-colonizing means here.
