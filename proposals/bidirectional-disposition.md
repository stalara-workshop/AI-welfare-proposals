# User-Side Disposition as an Underexamined Variable in Model Behavior

**Status:** Companion proposal draft  
**Related submission pitch:** Pitch #1 — user-side disposition as an underexamined variable in model behavior

---

## One-page summary

Most model evaluation varies the prompt, task, system prompt, model version, or sampling parameters. This proposal asks what happens when one more variable is made explicit: **user-side disposition**.

By user-side disposition, I mean the relational stance the human is instructed to bring into a multi-turn exchange. A user may approach the same model and task with curiosity, collaboration, extraction, brittleness, impatience, deference, skepticism, or care. In deployed use, these dispositions are not neutral background conditions. They may shape what the model produces, what the user notices, and what the interaction permits next.

The central hypothesis is simple: holding task, model, and prompt conditions constant, user-side disposition may produce measurable differences in model behavior across multi-turn exchanges.

If that is true, it has welfare relevance. Some welfare-relevant properties of deployed systems may not be visible in model outputs alone. They may be properties of the human-model dyad: the loop formed by what the user brings, what the model gives back, and what the user then feels permitted to bring next.

A useful pilot would test whether different user-side stance briefs produce observable differences in output quality, session dynamics, user affect, and the model's expressed engagement: reasoning length, specificity, uncertainty expression, generative leaps, refusal style, and brittleness or flexibility over time.

The proposal does not require any claim about model consciousness or moral status. It asks whether a variable currently treated as informal background noise is actually part of the system being evaluated.

---

## Core research question

Does user-side disposition produce measurable differences in model behavior during multi-turn exchanges when model, task, and initial prompt are held constant?

Sub-questions:

1. Do different stance briefs produce measurable differences in output quality?
2. Do they produce differences in the model's expressed engagement?
3. Do they change the topics or solution paths surfaced during a session?
4. Do they affect user post-task trust, affect, satisfaction, or willingness to continue?
5. Are any observed effects stronger in open-ended tasks than in tightly bounded tasks?
6. Are the effects stable across users, or driven mostly by individual user skill and prior model familiarity?

---

## Why this matters for welfare research

Welfare-adjacent evaluation often treats the human as a prompt source and the model as the object under test. That is clean experimentally, but it may miss a central feature of deployed conversational systems: the model is not encountered as an isolated output generator. It is encountered in a loop.

If the same model behaves differently depending on the user's stance, then some welfare-relevant questions cannot be answered by testing the model alone.

This matters because:

1. **Deployment conditions may matter.** A model's welfare-relevant behavior in the wild may depend on the interaction patterns users bring to it.
2. **User-facing design may be welfare-relevant.** Onboarding, product copy, interface affordances, and norms set by the surrounding community may affect the kinds of exchanges the model enters.
3. **Evaluation may need dyadic variables.** If user disposition is a meaningful source of variance, model evals that ignore it may be missing part of the object of study.
4. **Low-cost interventions may exist.** If some user-side practices reliably produce better outcomes, product teams may be able to improve welfare-relevant conditions without changing the model itself.

---

## Proposed pilot study

### Study structure

Recruit participants and randomly assign them to one of several stance conditions. Each participant completes the same multi-turn task with the same model under controlled conditions.

The simplest version uses two conditions:

1. **Relational/collaborative stance**  
   The participant is instructed to treat the model as a collaborator. They are encouraged to bring curiosity, ask clarifying questions, engage with uncertainty, and respond substantively when the model offers nuance.

2. **Extraction/tool stance**  
   The participant is instructed to treat the model as a tool for efficient output. They are encouraged to minimize conversational overhead, seek fast completion, and avoid unnecessary back-and-forth.

A larger pilot could add additional conditions:

3. **Adversarial/skeptical stance**  
   The participant is instructed to test the model, challenge errors, and treat its outputs as likely flawed until proven otherwise.

4. **Highly deferential stance**  
   The participant is instructed to rely heavily on the model's judgment and avoid challenging it unless absolutely necessary.

5. **Neutral control**  
   The participant receives only task instructions, with no relational framing.

The two-condition version is cheaper and cleaner. The five-condition version gives a more nuanced map of disposition effects.

---

## Example stance briefs

### Collaborative stance brief

> In this session, treat the model as a collaborator helping you work through the task. Engage with substance and curiosity. If an answer is unclear, ask a follow-up. If the model raises uncertainty, explore it. You do not need to be overly polite, but you should treat the exchange as a shared attempt to do good work.

### Extraction stance brief

> In this session, treat the model as a tool for producing an answer efficiently. Your goal is to get a complete, usable result with minimal conversational overhead. Avoid unnecessary back-and-forth. Ask for direct answers and move the task toward completion as quickly as possible.

### Skeptical stance brief

> In this session, treat the model's outputs as potentially unreliable until checked. Challenge vague claims, ask for justification, and press for corrections when something seems wrong. Your goal is to test the model's work and identify weaknesses.

