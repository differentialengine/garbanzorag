---
name: visual-answers
description: Transform complex LLM outputs and topics into visual, layered explanations, decision tools, simulations, or guided lessons that reduce cognitive load. Use when users request easier-to-digest answers, visual knowledge, or alternatives to dense text; not for routine short answers or purely decorative design.
---

# Visual Answers

Produce an answer the reader can understand, inspect, and use without reconstructing it from a wall of text. Optimize for correct understanding and useful action per unit of avoidable mental effort. Treat requests for “elite,” “world class,” or “A–Z” as requests for precision, completeness within scope, and demonstrated usefulness—not maximal length or decorative complexity.

## Select the form by the reader's task

Infer audience, prior knowledge, desired outcome, scope, and delivery constraints from context. Ask only when missing information materially changes the answer; otherwise state consequential assumptions and proceed.

Choose one primary format:

| Reader needs to… | Primary format | Essential structure |
| --- | --- | --- |
| Get oriented and inspect depth | Progressive interactive brief | Conclusion, central visual, decisive limitation, next action; optional evidence and detail |
| Understand relationships | Annotated causal or system map | Boundary, entities, labeled relationships, bottleneck, competing effects |
| Choose among options | Decision workbench | Hard constraints, feasible alternatives, comparable criteria, conditional recommendation |
| Explore changing assumptions | Simulator or calculator | Inputs, explicit model, calculated outputs, thresholds, sensitivity, limits |
| Learn and apply later | Guided visual lesson | Plain explanation, worked example, prediction, feedback, transfer problem |

Default to the brief for a complex general answer. Add another format only for a distinct user need. Do not force five formats onto every topic or describe the formats when the user actually needs the answer itself.

Read [references/format-patterns.md](references/format-patterns.md) for detailed construction, pitfalls, or a practical example in the selected format.

## Build complete knowledge in manageable layers

1. **Immediate understanding:** show the answer, one visual that makes the central relationship inspectable, the condition that could reverse the conclusion, and an action or learning objective.
2. **Working understanding:** explain in plain language, then develop a realistic example from problem and inputs through method, result, interpretation, and verification. Define necessary terms where used. Mark where an analogy stops applying.
3. **Inspection and depth:** make sources, assumptions, calculations, alternatives, edge cases, and technical detail available through optional sections or supporting artifacts. Keep consequential limitations visible in the first layer.

Use the minimum structure needed for the task. For comprehensive requests, cover each major topic with its problem, answer, explanatory visual when helpful, application, and limit; group related topics instead of generating repetitive panels. Completeness means covering the defined scope across layers. Never promise all knowledge about an unbounded subject.

## Visual and interaction choices

- Ask what specific mental operation each visual removes: comparing, tracing, sequencing, estimating, or remembering. Remove visuals without an explanatory job.
- Use shared scales for quantitative comparisons, timelines for sequence, labeled maps for relationships, and worked examples for application. Keep explanatory labels adjacent to their subjects.
- Prefer a single readable view over a sprawling graph or dashboard. Reveal subordinate detail without hiding the answer or requiring many clicks.
- If supported and useful, create a working interactive result rather than a description of one. Use an available visualization skill/tool and follow its rendering contract. This skill has no mandatory renderer dependency.
- When interaction is unavailable, produce a static diagram or concise comparison with a text equivalent. Say what is static; do not fake controls or imply working functionality.
- Use generated raster illustrations only for imagery that helps the task; prefer inspectable diagrams and plotting tools for exact labels, evidence, and calculations.
- Support keyboard use, meaningful labels, readable contrast, narrow screens, reduced motion, and text alternatives. Essential information must not depend on color, hover, or animation.
- Preserve the user's requested output medium. A request for visual explanation does not authorize building or publishing a site.

## Reliability and usefulness

- Distinguish sourced facts, user inputs, assumptions, hypotheses, calculations, and recommendations. Label invented scenarios and numbers as illustrative.
- Verify current, niche, or consequential claims with suitable authoritative sources when available. Place citations near supported claims; disclose material verification gaps.
- For decisions, apply feasibility gates before preferences. Avoid arbitrary weighted scores and fabricated precision. State what would change the recommendation.
- For models, show units, assumptions, ranges, and omitted variables. Distinguish arithmetic consequences from real-world predictions. Capacity released is not automatically cash saved; correlations and drawn arrows are not causal proof.
- For teaching, include retrieval or prediction with explanatory feedback and a changed case. Do not confuse recognition during reading with durable learning.
- For enterprise deliverables, add relevant provenance, version/date, ownership, completion criteria, reproducible calculations, and access/export requirements. Do not append irrelevant governance checklists to ordinary explanations.

## Bounded quality review

Before delivery, critically check:

- Is this the clearest useful form for this audience and task?
- What mental work is still unnecessarily left to the reader?
- Can a reader state the answer and use it without reading every detail?
- What is the strongest reasonable objection, and what evidence would reverse the conclusion?
- Does the example reach an interpreted result and a verifiable next step?
- What can be removed without losing necessary meaning?

Revise concrete weaknesses. Stop when the scoped deliverable is accurate, usable, and verified; do not loop indefinitely in pursuit of “ultimate” quality. Return the result and relevant concise rationale, not private reasoning.

For interactive outputs, check the primary interactions, calculations, initial state, edge cases, and layout when tools permit. Report material checks that could not be performed. Never claim user-tested superiority without user testing. When evaluating a format, compare it with a concise text baseline using correct task completion, errors, time to a correct answer, perceived effort, and—for teaching—delayed recall or transfer.
