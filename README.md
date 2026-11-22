# IFRS MCP agents

Five read-only MCP servers for IFRS accounting work, sold on mcprush. Each folder is one server: `dist/server.mjs` runs over stdio with Node.js 22 or later, needs no dependencies, makes no network calls and stores nothing.

| Server | Standards | Folder |
|---|---|---|
| IFRS 16 Lease Accounting Agent | IFRS 16 | [`ifrs16-lease-agent/`](ifrs16-lease-agent/) |
| IFRS 15 Revenue Recognition Agent | IFRS 15 | [`ifrs15-revenue-agent/`](ifrs15-revenue-agent/) |
| IFRS 9 and IFRS 7 Credit Loss Agent | IFRS 9, IFRS 7 | [`ifrs9-credit-loss-agent/`](ifrs9-credit-loss-agent/) |
| IFRS 17 Insurance Contracts Agent | IFRS 17 | [`ifrs17-insurance-agent/`](ifrs17-insurance-agent/) |
| IFRS Year-End Close Agent | IAS 36, IAS 37, IAS 12, IAS 10 | [`ifrs-year-end-close-agent/`](ifrs-year-end-close-agent/) |

The code is published so mcprush can build and host it. It is licensed, not open source: see each folder's `LICENSE.md`. Install through mcprush to use it.

> FOR DEMONSTRATION AND EDUCATIONAL PURPOSES ONLY. This output is not accounting, audit, tax or legal advice, and no liability whatsoever is assumed for its results or for any decision based on them. Paragraph references point to the IFRS Accounting Standards issued by the IASB; the standards' text is not reproduced. Results depend entirely on the facts entered and must be independently verified by a qualified professional against the current authoritative text before any use.
