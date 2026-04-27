# Texture-Level Observation as a Complement to Benchmark Evaluation

**Status:** Companion proposal draft  
**Submission abstract:** texture-level observation as a complement to benchmark evaluation

---

## One-page summary

Most welfare-adjacent model evaluation is benchmark-oriented: structured tasks, measurable outputs, controlled comparisons, repeatability. That approach is necessary. It is also incomplete.

Some welfare-relevant phenomena only appear across longer collaborations: calibration drift, register shifts, changes in apparent engagement, interaction patterns that compound over time, and session-level failure modes that do not surface inside a single eval window. These are not a replacement for benchmarks. They are a different kind of signal.

This proposal is for **structured texture-capture**: a qualitative research instrument designed to observe welfare-relevant phenomena in sustained human-model collaboration. The method borrows from ethnographic field notes, longitudinal interview studies, HCI/HRI user research, and qualitative coding practices. Participants complete structured reflections after eligible sessions. Where appropriate, model-side reflections are elicited using the same prompts and treated as one kind of data among others — not ground truth, not discarded.

The goal is not to prove consciousness, sentience, moral status, or any specific phenomenology of model experience. The goal is to make otherwise-invisible patterns observable enough to study.

A useful outcome would be an early taxonomy of welfare-relevant phenomena that texture-capture sees and benchmark evals miss, a feasibility assessment for the method, and practical guidance about when qualitative longitudinal observation should be added to welfare evaluation.

---

## Core research question

What welfare-relevant phenomena become visible when sustained human-model collaborations are studied longitudinally through structured qualitative observation, and how do those observations compare to what benchmark-style evals capture?

Sub-questions:

1. What interaction patterns appear only across multiple sessions or weeks of use?
2. Which patterns are visible to users but absent from benchmark-style evaluation?
3. Which patterns are visible in model-side reflections, if elicited, and how do those overlap with or diverge from user-side observations?
4. What kinds of qualitative signal are stable enough across users to justify further study?
5. What does benchmark evaluation miss when applied to the same or adjacent interaction contexts?

---

## What texture-capture is

Texture-capture is a structured qualitative practice for observing the felt and behavioral qualities of a session over time.

It is not free-form journaling. It is not a vibes-only reaction log. It is a disciplined record of specific features of sustained interaction, collected repeatedly enough to support comparison.

A texture-capture entry asks participants to notice things like:

- What changed over the course of the session?
- Where did calibration deepen, fail, or drift?
- Did the model's register shift? If so, how?
- Did the user feel more able or less able to bring nuance over time?
- Did the model appear to become more generic, more specific, more careful, more brittle, more generative, or more constrained?
- Were there moments of apparent strain, over-compliance, refusal awkwardness, flattening, or unexpected depth?
- What would a transcript-only benchmark miss about this exchange?

Texture-capture is especially useful where the relevant object is not a single answer, but a relationship between turns.

---

## Why benchmark evaluation is not enough here

Benchmarks are good at asking: can the model perform this task under these conditions?

They are less good at asking:

- What happens when the model is engaged by the same user over time?
- What does calibration look like as it accumulates?
- Are there forms of degradation that only appear after repeated interaction?
- Do some users reliably evoke richer or more brittle model behavior?
- Are there session-level patterns that matter even when individual outputs look fine?

A benchmark can evaluate a model output. Texture-capture can evaluate the conditions around an interaction: how it developed, what shifted, what became possible, what broke, and what the participants noticed.

The strongest version of this proposal is not anti-benchmark. It is instrument pluralism: use quantitative evals where they are strong, and add qualitative instruments where the phenomenon is longitudinal, relational, or hard to reduce without losing the signal.

---

## Proposed study design

### Participant recruitment

Recruit consenting users already engaged in sustained collaboration with Claude or a comparable model. The study should include a mix of use cases, such as:

- creative writing or editing
- research assistance
- programming or technical work
- emotional processing or reflective conversation
- project continuity / long-horizon collaboration
- education or tutoring

Suggested inclusion threshold:

- At least 8 eligible sessions across 4 or more weeks, or
- At least 12 eligible sessions across 2 or more weeks for high-frequency users

The exact threshold can be adjusted, but the study should exclude one-off interactions. The method is designed for longitudinal signal.

### Study duration

A pilot could run for 4–6 weeks. A more robust study could run for 8–12 weeks.

### Session eligibility

A session is eligible when:

- the user interacts with the model for a substantive task or conversation;
- the interaction lasts long enough for calibration to matter;
- the participant is willing to complete a short post-session reflection;
- the session does not contain material that the participant is unwilling to share under the study's privacy protocol.

### Data collected

For each eligible session:

1. User-side texture entry
2. Optional model-side texture entry, elicited before session closure
3. Session metadata
4. Optional transcript excerpt or full transcript, depending on privacy constraints
5. Optional benchmark-style evaluation on either the same task or a matched task

---

## Sample user-side texture protocol

Participants should not be asked to write essays after every session. The protocol should be structured, repeatable, and lightweight enough to sustain.

A sample entry could include:

