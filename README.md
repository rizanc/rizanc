# Costin Rizan

Integration & platform architect · C# / .NET, APIs & applied AI · Oracle OPERA / OHIP specialist · South Jordan, UT · open to relocation

I build the APIs, integrations, and platforms that business systems run on, mostly in hospitality and casino gaming, with earlier work in telecom. Since 2019 I have been the lead engineer on two hospitality software platforms (full-time since 2022). Most of that work lives in private client repositories; what you see here is the public slice.

## What I work on

**Platform engineering.** C# / .NET 8 APIs, React / TypeScript, and SQL Server on a hospitality SaaS platform (~200K lines of .NET, ~1.1M lines of React, 650+ stored procedures), shipped with a 7-engineer team on a 2-week release train. Recent work includes the transactional core of a new online booking engine: availability search with slot ranking, hold-and-expire reservations, atomic booking with double-booking prevention, and safe cancellation.

**Oracle OPERA integration.** I write OPERA interfaces rather than install them. I wrote the first casino player-tracking ↔ OPERA PMS interface (OWS), still in production across the Las Vegas Strip and Macau, and built custom OXI/OWS integrations for MGM Resorts, Wynn, Las Vegas Sands, Hyatt, and Fairmont as an Oracle/MICROS Custom Solutions architect. Today I migrate legacy OXI/OWS interfaces to OHIP REST APIs and event streaming as properties move to OPERA Cloud.

**Production AI engineering.** I architected and run the AI program for the same platform:

- LLM features shipped inside the product's .NET 8 API (OpenAI): pull-request review, ticket enrichment, iteration summaries, release notes
- An AI review check in CI on every pull request into the main branches
- An agentic delivery pipeline on Claude Code: role-specific subagents with per-model routing, deterministic hooks that enforce TDD and code review, and MCP tool servers (read-only SQL Server schema, Playwright) over a curated context knowledge base instead of vector search
- Measured, not estimated: 70% of 3,800+ commits across 7 engineers co-authored by the pipeline, and full-stack feature cycle time down from about 6.7 to about 2.2 workdays across 714 instrumented runs

**Stack.** C# / .NET 8 · TypeScript / React / Node.js · Python · Java · Rust · SQL Server · PostgreSQL · AWS · Azure · Azure DevOps · Docker

## Public projects

| Project | What it is |
| --- | --- |
| [ohip-ows-reservation-mapper](https://github.com/rizanc/ohip-ows-reservation-mapper) | C# / .NET 8: maps a legacy OPERA OWS CreateBookingRequest (SOAP/XML) to an OHIP `POST /rsv/v1` reservation, built against Oracle's published OHIP specs |
| [llm-platform-kit](https://github.com/rizanc/llm-platform-kit) | Eval harness with an LLM-as-judge and a CI merge gate, cost-aware model router with a spend log, citation RAG with a grounding check, vector store layer |
| [codesheriff](https://github.com/rizanc/codesheriff) | AI pull-request review assistant |
| [nomadic-hub](https://github.com/rizanc/nomadic-hub) | Destination site with a Rust API and SvelteKit front end, deployed and live |

I build with AI coding agents and say so. Claude appears as a co-author on some commits here; I review and own everything that lands.

## Contact

[linkedin.com/in/costinrizan](https://www.linkedin.com/in/costinrizan) · English, French, Romanian
