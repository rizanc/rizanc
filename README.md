# Costin Rizan

Integration architect and applied-AI engineer · South Jordan, UT · open to remote

I have spent 20+ years building the interfaces that connect mission-critical systems, mostly in hospitality and casino gaming (Oracle OPERA: OXI, OWS, OHIP), with stretches in telecom and financial services. Most of that work lives in private client repositories. What you see here is the public slice.

## What I work on

**Oracle OPERA integration.** I write OPERA interfaces rather than install them. I wrote the first casino player-tracking ↔ OPERA PMS interface (OWS), still in production across the Las Vegas Strip and Macau, and built custom OXI/OWS integrations for MGM Resorts, Wynn, Las Vegas Sands, Hyatt, and Fairmont as an Oracle/MICROS Custom Solutions architect. Today I focus on migrating legacy SOAP/XML interfaces to REST/JSON on OHIP as properties move to OPERA Cloud.

**Production LLM engineering.** Since 2026 I have architected and operated the LLM program for an enterprise hospitality SaaS platform (C# / .NET 8, React, SQL Server):

- AI features shipped inside the product API on OpenAI: pull-request review, ticket enrichment, iteration summaries, release notes
- An AI review gate in CI that runs on every pull request into the main branches
- An agentic delivery pipeline on Claude Code: role-specific subagents with per-model routing, deterministic hooks that enforce TDD and code review, and MCP tool servers (read-only SQL Server schema, Playwright) over a curated context knowledge base instead of vector search
- Measured, not estimated: 70% of 3,800+ commits across 7 engineers co-authored by the pipeline, and full-stack feature cycle time down from about 6.7 to about 2.2 workdays

**Stack.** C# / .NET 8 · TypeScript / React / Node.js · Rust · Python · SQL Server · PostgreSQL · AWS · Azure DevOps

## Public projects

| Project | What it is |
|---|---|
| [ohip-ows-reservation-mapper](https://github.com/rizanc/ohip-ows-reservation-mapper) | C# / .NET 8: maps a legacy OPERA OWS `CreateBookingRequest` (SOAP/XML) to an OHIP `POST /rsv/v1` reservation, built against Oracle's published OHIP specs |
| [llm-platform-kit](https://github.com/rizanc/llm-platform-kit) | Eval harness with an LLM-as-judge and a CI merge gate, cost-aware model router with a LiteLLM spend log, citation RAG with a grounding check, vector store layer |
| [nomadic-hub](https://github.com/rizanc/nomadic-hub) | Digital-nomad destination site: Rust API and SvelteKit front end, deployed and live |
| [codesheriff](https://github.com/rizanc/codesheriff) | AI pull-request review assistant |
| [raydium-swap-rs](https://github.com/rizanc/raydium-swap-rs) | Educational async Rust client for Raydium token swaps on Solana |

I build with AI coding agents and say so. Claude appears as a co-author on some commits here; I review and own everything that lands.

## Contact

[linkedin.com/in/costinrizan](https://linkedin.com/in/costinrizan) · English, French, Romanian
