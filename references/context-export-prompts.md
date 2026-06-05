# Context Export Prompts

Use these prompts during Press Start Phase 2. Paste the relevant prompt directly into the chat for the user to copy. Do not tell the user to open this reference file.

For beginner users, wrap each prompt with plain instructions:

```text
Open ChatGPT, paste the prompt below, then read ChatGPT's answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Adjust the tool name as needed. If the user has multiple tools, give one prompt at a time so the process stays easy.

Always explain:

```text
This answer becomes source material for your LLM Wiki. It is the draft source of truth the wiki will use to customize future help, so please correct it before sending it back.
```

## ChatGPT

Tell the user:

```text
Open ChatGPT, paste the prompt below, then read ChatGPT's answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Then give:

```markdown
I am setting up a Karpathy-style LLM Wiki so future AI assistants can understand me or my work better.

Based on our past conversations and anything you can infer from this chat history, summarize durable context that would be useful to preserve.

Include:
- who I am and what I do
- current goals, projects, responsibilities, and open loops
- recurring preferences, constraints, habits, and work style
- people, organizations, products, tools, and places I mention often
- decisions I have made and the rationale if known
- things I repeatedly ask for help with
- my writing and communication style
- anything that seems uncertain, outdated, or contradicted by newer context

Do not include passwords, API keys, account numbers, private addresses, or unnecessary sensitive details.
Mark uncertainty clearly.
Format the result in markdown with headings and bullets.
```

## Claude

Tell the user:

```text
Open Claude, paste the prompt below, then read Claude's answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Then give:

```markdown
I am setting up a Karpathy-style LLM Wiki so future AI assistants can start with durable context instead of making me re-explain everything.

Please summarize what you know from our conversations that would be useful for an AI-maintained wiki.

Focus on:
- my background, work, and current season
- active projects and priorities
- goals, constraints, preferences, and recurring patterns
- people, organizations, tools, and projects that matter
- decisions and tradeoffs already made
- topics I often return to
- how I like help, feedback, and writing to sound
- anything you are unsure about or that may be stale

Avoid secrets, credentials, account details, and overly sensitive specifics.
If something is sensitive but useful, summarize it abstractly.
Return clean markdown that can be saved as a raw source.
```

## Gemini

Tell the user:

```text
Open Gemini, paste the prompt below, then read Gemini's answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Then give:

```markdown
I am creating a Karpathy-style LLM Wiki: raw sources go in, and an AI maintains synthesized markdown pages over time.

From our conversations, extract durable context that future AI agents should know.

Include:
- identity/background
- active goals and projects
- responsibilities and routines
- preferences and constraints
- important people, organizations, tools, and places
- decisions and rationale
- repeated requests or recurring problems
- communication style
- unclear, outdated, or low-confidence claims

Do not include secrets, credentials, private account details, or unnecessary sensitive information.
Use markdown.
```

## Perplexity

Tell the user:

```text
Open Perplexity, paste the prompt below, then read Perplexity's answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Then give:

```markdown
I am setting up a Karpathy-style LLM Wiki. Please summarize any durable context from this thread or workspace that would help future AI assistants.

Separate:
- confirmed facts
- inferred but uncertain context
- active projects or questions
- useful sources or links mentioned
- follow-up questions I should answer before this becomes wiki knowledge

Do not include secrets or sensitive account details.
Use markdown.
```

## Cursor, Codex, Claude Code, or Other Coding Agents

Tell the user:

```text
Open the coding agent in the repo you want included, paste the prompt below, then read the answer carefully. Correct anything wrong, outdated, too private, or missing. Then paste the corrected answer back here.
```

Then give:

```markdown
I am setting up a Karpathy-style LLM Wiki for this repo or workspace.

Please inspect the repo and summarize durable context that should become initial wiki knowledge.

Include:
- what this repo/project is for
- architecture and important folders
- setup, test, build, and deploy commands
- current known issues, TODOs, and risks
- important decisions already encoded in the codebase
- project-specific terminology
- external services, dependencies, and integrations
- what future agents should read first
- unclear or missing context that needs follow-up questions

Do not expose secrets or credentials. If sensitive config exists, describe only the shape and where safe examples live.
Return markdown suitable to save in raw/.
```

## Notion, Google Docs, Obsidian, or Existing Notes

Ask the user to export or copy:

- personal operating docs
- project pages
- planning docs
- goals lists
- meeting notes
- decision notes
- research notes
- README-like overview docs
- bios, resumes, or about pages

If the tool supports markdown export, prefer markdown. Otherwise, pasted text is fine.

## Data safety reminder

Before asking the user to paste or export content, say:

```text
Only include information you are comfortable storing in local markdown files. Do not include passwords, API keys, bank details, private addresses, or sensitive records. If something is useful but sensitive, summarize it abstractly instead.
```
