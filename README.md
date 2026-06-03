# Cornerstone Smart Agent

`Smart` is a proposal-focused AI agent for Cornerstone Consulting.

It is built to turn client-facing training and consulting needs into structured deliverables using local knowledge assets, proposal patterns, reusable methods, and a PPT generation workflow.

## What Smart does

`Smart` is not a general chatbot.

Its main job is to:

- understand client needs in talent, leadership, training, workshop, and consulting scenarios
- map ambiguous requests into a clear proposal structure
- reuse Cornerstone's local knowledge base and existing proposal assets first
- generate professional draft proposals in a consulting-style format
- convert structured HTML slide drafts into `.pptx` files

## Smart-specific capabilities

Compared with a generic agent, `Smart` has a few workspace-specific strengths:

- local knowledge-first workflow based on `knowledge-base/` and `~/Desktop/Cornerstone Wiki/`
- proposal writing style aligned with Cornerstone's existing decks and consulting tone
- default structure for formal client proposals
- memory of customer names, industries, confirmed needs, common modules, and prior outputs
- HTML-to-PPT production workflow for local deliverables

More detail is documented in [SMART_CAPABILITIES.md](SMART_CAPABILITIES.md).

## Repository structure

### Agent instruction layer

- `AGENTS.md`
- `SOUL.md`
- `IDENTITY.md`
- `USER.md`
- `TOOLS.md`
- `MEMORY.md`
- `HEARTBEAT.md`

### Knowledge and reusable assets

- `knowledge-base/`
- `scripts/`

### PPT generation workflow

- `html_to_pptx.py`
- `build_ppt_from_html.sh`
- `generate_budweiser_ppt.py`
- `gen_budweiser.py`

### Operational helpers

- `reset_feishu_smart_session.sh`
- `STALE_LOCK_RUNBOOK.md`

## Typical workflow

1. Read the customer request.
2. Search the local knowledge base and reference proposals.
3. Frame the request into a proposal type such as course, bootcamp, high-potential program, or action learning project.
4. Draft a slide structure.
5. Generate HTML slide content.
6. Convert the deck to `.pptx`.
7. Store key customer information in memory for later follow-up.

## Output philosophy

`Smart` is designed to prefer:

- structured thinking over generic copy
- explicit assumptions over invented facts
- project design over course stacking
- reusable knowledge assets over one-off improvisation

## Notes

- This repo is intended to store the agent framework and reusable assets.
- Temporary files and customer-specific generated outputs are ignored by default.
