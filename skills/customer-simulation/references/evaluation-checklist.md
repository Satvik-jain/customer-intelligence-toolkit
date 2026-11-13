# Simulation evaluation checklist

Separate these evaluation questions; a pass on one does not imply a pass on the others.

| Dimension | Question |
|---|---|
| Grounding | Do persona fields trace to data, theory, or explicit assumptions? |
| Task fit | Does the simulation address the intended scenario and decision? |
| Persona sensitivity | Do meaningfully different profiles respond differently for relevant reasons? |
| Internal consistency | Are repeated responses reasonably stable under unchanged conditions? |
| Robustness | Do useful conclusions persist across reasonable prompt variants or model versions? |
| External validity | Does output align with held-out human or behavioral evidence for this population and task? |
| Coverage and fairness | Are important groups or viewpoints missing, distorted, or stereotyped? |
| Decision utility | Does the simulation produce a useful hypothesis or test plan without overstating certainty? |

## Interpretation

- Consistency measures repeatability; it does not prove accuracy.
- Distribution similarity or choice accuracy is specific to the benchmark, task, population, and model setup.
- Comparing with the same data used to construct personas is not an independent validation. Prefer held-out evidence when available.
- If no human benchmark exists, report external validity as untested.
- Model-generated sample size does not establish precision about real people.

## Source note

The checklist is a project-authored evaluation aid. The cited simulation and synthetic-survey studies are task- and population-specific; some are preprints. They motivate testing persona adherence, subgroup fidelity, and external validity but do not validate every simulator or use case. See [verified source notes](../../../references/sources.md#synthetic-customer-simulation-and-evidence-limits).
