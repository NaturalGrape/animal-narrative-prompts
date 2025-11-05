# Animal Narrative Prompts (Prompt Pack)

Lightweight, **prompt-only** repo for generating humorous, kind narrations for animal videos.
You can use these prompts with *any* LLM provider (OpenAI, Anthropic, etc.)—no model code included.

## What’s here
- `prompts/narrative_v1.yml` — main prompt (templated).
- `prompts/humor_strategies.md` — quick reference for humor moves.
- `prompts/style_guide.md` — keep tone consistent and safe.
- `prompts/safety_policy.md` — guardrails to avoid harmful content.
- `examples/` — how to fill inputs and call an LLM.

## How to use
1. Prepare a **request object** like `examples/example_request.json`.
2. Load `prompts/narrative_v1.yml` and substitute the fields.
3. Send the resulting prompt string to your LLM of choice.

## Versioning prompts
- Duplicate `narrative_v1.yml` → `narrative_v2.yml` when you change logic.
- Add a short note to the top of each file describing the changes.
- Use Git tags for milestones:
  ```bash
  git tag -a v0.1 -m "First public prompt"
  git push --tags
