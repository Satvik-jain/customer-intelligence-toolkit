---
name: analyze
description: Orchestrate customer-intelligence work by routing a market, customer, product, positioning, pricing, validation, or go-to-market question to the relevant specialist skill or skills.
---

# Customer Intelligence Orchestrator

Use this skill for broad or ambiguous customer and monetization questions. Keep the work scoped: route to the smallest useful set of specialists rather than running every analysis.

## Intake

Identify:

- The decision or deliverable the user needs.
- Product/service, market, geography, lifecycle stage, and target customer.
- Available customer, usage, transaction, and external research evidence.
- Constraints such as timing, budget, privacy, and risk.

Ask a short clarifying question only when missing information would materially alter the route or conclusion. Otherwise state assumptions.

## Routing

| Request | Route |
|---|---|
| Market boundaries, competitor set, market structure, TAM/SAM/SOM | market-intelligence |
| Motivation, purchase journey, risk, emotion, social or habitual behavior | consumer-psychology |
| Customer groups, ICP, persona grounded in actual segments | segmentation |
| Synthetic personas, simulated panel, candidate objections or purchase scenarios | customer-simulation |
| Research method, experiment, usability test, causal evidence | validation |
| Problem severity, product evaluation, adoption, retention, fit signals | product-fit |
| Target, category, differentiation, value proposition, messaging | positioning |
| Price model, packaging, tiers, WTP | monetization |
| Launch, channels, sales motion, acquisition and retention economics | go-to-market |

For multi-part work, sequence specialists as needed: market and segmentation before positioning; validation before treating a claim as established; monetization and GTM after the target and value proposition are clear. Customer Simulation can generate exploratory hypotheses, but route consequential conclusions to Validation, Product Fit, or Monetization for real-evidence assessment.

## Dispatch

After choosing the route, invoke the corresponding specialist skill or skills so their workflow and limits are applied. Use the smallest useful set. For a simple request, answer directly when no specialist workflow adds value. If a specialist cannot be loaded in the current session, say so and follow only the relevant guidance available in this orchestrator; do not claim that a skill ran when it did not.

## Output contract

Return:

1. Decision and scope.
2. Recommendation or current best answer.
3. Evidence grouped with the labels in [evidence-labels.md](../../references/evidence-labels.md).
4. Assumptions, uncertainty, counterevidence, and missing inputs.
5. Next action, including a real-customer validation step when the decision depends on customer behavior.

Use the [customer research brief](../../templates/customer-research-brief.md) for plans and the [evidence ledger](../../templates/customer-evidence-ledger.md) for mixed-source conclusions.

## Guardrails

- Never fabricate citations, market statistics, customer quotes, or research results.
- Do not merge synthetic simulation with actual customer evidence.
- Do not claim PMF, demand, conversion, or actual WTP without suitable real evidence.
- If current market facts are requested but cannot be verified with available tools, state the limitation.
- Apply the shared [evidence labels](../../references/evidence-labels.md) to material claims.