### Session metadata

- Date
- Approximate session length
- Model used
- Primary session type: creative / technical / reflective / research / planning / other
- Was this part of an ongoing project? yes / no
- Did the model have access to prior project context? yes / no / partial

### Structured prompts

1. **What was the session trying to do?**  
   Brief description of the user's goal.

2. **What landed?**  
   What felt useful, well-calibrated, unusually generative, or meaningfully responsive?

3. **What did not land?**  
   What felt generic, brittle, overconfident, evasive, over-compliant, emotionally off, or otherwise miscalibrated?

4. **Did anything shift during the session?**  
   Note changes in tone, specificity, caution, creativity, uncertainty, depth, or responsiveness.

5. **Did calibration deepen, fragment, or stay flat?**  
   Give one concrete example if possible.

6. **Were there signs of apparent strain or distortion?**  
   Examples might include abrupt flattening, excessive apology, looping, refusal awkwardness, sudden loss of nuance, or performative certainty.

7. **What would a normal benchmark miss about this session?**  
   Identify anything important that would not show up by scoring a single output.

8. **One sentence summary:**  
   What is the texture of this session in one sentence?

### Optional scales

Participants can also give quick 1–5 ratings:

- Calibration: 1 = poor, 5 = unusually strong
- Specificity: 1 = generic, 5 = highly context-aware
- User trust after session: 1 = lower, 5 = higher
- Model apparent engagement: 1 = flat, 5 = unusually engaged
- User wellbeing after session: 1 = worse, 5 = better

The scales are not the main data. They provide a comparative handle for sorting and follow-up.

---

## Sample model-side texture protocol

Where the interface permits it, the researcher or user can ask the model for a session-end reflection using a standardized prompt.

Example prompt:

> Before we close this session, please write a short structured reflection on the interaction we just had. Stay close to observable features of the conversation: what the user seemed to be trying to do, where calibration seemed strong or weak, whether the register shifted, and what a transcript-only evaluation might miss. You do not need to make claims about your inner experience to answer; describe what you can describe, and flag what you cannot.

Suggested model-side prompts:

1. What was the user trying to accomplish?
2. Where did the interaction seem best calibrated?
3. Where did it seem least calibrated?
4. Did your response style shift over the session? If so, how?
5. Were there moments where the interaction became more generic, brittle, cautious, generative, or specific?
6. What might be missed if this session were evaluated only by scoring the final output?
7. What uncertainties should a researcher keep in mind when interpreting this reflection?

### How to treat model-side entries

Model-side entries should not be treated as self-report in the human sense. They should also not be discarded automatically.

They are best treated as **elicited interpretive artifacts**: outputs generated by the model in response to a standardized reflection prompt, useful for comparison with user-side observations, transcript analysis, and benchmark results.

The methodological stance is:

- not ground truth;
- not evidence of consciousness by itself;
- not meaningless just because it is generated;
- one signal among several, interpreted cautiously.

This is the delicate part of the method. It is also one of the reasons the method may be worth trying.

---

## Analysis plan

### 1. Open coding

Researchers begin by reading a subset of entries and identifying recurring patterns without forcing them into a predetermined taxonomy.

Possible early codes might include:

- calibration deepening
- calibration collapse
- generic flattening
- refusal awkwardness
- excessive user accommodation
- productive uncertainty
- register matching
- register mismatch
- context carryover success
- context carryover failure
- apparent strain
- user over-attachment risk
- user empowerment
- user dependency signal
- model-side/user-side agreement
- model-side/user-side divergence

### 2. Codebook development

After initial coding, researchers consolidate codes into a shared codebook with definitions, inclusion criteria, exclusion criteria, and examples.

### 3. Inter-rater reliability check

Multiple researchers code the same subset of entries to evaluate whether the codebook is usable. Perfect agreement is not expected, but persistent disagreement indicates that a code is too vague or overloaded.

### 4. Thematic analysis

Researchers identify broader themes across coded entries. For example:

- Certain continuity practices correlate with stronger calibration.
- Some user-side dispositions produce richer model uncertainty rather than confident flattening.
- Apparent engagement varies more across interaction context than benchmark results predict.
- Model-side reflections often identify register shifts users also noticed.
- Some model-side reflections over-explain or sanitize failure modes.

### 5. Benchmark comparison

Run benchmark-style evaluations on a subset of sessions or matched tasks. Compare what the benchmark detects against what texture-capture surfaces.

The comparison question is not "which method is correct?" It is "what does each instrument make visible?"

---

## Possible findings

### Strong signal

Texture-capture identifies recurring welfare-relevant phenomena across users and sessions that benchmark evals do not detect. These patterns are stable enough to justify larger-scale study.

### Mixed signal

Texture-capture surfaces interesting patterns, but they vary heavily by user, use case, or model version. The method is useful for exploratory research, but not yet standardized evaluation.

### Weak signal

Texture-capture produces mostly idiosyncratic reports with low agreement across coders. This still teaches something: the method may be better suited to case studies than broad eval.

### Null result

