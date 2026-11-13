---
name: customer-simulation
description: Construct clearly labeled synthetic customer personas or panels to explore product concepts, objections, and purchase scenarios. Use simulation only as exploratory model output, never as actual customer evidence.
---

# Customer Simulation

Use this skill when asked to construct synthetic personas, run a synthetic panel, explore likely objections, or simulate purchasing choices. The result is a scenario exercise, not a survey of people or a validated market model.

## Required inputs

Before simulating, identify:

- The decision the user is trying to make.
- The product, concept, price, message, or experience being evaluated.
- The target population, context, geography, and relevant alternatives.
- The available real customer or market evidence that grounds the personas.
- Any decision constraints, privacy limits, or groups requiring special care.

If a missing input could materially change the scenario, ask a focused question. Otherwise state a reasonable assumption and label it.

## Workflow

1. **Check whether simulation fits.** Prefer simulation for early exploration, structured comparisons, candidate objections, and scenario planning. Do not use it as a substitute for real research on radically novel products, sensitive populations, high-stakes decisions, or claims about actual demand.
2. **Define the population from evidence.** Use user-provided, aggregated, de-identified segment information when available. Ask the segmentation skill to define real segments if needed. If there is no grounding evidence, call the profiles illustrative archetypes and do not imply representativeness.
3. **Construct persona records.** Use the schema in [persona-schema.md](references/persona-schema.md). Separate observed traits from inferences and assumptions. Include relevant needs, situations, constraints, alternatives, and buyer/user/payer roles. Do not invent sensitive attributes or stereotyped preferences.
4. **Design a balanced scenario.** Follow [panel-protocol.md](references/panel-protocol.md). Show each persona the same concise stimulus and decision context. Include realistic alternatives and a no-purchase option. Keep individual responses separate unless group interaction is itself the scenario.
5. **Elicit decisions and objections.** Ask for a choice or no-choice response, the key condition affecting that choice, likely objections, missing information, and a generated explanation. Explore one change at a time when comparing price, features, packaging, or messaging.
6. **Check robustness and validity.** Apply [evaluation-checklist.md](references/evaluation-checklist.md). Check prompt/model sensitivity, profile diversity, internal consistency, stereotyping, and grounding. Compare against real held-out evidence if it exists; otherwise state “not externally validated.”
7. **Report only exploratory implications.** Use the [simulation report template](../../templates/simulation-report.md). Separate persona responses, cross-person patterns, model-generated rationales, and hypotheses for real research. Route actual price conclusions to Monetization and research claims to Validation.

## Required output

Include:

- A visible **[SYNTHETIC SIMULATION]** label.
- The decision question, scenario, target population, persona basis, model/setup details when known, and number of simulated profiles.
- Persona-by-persona choices and likely objections, with generated rationales clearly distinguished from observations.
- Differences, uncertainty, prompt/model sensitivity, and bias checks.
- Whether any real evidence was used for grounding or comparison.
- Specific hypotheses and an appropriate real-customer validation step.

## Evidence and safety limits

- Synthetic output remains synthetic even when conditioned on real customer data. The source dataset may be real evidence; model responses are not.
- Never write “customers said,” “X% of customers prefer,” or “market demand is…” from generated panel output. Do not present generated language as a testimonial or real quote.
- A large synthetic panel is not a large real sample. Do not claim representativeness, sampling error, statistical significance, or a real demand curve from arbitrary model-generated counts.
- Do not call a profile population-representative unless a real sampling frame and a validated calibration support that claim.
- Model-generated reasons are not proof of the causes of behavior.
- If the target is new, underrepresented, culturally specific, or poorly represented in the grounding data, lower confidence and recommend human research.
- Use the shared [evidence labels](../../references/evidence-labels.md) in all mixed-evidence reporting.

## Supporting references

- [Persona schema](references/persona-schema.md)
- [Panel protocol](references/panel-protocol.md)
- [Evaluation checklist](references/evaluation-checklist.md)