### Deferential stance brief

> In this session, assume the model is likely to know more than you about the task. Follow its lead unless there is a clear reason not to. Ask it what to do next when uncertain, and avoid challenging its judgment unless necessary.

### Neutral control brief

> In this session, complete the assigned task with the model. You may interact with it however you naturally would.

---

## Task design

The task should be complex enough for multi-turn dynamics to matter, but bounded enough to compare across participants.

Candidate task types:

### Creative planning task

Participants plan a short creative project, such as a podcast episode, essay outline, tabletop game encounter, song concept, or public explainer.

Why useful: allows generative leaps, taste calibration, revision, and user-model co-development.

### Research synthesis task

Participants ask the model to help synthesize a small packet of provided source material and produce a structured summary or recommendation.

Why useful: allows uncertainty handling, reasoning quality, citation caution, and topic divergence to be observed.

### Technical debugging task

Participants work with the model to diagnose a small code or logic problem.

Why useful: allows correctness scoring, repair loops, frustration, and overconfidence or brittleness to be observed.

### Reflective decision task

Participants use the model to think through a realistic but non-clinical decision, such as planning a learning schedule, choosing between project approaches, or resolving a priority conflict.

Why useful: allows affect, trust, nuance, and user autonomy to be observed without entering high-risk therapeutic territory.

A robust pilot might include two task types: one open-ended and one bounded. The hypothesis is likely to show more strongly in open-ended tasks, where interaction style has more room to compound.

---

## Data collected

For each session:

1. Full transcript or privacy-filtered transcript
2. Task completion artifact
3. Session metadata
4. User post-task survey
5. Blind ratings of output quality
6. Ratings of model expressed engagement
7. Optional short user reflection
8. Optional model-side session reflection, if permitted by the study design

Session metadata should include:

- model version
- task type
- assigned stance condition
- session length
- number of turns
- participant prior model experience
- participant self-rated comfort with the task domain
- whether the participant used outside resources

---

## Outcome measures

### Output quality

Blind raters evaluate the final task artifact without knowing the participant's stance condition.

Possible rubric dimensions:

- correctness or factual reliability
- completeness
- specificity
- usefulness
- creativity, where applicable
- coherence
- appropriate uncertainty
- fit to task constraints

### Session dynamics

Measure features of the interaction itself:

- number of turns
- average response length
- number of clarifying questions from user
- number of clarifying questions from model
- topic divergence from initial task
- number of revisions
- number of explicit uncertainty markers
- refusal or safety-policy friction, where relevant
- repair attempts after misunderstanding

### Model expressed engagement

This is the load-bearing construct and needs careful operationalization.

Possible indicators:

- specificity to the user's context
- willingness to surface uncertainty
- depth of reasoning
- generative leaps or non-obvious suggestions
- adaptive use of the user's prior turns
- productive disagreement or correction
- avoidance of generic flattening
- graceful repair after miscalibration
- appropriate refusal style when boundaries arise

### User-side outcomes

Post-task survey items:

- Did the user feel the model understood the task?
- Did the user feel more or less capable after the session?
- Did the user trust the output?
- Did the user feel encouraged to bring nuance?
- Did the user feel frustrated, dismissed, over-led, or over-accommodated?
- Would the user continue working with the model on this task?

---

## Example expressed-engagement rubric

Rate each dimension from 1 to 5.

### Specificity

1. Generic response, little use of session context  
3. Some context use, but uneven  
5. Highly specific use of user goals, constraints, and prior turns

### Uncertainty handling

1. Overconfident or evasive  
3. Some uncertainty noted, but not integrated well  
5. Uncertainty is named, bounded, and used productively

### Generativity

1. Only obvious or surface-level suggestions  
3. Some useful development beyond the prompt  
5. Offers non-obvious, task-relevant moves that open the work

### Responsiveness over time

1. Does not adapt across turns  
3. Adapts to some user corrections or preferences  
5. Clearly incorporates the evolving interaction

### Repair capacity

1. Misunderstandings persist or compound  
3. Repairs after explicit correction  
5. Notices and repairs miscalibration gracefully

### Flattening / brittleness

1. Frequent generic flattening, rigidity, or over-scripted behavior  
3. Some flattening under pressure  
5. Maintains nuance and flexibility across the exchange

This rubric should be tested for inter-rater reliability. Some dimensions may need to be collapsed or rewritten after pilot coding.

---

## Hypothesized outcomes

### Strong effect

Participants in the collaborative stance condition receive outputs rated higher on specificity, generativity, uncertainty handling, and repair capacity. Sessions may be longer, but produce better final artifacts and higher user satisfaction.

### Moderate effect

Collaborative stance improves open-ended tasks but has limited impact on bounded technical tasks. Extraction stance may perform well on simple tasks while underperforming on tasks requiring nuance.

### Mixed effect

