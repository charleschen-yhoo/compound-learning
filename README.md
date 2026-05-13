# Compound Learning

A shared brain for PM teams. Experiment results, UXR findings, and data observations go in as structured artifacts. A living synthesis reconciles them, surfaces contradictions, and identifies opportunities.

## How It Works

1. **Add a learning** — provide a test result, UXR readout, data observation, or a link to one. The system normalizes it into a structured artifact.
2. **Synthesis runs automatically** — the new learning is reconciled against everything we already know. Confirmations strengthen confidence. Contradictions are surfaced with hypotheses for why.
3. **Query anytime** — read `synthesis/index.md` for the current state of knowledge, or ask questions against the corpus.

## Structure

| Path | Purpose |
|------|---------|
| `learnings/` | Individual learning artifacts (one per test/observation) |
| `synthesis/index.md` | Master synthesis — themes, key findings, contradictions, opportunities |
| `synthesis/{theme}.md` | Deep synthesis per theme |
| `manifest.md` | Audit log — what was added and what changed |

## Adding a Learning

Open Claude Code in this repo and provide your learning in any format:

- Paste raw text from an experiment readout
- Share a link to a doc or dashboard
- Describe what you observed

The system will parse it into a structured artifact, update the synthesis, and tell you what changed.

## Reading the Synthesis

Start with `synthesis/index.md` for the full picture. Each claim traces back to specific learning IDs so you can drill into the source artifact.
