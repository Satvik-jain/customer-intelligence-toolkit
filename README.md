# Customer Intelligence & Monetization Toolkit

**Evidence-aware customer research and growth workflows for Claude Code.**

Turn customer questions into structured research plans, product decisions, positioning, pricing, and go-to-market strategy. The plugin includes one orchestrator and nine focused specialist skills.

## What you can do

- Map a market, competitors, customer needs, and useful segments.
- Explore product concepts and likely objections with clearly labeled synthetic personas.
- Plan customer interviews, usability studies, surveys, and experiments.
- Evaluate product fit, positioning, monetization, and launch options.
- Keep assumptions, external research, real customer evidence, and simulation results distinct.

## Specialist skills

| Skill | Focus |
|---|---|
| **Customer Simulation** | Synthetic personas, panels, product reactions, and objections |
| **Consumer Psychology** | Decision context, motivation, risk, emotion, and social influence |
| **Segmentation** | Customer segments, personas, and B2B ideal customer profiles |
| **Validation** | Research methods, usability studies, and experiments |
| **Product Fit** | Problem severity, solution value, adoption, and retention |
| **Market Intelligence** | Market boundaries, competitors, and market sizing |
| **Positioning** | Target, category, differentiated value, and messaging |
| **Monetization** | Pricing models, tiers, and willingness-to-pay research |
| **Go-to-Market** | Beachhead, channels, sales motions, and launch planning |

## Install

Install the plugin from this GitHub repository inside Claude Code:

~~~text
/plugin marketplace add Satvik-jain/customer-intelligence-toolkit
/plugin install customer-intelligence-toolkit@customer-intelligence-toolkit
~~~

For a fork, replace the owner and repository with your GitHub path.

## Quick usage

Start with the orchestrator for a cross-functional question:

~~~text
/customer-intelligence-toolkit:analyze Help me choose a first segment and decide what to validate before launch.
~~~

Use a specialist directly when you know the task:

~~~text
/customer-intelligence-toolkit:customer-simulation Explore possible objections to this concept. Keep every response labeled synthetic.
/customer-intelligence-toolkit:validation Design a real customer test for this purchase hypothesis.
/customer-intelligence-toolkit:monetization Compare pricing models and propose a way to test them.
~~~

## How it works

The orchestrator routes each request to the smallest useful set of specialist workflows. Those workflows provide structured questions, decision steps, and output templates. The plugin does not connect to customer databases or conduct research by itself; it works with the context and tools available in your Claude Code session.

## Evidence and limitations

The toolkit distinguishes **real customer evidence**, **external research**, **synthetic simulation**, **assumptions**, and **inferences**. AI-generated customer responses are not real customer statements and cannot establish market demand, product-market fit, conversion, or actual willingness to pay. Use simulation to explore hypotheses, then validate important decisions with people or observed behavior.

## Privacy

The plugin itself does not independently collect or transmit data and has no backend or external data-transmission integrations. See the [Privacy Policy](PRIVACY.md) for details about Claude and any external services you connect.

## Contributing and license

Contributions are welcome. Please include traceable sources for research claims, avoid unsupported numerical claims, and never submit private customer data or the local research reports.

This project is licensed under the [MIT License](LICENSE).

## Development and testing

From the repository root, load the local plugin for a development session and validate its manifests:

~~~sh
claude --plugin-dir .
claude plugin validate .
~~~

The research/ directory contains private local development material and is ignored by Git.
