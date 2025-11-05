# Animal Narrative Prompts (Prompt Pack)

Lightweight, **prompt-only** repo for generating humorous narrations for animal videos.
You can use these prompts with *any* LLM provider (OpenAI, Anthropic, etc.) no model code included.

## What’s here
- `prompts/prompt_1` — used to analyze the objective contents and actions in a video.
- `prompts/prompt_2a` — prompt used to generate narrative (gives more flamboyant results).
- `prompts/prompt_2b` — more grounded consistent tone.
- `prompts/prompt_3` — turns the narrative into dialogue and captions.

## How to use
1. Prepare a **request object** like `examples/example_request.json`.
2. Load the different files in `prompts` and substitute the fields.
3. Send the resulting prompt string to your LLM of choice.
4. Use a voiceover AI (eleven labs) to turn into audio

## Versioning prompts
- Add a short note to the top of each file describing the changes.
- Use Git tags for milestones:
  ```bash
  git tag -a v0.1 -m "First public prompt"
  git push --tags
