# Salesforce AI Hub — Project Instructions

## Context and scope

This project is an internal MVP named **AI Hub** for a Salesforce Enterprise Edition sandbox. It centralizes AI-related news, Salesforce AI and Agentforce updates, AI and agentic tools, articles, videos, links, ideas, POCs, presentations, and files.

Work only on the feature or phase requested. Do not implement future phases without explicit approval, and do not modify unrelated files.

## Technology and architecture

- Use Salesforce Lightning Experience, Salesforce DX, Lightning Web Components (LWC), custom objects, Salesforce Files, permission sets, and a Lightning app as appropriate.
- Prefer native declarative Salesforce capabilities when they meet the requirement.
- Use LWC for custom AI Hub Home experiences. Keep components small, focused, and reusable.
- Do not use Aura components.
- Add Apex only when it provides a real technical benefit. Bulkify Apex, avoid SOQL in loops, and enforce CRUD and field-level security (FLS) whenever accessing data.
- Separate responsibilities clearly and follow Salesforce development best practices.
- Do not add external dependencies without a clear need.

## Implementation workflow

Before making changes:

1. Inspect the project structure and relevant existing metadata, code, tests, and documentation.
2. Identify existing patterns and functionality that can be reused.
3. Briefly explain the implementation plan before editing.

After making changes:

1. Review every modified file.
2. Check Salesforce metadata structure, imports, API names, and references affected by the change.
3. Run the smallest applicable validation; use the project scripts where relevant (`npm run lint`, `npm run test:unit`, and `npm run prettier:verify`).
4. Report files created or changed, validation results, and any manual Salesforce setup or deployment steps.
5. Do not report the task as complete while a known error remains.

## Salesforce-specific guidance

- Keep metadata in the Salesforce DX package directory, `force-app/`.
- Use `sf` CLI commands for Salesforce org and metadata workflows when needed; do not assume an org is authorized or deploy without the task requiring it.
- Use Salesforce Files for document storage rather than introducing a separate storage mechanism.
- Grant access through permission sets where appropriate.
