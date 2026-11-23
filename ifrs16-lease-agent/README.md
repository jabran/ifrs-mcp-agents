# IFRS 16 Lease Accounting Agent

[![IFRS 16 Lease Accounting Agent MCP server](https://mcprush.com/badge/ifrs-16-lease-accounting-agent-mcp/card.svg)](https://mcprush.com/to/ifrs-16-lease-accounting-agent-mcp?ref=badge)

Lease identification, lessee schedules, modifications, lessor, sale and leaseback and disclosures, with paragraph citations.

> FOR DEMONSTRATION AND EDUCATIONAL PURPOSES ONLY. This output is not accounting, audit, tax or legal advice, and no liability whatsoever is assumed for its results or for any decision based on them. Paragraph references point to the IFRS Accounting Standards issued by the IASB; the standards' text is not reproduced. Results depend entirely on the facts entered and must be independently verified by a qualified professional against the current authoritative text before any use.

**Standards:** IFRS 16 Leases
**Tools:** 9 calculators, checklists and lookups, plus `agent_about`
**For:** Corporate accountants, controllers and audit teams handling property, vehicle and equipment leases.

## What it does

- Decide whether a contract contains a lease
- Build the lease liability and right-of-use asset schedule with journals
- Remeasure for reassessments and modifications
- Account for subleases, sale and leaseback and transition
- Produce the IFRS 16 disclosure checklist

Every result cites the IFRS paragraphs it relies on. The standards' text is paraphrased, never reproduced.

## Install

With the mcprush CLI (after buying the listing):

```bash
npx mcprush add <publisher>/ifrs16-lease-agent
```

Or point any MCP client at the bundled server (Node.js 22+, no dependencies, no network, no API keys):

```json
{ "mcpServers": { "ifrs16-lease-agent": { "command": "node", "args": ["<path>/ifrs16-lease-agent/dist/server.mjs"] } } }
```


## Try it

> We lease an office for 5 years at 120,000 a year paid in arrears, incremental borrowing rate 6%. Build the IFRS 16 schedule and journals.

## Tools

| Tool | What it does |
|---|---|
| `ifrs16_lease_identification` | Is it a lease? Exemptions (5-11, B9-B31) |
| `ifrs16_lessee_measurement` | Lessee: lease liability, ROU asset & schedule (22-38) |
| `ifrs16_remeasurement_and_modification` | Lessee: reassessment & modifications (39-46) |
| `ifrs16_lessor` | Lessor: classification & accounting (61-88) |
| `ifrs16_sale_and_leaseback` | Sale and leaseback: seller-lessee (98-103) |
| `ifrs16_disclosure_checklist` | Disclosure checklist (51-60, 89-97) |
| `ifrs16_lookup` | Paragraph & topic lookup |
| `ifrs16_transition` | Lessee transition: modified retrospective options (C5-C10) |
| `ifrs16_sublease` | Sublease classification and intermediate lessor accounting (B58, 68) |

## Sample output (`ifrs16_lease_identification`, built-in example)

Dedicated rail cars for 5 years: lease.

## Privacy and safety

- Runs locally over stdio. No network calls, no telemetry, no files written.
- Every tool is read-only, idempotent and closed-world (MCP annotations declared).
- No personal data is collected.

Demo and educational use only. No liability assumed for results. Not professional advice.
