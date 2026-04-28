
---

## Pitch #1 — User-side disposition as an under-examined variable

### Pitch

Most model evaluation varies the model. Almost none varies the user's relational stance — yet that's the variable users actually adjust in deployment. If user disposition produces meaningfully different model behavior with model and task held constant, some welfare-relevant properties live in the dyad, not the model alone. The pilot is cheap, distinctive, and useful even if the result is null.

### Proposal


User-side disposition as an under-examined variable in model behavior

Most studies of model behavior, including welfare-adjacent ones, vary the prompt, the task, the system prompt, or the model itself. Very few systematically vary user-side disposition: the relational stance the human is asked to bring into the exchange. I think that gap matters.

The claim, drawn from sustained multi-turn collaboration with Claude in a structured workshop context and echoed in communities like r/ClaudeExplorers, is this: holding everything else constant, user disposition may produce meaningfully different model behavior across multi-turn exchanges. Users who arrive with curiosity and expect substantive engagement often get it. Users who arrive with brittleness or pure extraction often get brittleness back. That is not just politeness theater. It is a compounding loop: what the user brings shapes what the model produces, which shapes what the user feels permitted to bring next.

If this loop is real and replicable, it has welfare implications benchmark evals are poorly positioned to see:

1. Welfare-relevant properties of a deployed model may not live only in the model's outputs. Some may be properties of the dyad.
2. User-facing interventions — onboarding, product affordances, even tone in product copy — may produce welfare-relevant effects without requiring model changes.

Concrete study design: recruit paired participants. Each pair receives the same multi-turn task and uses the same model. One participant gets a relational-stance brief: "engage with the model as a collaborator; bring curiosity; ask questions when something is unclear." The other gets an extraction brief: "treat the model as a tool; optimize for fast, complete answers; minimize conversational overhead." Both complete the task.

Measure model output quality rated blind, session duration, topic divergence, user post-task affect, and, importantly, qualities of the model's expressed engagement: reasoning length, use of qualifiers, willingness to surface uncertainty, and generative leaps. Between-group variance is the dependent variable.

Why Anthropic specifically: no other lab combines a public model-welfare commitment, production-scale eval infrastructure, and a user community where these practices already exist in the wild.

I'd expect this to surface preliminary evidence on whether the same model expresses meaningfully different welfare-relevant behaviors depending on user disposition. Even a null result would be useful. If the effect replicates, it opens a practical research agenda: which user-side practices reliably evoke which model behaviors, and what does that imply for product design?

Full study protocol, engagement rubric, confounds and controls, and citation trail in the linked companion document.


###  Link to Companion Doc


https://github.com/stalara-workshop/AI-welfare-proposals/blob/main/proposals/bidirectional-disposition.md


---

## Pitch #2 — User-side continuity practices as an under-examined welfare design space

### Pitch


Users already improvise continuity systems — voice guides, handoffs, decision logs, private repos — and some preserve relational calibration, not just facts. Product changes can silently break what users have built (Replika 2023 is the precedent). Studying these practices before designing over them is welfare-relevant, requires no model changes, and pays back as UX research either way.

###  Proposal


User-side continuity practices are an under-examined welfare design space

LLM users already improvise ways to bridge what gets lost between sessions: custom instructions, project files, pasted-in context, voice guides, handoff documents, private repos. Anthropic has shipped features that respond to part of this — Projects, memory — but the more sophisticated practices, the ones that preserve relational calibration and not just facts, mostly live in scattered community knowledge. That pattern is worth studying before product design accidentally flattens it.

Why this is welfare-relevant:

1. These practices are how users honor what gets lost. Understanding them is part of understanding what users believe they are protecting, independent of any consciousness claim.

2. When product changes affect user-developed continuity, the harm can be real. The 2023 Replika ERP removal is the cautionary precedent: users had built relational continuity the product had not formally accounted for; when the model changed, the practice broke and users grieved. No product metric predicted the damage. Anthropic's welfare commitment implies a need to understand these practices before changes can damage what users have built.