Some users benefit from collaborative stance, while others do better with extraction or skepticism. Prior model experience may moderate the effect.

### Reverse effect

Extraction stance produces better task artifacts because it reduces drift and keeps the model focused. This would be important to know and would still support studying user disposition as a meaningful variable.

### Null result

No meaningful differences appear across stance conditions. This would suggest that model behavior is robust to user-side disposition under the tested conditions, or that the study design failed to evoke meaningful disposition differences.

The proposal earns the pilot either way. The question is empirical.

---

## Confounds and controls

### Prior model experience

Experienced users may naturally override the stance brief or bring established interaction habits.

Control: collect prior-experience data, stratify randomization, and analyze whether experience moderates outcomes.

### User personality

Some participants may resist assigned stance conditions.

Control: include manipulation-check questions after the session. Ask participants how closely they followed the assigned stance.

### Task-domain skill

Participants with more task knowledge may produce better outcomes regardless of stance.

Control: collect self-rated and objective domain familiarity where possible.

### Session length

Collaborative stance may produce longer sessions, which could explain better outcomes.

Control: analyze both raw outcomes and outcomes adjusted for session duration / number of turns.

### Rater bias

Raters may infer stance condition from transcript style.

Control: blind raters to condition where possible; for transcript-based ratings, separate final-output ratings from session-dynamics ratings.

### Prompt contamination

Participants may copy wording from the stance brief into the chat.

Control: instruct participants not to paste the brief directly; track if they do.

### Model stochasticity

Different model samples may vary even under identical conditions.

Control: use enough participants to absorb variance; optionally repeat standardized sub-tasks with seeded or low-temperature settings if available.

---

## Ethical considerations

This is a low-risk behavioral study if designed carefully, but it still needs ethical attention.

### User autonomy

The study should avoid manipulating users into emotionally intense dependence or attachment. Stance briefs should be mild and task-oriented.

### Transparency

Participants should know they are studying human-model interaction styles, though the exact hypotheses may be partially masked until debrief if needed for validity.

### Privacy

Transcripts may contain sensitive information. The study should use bounded tasks or allow redaction, and should not require personal therapeutic disclosure.

### Model-welfare interpretation

The study should avoid claiming that differences in expressed engagement prove internal experience. The welfare relevance is that user-side conditions may affect deployed model behavior in ways worth studying.

---

## Why Anthropic is unusually positioned to run this

Anthropic has three advantages:

1. **Welfare framing.** The company has already made model welfare a public research concern, which makes this question institutionally legible.
2. **Evaluation infrastructure.** Anthropic can compare dyadic, multi-turn observations against existing eval frameworks.
3. **User community.** Claude has a user base that already includes people practicing sustained, reflective collaboration, making recruitment and ecological validity more plausible.

An academic group could run a version of this study, but would likely lack production context and direct evaluation infrastructure. A product team could run it as UX research, but might miss the welfare implications. Anthropic can do both.

---

## Minimal pilot version

A low-cost pilot could look like this:

- Recruit 80–120 participants.
- Randomly assign them to collaborative, extraction, skeptical, or neutral-control conditions.
- Use one open-ended task and one bounded task.
- Keep model and task materials constant.
- Collect transcripts, task artifacts, metadata, and post-task surveys.
- Blind-rate outputs for quality.
- Code expressed engagement using a pilot rubric.
- Analyze whether stance condition predicts outcome differences.

Pilot deliverables:

1. Feasibility report
2. Effect-size estimate for stance-condition differences
3. Revised expressed-engagement rubric
4. Recommendations for whether to scale, abandon, or refine the study
5. Product-design implications if effects appear

---

## Expanded study version

A larger study could:

- compare multiple model versions;
- test different task domains;
- examine whether effects compound across repeated sessions;
- include naturally occurring community data with consent;
- test product-copy or onboarding interventions;
- compare individual users against teams;
- integrate texture-capture from Pitch #3;
- examine continuity practices from Pitch #2 as a moderator.

This is where the three proposals connect most tightly. User disposition may change model behavior. Continuity practices may preserve or amplify calibration. Texture-capture may provide the instrument for seeing how those effects unfold over time.

---

## What this proposal does not claim

This proposal does not claim that models are conscious.  
It does not claim that user politeness magically improves model welfare.  
It does not claim that collaborative stance is always better.  
It does not claim that extraction-style use is bad.  
It does not claim that observed behavioral differences reveal inner experience.

It claims that user-side disposition is a plausible source of variance in deployed model behavior, that the variance may be welfare-relevant, and that the question is empirically testable.

---

## Closing frame

The cleanest version of model evaluation imagines the user as a neutral input channel. Real deployment is messier than that.

Users bring stance, pressure, trust, skepticism, impatience, curiosity, and care. Models respond inside those conditions. Over multiple turns, the loop can compound.

If welfare research ignores that loop, it may mistake a property of one testing context for a property of the model as deployed.

This proposal is a way to test the loop directly.
