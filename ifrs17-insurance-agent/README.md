# IFRS 17 Insurance Contracts Agent

Scope and model choice, level of aggregation, GMM initial measurement, CSM roll-forward, PAA, reinsurance held and transition.

> FOR DEMONSTRATION AND EDUCATIONAL PURPOSES ONLY. This output is not accounting, audit, tax or legal advice, and no liability whatsoever is assumed for its results or for any decision based on them. Paragraph references point to the IFRS Accounting Standards issued by the IASB; the standards' text is not reproduced. Results depend entirely on the facts entered and must be independently verified by a qualified professional against the current authoritative text before any use.

**Standards:** IFRS 17 Insurance Contracts
**Tools:** 9 calculators, checklists and lookups, plus `agent_about`
**For:** Insurers' actuaries and finance teams, insurance auditors and consultants.

## What it does

- Choose GMM, PAA or VFA and set the level of aggregation
- Measure fulfilment cash flows and the CSM at initial recognition
- Roll the CSM forward and release it on coverage units
- Measure PAA liabilities and reinsurance held, with loss-recovery
- Apply the fair value transition approach and run the disclosure checklist

Every result cites the IFRS paragraphs it relies on. The standards' text is paraphrased, never reproduced.

## Install

With the mcprush CLI (after buying the listing):

```bash
npx mcprush add <publisher>/ifrs17-insurance-agent
```

Or point any MCP client at the bundled server (Node.js 22+, no dependencies, no network, no API keys):

```json
{ "mcpServers": { "ifrs17-insurance-agent": { "command": "node", "args": ["<path>/ifrs17-insurance-agent/dist/server.mjs"] } } }
```


## Try it

> Premiums of 1,000 now, claims PV 700, expenses PV 100, risk adjustment 50. Measure the CSM at initial recognition and roll it forward over 5 equal coverage periods.

## Tools

| Tool | What it does |
|---|---|
| `ifrs17_scope_and_model` | Scope & measurement model (3-8, 53, B101) |
| `ifrs17_level_of_aggregation` | Level of aggregation (14-24) |
| `ifrs17_gmm_initial_measurement` | GMM initial measurement: FCF & CSM (32-38, 47) |
| `ifrs17_csm_rollforward` | CSM roll-forward & insurance revenue (44, B119-B124) |
| `ifrs17_paa_measurement` | Premium allocation approach (53-59) |
| `ifrs17_reinsurance_held` | Reinsurance contracts held (60-70A) |
| `ifrs17_disclosure_checklist` | Disclosure checklist (93-132) |
| `ifrs17_lookup` | Paragraph & topic lookup |
| `ifrs17_transition_fair_value` | Fair value approach on transition: CSM or loss component (C20-C24) |

## Sample output (`ifrs17_scope_and_model`, built-in example)

Unit-linked savings with death benefit: VFA.

## Privacy and safety

- Runs locally over stdio. No network calls, no telemetry, no files written.
- Every tool is read-only, idempotent and closed-world (MCP annotations declared).
- No personal data is collected.

Demo and educational use only. No liability assumed for results. Not professional advice.
