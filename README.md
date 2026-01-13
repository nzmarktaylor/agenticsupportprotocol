# Agentic Support Protocol (ASP)

The **Agentic Support Protocol (ASP)** is an open, domain‑specific protocol designed to enable
AI agents to collaborate, escalate, and resolve IT support issues across heterogeneous
helpdesk platforms.

ASP defines a universal language for support operations — including incidents, requests,
problems, changes, CMDB interactions, diagnostics, and multi‑tier escalation — allowing
agents to work together regardless of the underlying ITSM system.

## Why ASP?

Modern support environments are fragmented. ServiceNow, Jira Service Management, BMC,
Freshservice, Zendesk, and countless custom systems all expose different APIs, workflows,
and data models. This makes it difficult for autonomous agents to collaborate or perform
consistent support actions.

ASP solves this by providing:

- A **unified schema** for ITSM objects (incidents, requests, problems, changes, KB, CMDB)
- A **standard set of verbs** for support actions (triage, escalate, diagnose, remediate)
- A **collaboration model** for multi‑agent support workflows
- A **transport layer inspired by the Model Context Protocol (MCP)**, leveraging proven
  patterns such as structured messages and server‑sent events
- A **connector architecture** that enables interoperability with any helpdesk system

## Relationship to MCP

ASP is not a fork or extension of the Model Context Protocol. Instead, it draws on MCP’s
well‑established transport patterns — such as SSE‑based streaming, structured envelopes,
and session semantics — while defining its own domain‑specific protocol layer tailored
for IT support.

MCP provides a strong foundation for agent communication. ASP builds on that foundation
to define the semantics, workflows, and safety rules required for enterprise‑grade
support operations.

## Goals

- Enable AI agents to perform support tasks safely and consistently
- Standardize cross‑desk collaboration and escalation
- Provide a vendor‑neutral abstraction over ITSM systems
- Support human‑in‑the‑loop workflows and auditability
- Encourage an open ecosystem of connectors and agent implementations

## License

ASP is released under the **MIT License**, encouraging broad adoption, modification, and
commercial use. Portions of the transport layer may incorporate or adapt MIT‑licensed
components from the Model Context Protocol, with attribution preserved.

## Status

This project is in early development. The initial focus is on:

- Defining the core schemas
- Establishing the message envelope format
- Drafting the support verbs
- Building the first reference connector
- Creating a minimal reference agent

Contributions, discussions, and proposals are welcome.
