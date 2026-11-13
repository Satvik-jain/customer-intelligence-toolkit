# Synthetic persona schema

Create each persona as a structured scenario profile, not as a claim that a real person exists.

| Field | Include when relevant | Provenance |
|---|---|---|
| Persona ID | Neutral identifier such as P01; avoid realistic names unless clearly fictional and needed for readability. | Synthetic label |
| Segment and role | Segment basis; distinguish user, buyer, payer, approver, and influencer. | Observed / inferred / assumed |
| Situation and job | Trigger, context, task, desired progress, and outcome. | Observed / inferred / assumed |
| Behaviors and alternatives | Current workaround, usage pattern, switching constraints, and competitors considered. | Observed / inferred / assumed |
| Goals and trade-offs | Functional, economic, emotional, or social priorities relevant to the scenario. | Observed / inferred / assumed |
| Constraints | Budget, time, access, skills, policy, or other decision limits. | Observed / inferred / assumed |
| Uncertainty | Missing or weakly supported fields and plausible alternatives. | Explicit unknowns |

## Construction rules

- Ground profiles in de-identified, aggregated customer evidence or a defined real segment when available.
- Preserve evidence provenance per field. A model-generated trait is not an observed trait.
- Do not make demographic details do explanatory work unless relevant evidence supports the connection.
- Avoid sensitive attributes and stereotypes. If subgroup analysis is necessary, base it on an appropriate, ethical, and lawful research design.
- Include heterogeneity and plausible counterexamples; do not make every persona articulate, consistent, or enthusiastic.
- If no population or customer data is available, label the entire set “illustrative assumptions, not representative.”

## Source note

This schema is a project-authored prompt structure, not a validated persona model. Evidence on persona-conditioned synthetic respondents is mixed and domain-specific; see [verified source notes](../../../references/sources.md#synthetic-customer-simulation-and-evidence-limits).