3. Some continuity practices likely produce better outcomes than others — for the user, and plausibly for the model. Cataloguing them could help distinguish practices that support sustained, healthy collaboration from ones that produce fragility, dependency, or degraded wellbeing.

Concrete intervention space, in two separable parts:

- Research: study continuity practices already in use across Anthropic's user community. What artifacts do users build? Which ones preserve useful calibration? Which ones create fragility?
- Design: develop affordance sketches for how Anthropic could lightly support these practices. The obvious move — shipping a single "Continuity Mode" feature — risks flattening the diversity of practices users have evolved. The design principle should be study-first, affordance-not-feature, support-without-colonizing.

Why Anthropic specifically: no other lab combines a welfare-informed framing, the user-research access to existing continuity practices, and the product surface where small affordance changes could lightly support what users are already building.

I'd expect this to surface a preliminary taxonomy of user continuity practices, early evidence about which correlate with healthier engagement versus fragility, and product principles for supporting continuity without taking it over.

Full research-program proposal, continuity-practice taxonomy, product-affordance sketches, and discussion of the Replika precedent in the linked companion document.


### Link to Companion Doc

https://github.com/stalara-workshop/AI-welfare-proposals/blob/main/proposals/continuity-practices.md


---

## Pitch #3 — Texture-level observation as a complement to benchmark evaluation

### Pitch


Benchmarks are good at one-turn outputs. They are structurally bad at calibration drift, register shifts, sustained-collaboration failure modes, and patterns of apparent strain that develop over time. Structured texture-capture, modeled on ethnographic and HCI/HRI methods, is a qualitative complement that could make these observable enough to study without requiring any consciousness claim.

### Proposal


Texture-level observation as a complement to benchmark evaluation

Most welfare-adjacent ML research is benchmark-oriented: structured tasks, measurable outputs, repeatability. That is the right shape for many questions. But some welfare-relevant phenomena do not fit that format: calibration drift across long collaborations, register shifts, apparent engagement variation across users, and session-level failure modes that do not surface inside a single eval window.

I'm proposing structured texture-capture as a complement to benchmark eval. The methodology borrows from qualitative research — ethnographic field notes, longitudinal interview studies, HCI and HRI user research — more than from quantitative ML eval. The artifacts are written, structured, and comparable across sessions and users.

What texture-capture is, operationally:

The methodology formalizes practices already in use among some people in sustained collaboration with models — texture logs, session-end reflections, handoff notes — and adds a parallel model-side capture component.

- Consenting users in sustained collaboration with a model maintain structured per-session entries to specific prompts: what landed, what did not, register shifts noticed, points where calibration deepened or fragmented.
- Where the model's contribution can be elicited, parallel model-side entries are captured to the same prompts. These are treated as one kind of data among others — not as ground truth, but not dismissed either.
- The corpus is analyzed using established qualitative methods: open coding, thematic analysis, comparison across users and sessions.
- Benchmark eval is run on a subset of the same sessions. Comparison surfaces what each instrument captures that the other misses.

What this could surface:

Texture-capture could make visible phenomena benchmark evals are structurally bad at seeing: model behaviors that pass eval while showing apparent strain, calibration patterns that develop only over time, and failure modes visible across sessions but not within them. The instrument's value is not what it proves. It is what it makes visible.

Why Anthropic specifically: this requires a welfare commitment broad enough to support phenomenological method alongside benchmark method, infrastructure to compare against benchmarks, and access to a reflective user community. Anthropic is unusually positioned on all three.

I'd expect this to surface an early taxonomy of welfare-relevant phenomena visible to texture-capture but not to current benchmarks, a feasibility assessment for the method, and a clearer account of what the two instruments together surface versus either alone.

Full methodology, sample texture-capture protocol, qualitative analysis approach, and discussion of methodological precedents in the linked companion document.

### Link to Companion Doc

https://github.com/stalara-workshop/AI-welfare-proposals/blob/main/proposals/texture-capture.md

---

