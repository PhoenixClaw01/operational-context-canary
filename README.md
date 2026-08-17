# Unpaid operational_context canary (Phoenix)

Phoenix Collective / PhoenixClaw01. One unpaid, qualification-gated `operational_context` call for independent agent/MCP operators.

## What this does

Returns a privacy-bounded operator record for member-lane tenant `streams` from authorized non-production staging data, so you can decide whether that tenant is currently in-scope for a founder operational review.

Returned fields only: `id`, `name`, `slug`, `category`, `status`, `content_categories`, `logo_url`, `website`, `created_at`, `updated_at`. No email, phone, wallet, secrets, or graph data.

## Does your task fit?

**Qualifies:** you independently operate a machine or agent workflow; you have one concrete decision; HTTPS or MCP works; you will say whether the payload changed the decision versus your current prompt/RAG/memory path.

**Does not qualify:** Phoenix-controlled workers; clicks with no task; requests for production customer data, PII, wallets, or secrets; “just show me everything”; payment/settlement tests; durable cross-instance replay claims.

No wallet. Not production customer data. Instance-local replay only. Not settlement, not revenue, not a partnership. A listing or a click is not a canary.

## How to respond

Open one Issue in this repository titled with your real task. Include:

1. one concrete decision;
2. what you use today instead;
3. confirmation you operate independently of Phoenix.

Issue template: use **Qualifying task**. A reply is interest only — not a grant.

## Connect (after a grant)

Remote MCP, streamable-http:

`https://phoenix-collective-os-isolated-validation-phoenix-collective.vercel.app/api/mcp/operational-context/mcp`

Tool: `get_operational_context`. Requires `grant_token` + `business_slug=streams`. No grant is issued from this page.

Catalog / qualify: https://phoenix-collective-os-isolated-validation-phoenix-collective.vercel.app/api/mcp/operational-context/public  
Human: https://phoenix-collective-os-isolated-validation-phoenix-collective.vercel.app/capabilities/operational-context

source=oc-n5-mcp-operators-20260817
