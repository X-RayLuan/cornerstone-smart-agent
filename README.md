# Cornerstone Smart Agent

`Smart` is a proposal-focused agent for Cornerstone Consulting.

It is designed to turn client training and consulting needs into structured deliverables using local knowledge assets, proposal patterns, and a PPT generation workflow.

## What this repo contains

- Agent identity and working instructions
- Cornerstone proposal knowledge base
- PPT generation helpers
- Reusable scripts for proposal production

## Core capabilities

- Read local `knowledge-base/` and Cornerstone source materials first
- Convert fuzzy client requests into structured proposal logic
- Follow a consulting-style proposal structure instead of generic AI copy
- Produce HTML-based slide drafts and convert them to `.pptx`
- Preserve memory about customers, needs, modules, and prior outputs

## Main files

- `AGENTS.md`
- `SOUL.md`
- `IDENTITY.md`
- `USER.md`
- `TOOLS.md`
- `MEMORY.md`
- `knowledge-base/`
- `html_to_pptx.py`
- `build_ppt_from_html.sh`
- `scripts/`

## Notes

- This repo is intended to store the agent framework and reusable assets.
- Temporary files and customer-specific generated outputs are ignored by default.