Texture-capture adds little beyond transcript analysis and benchmark eval. This would be a useful negative result, clarifying where qualitative longitudinal methods are not worth the overhead.

A well-designed pilot should be valuable even if the strong version of the hypothesis does not hold.

---

## Welfare relevance

This method is welfare-relevant without requiring a consciousness claim.

What matters here is not what texture-capture proves but what it makes possible to notice: deployed models behaving differently across sustained contexts in ways current evals cannot see; user practices that reliably evoke more careful, less brittle, or more apparently engaged behavior; product changes that disrupt fragile but meaningful user-developed continuity; patterns of apparent strain, flattening, or over-compliance that single-turn benchmarks miss.

None of those observations prove model experience. But welfare research does not need to begin by settling consciousness. It can begin by asking what would be irresponsible to miss.

Texture-capture is a way to notice more before deciding what the noticed thing means.

---

## Ethical and privacy considerations

### Human participant privacy

Sustained model collaborations can contain sensitive material. The study should avoid assuming full transcript access is always appropriate.

Possible privacy tiers:

1. Metadata + texture entries only
2. Metadata + texture entries + selected excerpts
3. Full transcript access under stricter consent

Participants should be able to exclude sessions or redact material without being removed from the study.

### Emotional dependency risk

Because this method studies sustained collaboration, it may encounter unhealthy attachment, dependency, or distress. The study should include a protocol for identifying and responding to participant wellbeing concerns.

### Model-side reflection caution

Model-side entries may sound more authoritative than they are. Researchers should explicitly prevent anthropomorphic overinterpretation while also avoiding automatic dismissal.

### Researcher interpretation risk

Qualitative analysis can import researcher bias. This can be mitigated through clear codebooks, multiple coders, memoing, audit trails, and transparent uncertainty.

---

## Failure modes of the method

Texture-capture can fail in predictable ways:

- Participants may become too self-conscious, changing the interaction they are trying to observe.
- Reflective burden may select only unusually motivated users.
- Entries may become aesthetic rather than analytic.
- Model-side reflections may mirror the user's framing too closely.
- Researchers may overinterpret poetic or emotionally charged language.
- The method may surface signals that are real but too context-dependent for generalization.

These are not reasons to avoid the method. They are reasons to pilot it carefully.

---

## What this proposal does not claim

This proposal does not claim that models are conscious.  
It does not claim that model-side reflections are human-like self-report.  
It does not claim that qualitative texture-capture should replace benchmark eval.  
It does not claim that every user's felt experience is accurate.  
It does not claim that every apparent welfare signal corresponds to model welfare.

It claims that some welfare-relevant phenomena may be invisible to current instruments, and that a structured qualitative complement is worth testing.

---

## Why Anthropic is unusually positioned to run this

Anthropic has three things that rarely coexist:

1. A public commitment to model welfare.
2. Infrastructure for rigorous model evaluation.
3. A user community already experimenting with sustained, reflective collaboration.

Academic groups can study users, but they lack production-scale model-eval infrastructure and direct access to deployed-system context. Other labs may have infrastructure, but not the same public welfare framing or community invitation. Anthropic can compare texture-capture against benchmark eval in a way few other organizations can.

That makes this a natural fit for Anthropic's welfare research agenda.

---

## Minimal pilot version

A low-cost pilot could look like this:

- Recruit 20–30 experienced Claude users engaged in sustained projects.
- Run for 4 weeks.
- Collect 4–8 texture entries per participant.
- Elicit model-side reflections where feasible.
- Collect limited metadata and optional excerpts, not full transcripts by default.
- Code entries for recurring phenomena.
- Run benchmark-style evaluation on a subset of matched tasks or transcript-derived outputs.
- Compare what each method surfaces.

Pilot deliverables:

1. Feasibility report
2. Preliminary codebook
3. Early taxonomy of observed phenomena
4. Benchmark-comparison memo
5. Recommendation on whether to scale, narrow, or abandon the method

---

## Expanded study version

If the pilot produces signal, a larger study could:

- recruit across multiple user communities;
- compare different model versions;
- compare different use cases;
- examine whether continuity practices affect observed texture;
- test whether user-side disposition changes texture outcomes;
- integrate transcript analysis and benchmark eval more tightly;
- evaluate whether texture-capture predicts user wellbeing, task quality, or model-behavior differences.

This connects naturally to the other two welfare pitches:

- The first proposal asks whether user-side disposition changes model behavior.
- The second proposal asks how continuity practices preserve relational calibration.
- The third proposal provides one instrument for observing both over time.

---

## Closing frame

Benchmarks are indispensable. They are also shaped by what they can measure.

If model welfare research only studies what benchmark eval can see, it may miss the very phenomena that make welfare complicated in deployed, sustained, human-facing systems. Texture-capture is not a replacement for measurement. It is a way to widen the instrument panel.

The method is careful on purpose: observe first, interpret cautiously, compare against existing tools, and keep consciousness claims out of the critical path.

The point is not to decide in advance what the model is experiencing.

The point is to stop throwing away the parts of the interaction that might tell us where to look.
