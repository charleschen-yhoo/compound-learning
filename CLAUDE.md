# Compound Learning System

A shared brain for PM teams. Learnings go in, compounded insight comes out.

## Architecture

```
/learnings/       Individual learning artifacts (one per test/observation)
/synthesis/
  index.md        Master synthesis — themes, contradictions, opportunities
  {theme}.md      Per-theme deep synthesis (created as themes emerge)
/manifest.md      Audit log of what was added and what changed
```

## Atlassian Connection

- Cloud ID: `c07c0d37-d9c1-4795-8f63-ab7d6bcf3d2a`
- Site: `ouryahoo.atlassian.net`
- Use this cloud ID for all Jira and Confluence API calls.

## Adding a New Learning

When a user provides a new learning (raw text, a link to a readout, or a structured entry):

1. **Parse** the input into a structured artifact using the template in `learnings/TEMPLATE.md`. Assign the next sequential ID. Save as `learnings/{id}-{slug}.md`.

2. **Update the manifest** — add a row to `manifest.md` with the ID, title, date, themes, and a brief note on what changed in the synthesis.

3. **Run synthesis** — this is the core step:
   - Read `synthesis/index.md` and any relevant `synthesis/{theme}.md` files
   - Read ALL existing learning artifacts in `learnings/` (excluding TEMPLATE.md)
   - Reconcile the new learning against the full corpus:
     - Does it **confirm** an existing finding? Strengthen the confidence.
     - Does it **contradict** an existing finding? Surface the contradiction with a hypothesis for WHY (different segment? timing? surface? methodology?)
     - Does it **open a new theme**? Create a new theme section.
   - Resynthesize opportunity areas based on the updated corpus
   - Update `synthesis/index.md` with the new state
   - Create or update `synthesis/{theme}.md` files as needed

4. **Report** what changed — tell the user what was added, what it confirmed/contradicted, and any new opportunities identified.

## Ingesting from JIRA

When a user provides JIRA ticket IDs or a JQL query:

### Single ticket or list of tickets
1. Fetch each ticket using `getJiraIssue` with the cloud ID above. Request `responseContentFormat: "markdown"` and fields: `["summary", "description", "comment", "labels", "status", "created"]`.
2. Extract the learning from the ticket — the hypothesis, what was tested, the outcome, and any nuance. Pull from both the description and comments, as results are often posted in comments.
3. Parse into a structured artifact per the standard flow above.
4. Include the JIRA ticket key in the artifact's `source` field (e.g., `source: "PROJ-123"`).

### JQL bulk ingest
1. Run the JQL query using `searchJiraIssuesUsingJql` with `maxResults: 100`.
2. For each result, fetch the full ticket to get comments.
3. Parse ALL tickets into artifacts first — do NOT run synthesis between each one.
4. Run synthesis once at the end against the full new batch.
5. Update the manifest with all new entries.
6. Report a summary: how many learnings added, what themes emerged, key contradictions.

### What to extract from a JIRA ticket
- **Title/Summary** → artifact title
- **Description** → hypothesis, test design
- **Comments** → often contain results, data, and nuance — read all comments
- **Labels** → can inform theme tags
- If a ticket doesn't contain a clear learning (e.g., it's a task or bug), skip it and tell the user.

## Ingesting from Decks / PDFs

When a user provides a PDF, deck export, or pasted slide content:

1. Read the content and identify distinct learnings — a single deck may contain multiple.
2. Each distinct learning becomes its own artifact.
3. Set `source` to the filename or link.
4. Follow the standard parse → manifest → synthesis flow.
5. For bulk (multiple learnings from one source), parse all first, synthesize once.

## Synthesis Principles

- Every claim in the synthesis must trace back to specific learning IDs
- Contradictions are features, not bugs — surface them prominently with hypotheses
- Confidence levels compound: multiple independent learnings confirming the same thing = high confidence
- Opportunity areas should be specific and actionable, not vague ("users struggle with X" not "improve UX")
- The synthesis should be useful to someone who has never read any individual artifact
- Keep synthesis concise — a PM should be able to read index.md in under 5 minutes

## Querying the System

When a user asks a question against the learnings (e.g., "what do we know about onboarding?", "should we try X?"):

- Reference specific learnings by ID
- Flag confidence levels
- Call out what we DON'T know (gaps in the corpus)
- If the question touches a contradiction, present both sides

## Theme File Structure

Each `synthesis/{theme}.md` should contain:
- Summary of what we know (with learning IDs)
- Confidence-ranked findings
- Contradictions within this theme
- Open questions
- Opportunity areas specific to this theme
