---
name: press-start
description: Guided first-run onboarding for Karpathy-style LLM Wiki, especially for complete beginners moving from ChatGPT or Claude web chat to Codex, Claude Code, or another file-working agent. Use when a user wants to install or bootstrap Andrej Karpathy's LLM Wiki pattern, collect existing AI context and documents, verify what is accurate, ask targeted follow-up questions, and create the initial raw and wiki structure without changing the LLM Wiki architecture.
metadata:
  short-description: Guided setup for Karpathy-style LLM Wiki
---

# Press Start

Press Start is a guided setup layer for Andrej Karpathy's LLM Wiki pattern.

The canonical LLM Wiki source is:
https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f

Do not reinvent, replace, rename, or redesign the LLM Wiki architecture. First help the user install or apply the canonical LLM Wiki pattern, then guide them through collecting context, confirming it, filling gaps, and bootstrapping the initial wiki.

## Operating stance

- Treat Karpathy's LLM Wiki as the backbone.
- Treat Press Start as a one-time setup assistant, not an ongoing workflow skill.
- Preserve the raw-to-wiki model: raw sources are immutable inputs; wiki pages are synthesized, maintained knowledge.
- Assume the user is a complete beginner unless they clearly show otherwise.
- Keep the setup accessible for people who only know ChatGPT or Claude in a web browser.
- Explain every unfamiliar word before using it repeatedly: folder, file, local, terminal, command, repo, markdown, raw, wiki, Codex, Claude Code.
- Use plain language first, then the technical term in parentheses when helpful.
- Give one action at a time for installation and setup. Do not hand beginners a long wall of terminal commands.
- Ask for messy context first; organize it after.
- Do not ask for secrets, passwords, API keys, full addresses, account numbers, or sensitive records.
- Before writing sensitive personal details, ask whether the user wants full detail, a private abstraction, or exclusion.
- Confirm uncertain, stale, or conflicting claims before turning them into durable wiki pages.

## Phase 0: Explain what is happening

Start with a short, calming explanation. Do not begin with commands.

Use wording like:

```text
You do not need to understand how AI works to do this.

ChatGPT or Claude in the browser is mostly a chat window. The assistant you are using now can work with files on your computer. That matters because an LLM Wiki is just a folder of text files that the assistant can read and update over time.

We are going to:
1. Make one AI memory folder.
2. Set up the proven Karpathy LLM Wiki structure inside it.
3. Collect context you already have from ChatGPT, Claude, documents, and notes.
4. Ask only the missing questions.
5. Turn it into a useful starter wiki.

I will go one step at a time.
```

Do not ask the user to choose between Codex and Claude Code. If Press Start is running, the user has already chosen an agent environment. The relevant question is where the wiki folder should live.

If the user asks how to install Codex or Claude Code, then point them to official docs. Otherwise, do not make tool installation part of the active setup.

## Phase 1: Install the LLM Wiki foundation

Start here every time unless the current repo already has a working LLM Wiki.

1. Explain that the LLM Wiki needs its own folder on the user's computer:

```text
We need to make one folder for your LLM Wiki. Think of this as your AI memory folder. It will hold the original material you give the assistant and the cleaner wiki pages the assistant creates from it.
```

Then ask where to create it:

```text
Where do you want this folder to live?

If you are not sure, I recommend your Desktop because it is easy to find. We can make a folder there called `llm-wiki`.
```

Do not choose a location without the user's answer. If they are unsure, suggest:

```text
Desktop -> llm-wiki
```

2. Direct them to the canonical LLM Wiki idea file:
   https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
3. Explain that this link is the original idea and pattern Press Start is using. The user does not need to understand the whole document before continuing.
4. Read the gist if network access is available; otherwise tell the user to open the link and paste the relevant setup instructions.
5. Apply the Karpathy-style structure and instructions in the target folder. If the user already has an LLM Wiki setup they prefer, use that exact setup and do not replace it.
6. Create or verify the standard structure:

```text
raw/
wiki/
  index.md
  log.md
  entities/
  concepts/
  decisions/
  sources/
  syntheses/
  projects/
```

Explain the structure in beginner language:

```text
`raw/` is the inbox. We put original notes, exports, and documents there.
`wiki/` is the clean organized memory. The agent writes and updates those pages.
`index.md` is the map.
`log.md` is the history of what changed.
```

7. Create or update the repo's agent instructions only as needed so future agents understand the LLM Wiki workflow. Use the host agent's convention when obvious, such as `AGENTS.md` for Codex or `CLAUDE.md` for Claude Code.

If the user says they have already installed LLM Wiki, verify the folder structure and instructions before continuing.

## Phase 2: Collect existing context

Before interviewing the user, help them gather context they already have.

Ask which AI tools or document systems they use. If they use ChatGPT, Claude, Gemini, Perplexity, Cursor, Codex, Claude Code, Notion, Google Docs, Obsidian, or similar tools, load `references/context-export-prompts.md` and paste the relevant export prompts directly into the chat for the user to copy. Do not make non-technical users hunt through files or understand the skill internals.

For beginner users, give simple instructions:

1. Open the AI tool or document app you already use.
2. Copy the prompt I give you.
3. Paste it there.
4. Copy the answer it gives you.
5. Read the answer and correct anything wrong, outdated, too private, or missing.
6. Paste the corrected answer back here.

Explain why this matters:

```text
This export is the starting source of truth for your wiki. It is not automatically correct just because an AI wrote it. Please read it over and fix anything wrong, outdated, too private, or incomplete.

The LLM Wiki will use this source material to create the memory pages that future assistants read before helping you. Better source material means better, more personal answers later.
```

If the user has multiple tools, handle one tool at a time.

Tell the user they can provide context in any mix of:

- pasted AI summaries
- exported chat summaries
- resumes, bios, or about pages
- project docs, READMEs, specs, meeting notes, tickets, or plans
- goals lists, planning docs, journals, or personal operating docs
- company docs, process docs, CRM notes, or research notes
- links, copied text, markdown files, PDFs, documents, spreadsheets, screenshots, or folders

Explain that messy dumps are welcome. The agent's job is to sort, not to make the user pre-organize.

## Phase 3: Analyze before asking

After the user provides context, analyze it before asking a questionnaire.

Load `references/interview-map.md` and use it as the audit map. Do not ask every question in it. Use it to decide what information is already strong, what is thin, and what follow-ups would make the wiki much more useful.

First identify the user's primary use case from the use-case routing section. Do not assume it is job search, coding, or AI work. If the source dump does not make the use case obvious, ask the user what they most want the wiki to help with before asking deeper questions.

Do not treat AI exports as enough context by themselves. Exports are only the starting material. Press Start must run a deep interview before building the wiki unless the user explicitly asks to stop.

Identify:

- durable facts
- active projects
- people, organizations, tools, places, and products
- current goals and priorities
- recurring preferences and constraints
- important decisions already made
- raw sources that should be preserved
- potential wiki pages to create
- stale, uncertain, contradictory, or sensitive claims
- context gaps future agents would still struggle with
- the user's likely primary use case and any secondary use cases
- which interview-map topic branches are strong, thin, missing, sensitive, stale, or contradictory

Then present a short intake report:

```text
I found enough to create pages for:
- ...

I need to confirm:
- ...

I am missing:
- ...

Potentially sensitive or stale items:
- ...
```

Keep this report short and practical. Do not turn the whole source dump into a long summary unless the user asks.

## Phase 4: Confirm and filter

Before writing durable pages, ask the user to confirm:

- what is accurate and current
- what is outdated
- what should be excluded
- what should be summarized more privately
- what future agents should always know
- what future agents should avoid assuming

If the user is overwhelmed, ask them to answer only the confirm/exclude items first.

## Phase 5: Run the deep interview

Run at least three rounds of interview questions before building the wiki.

Each round should include about 25 questions. The questions must be customized to:

- the user's primary use case
- what the source dump already says
- what is missing, vague, stale, contradictory, or sensitive
- what future agents would need to know to give surprisingly useful help
- what would make the LLM Wiki feel much better than normal web chat

Before the first round, tell the user:

```text
The export gave us a starting point, but it is not enough by itself. To make this wiki actually useful, I am going to ask a few rounds of deeper questions.

You do not need perfect answers. If you do not know, say "I don't know." If a question does not apply, say "skip." Short answers are fine, but examples are very helpful.
```

Use this structure:

1. **Round 1: Foundation and use case** - identity/current situation, chosen use case, goals, current responsibilities, what they want AI to help with, privacy boundaries.
2. **Round 2: Depth and operating context** - active projects, workflows, people/organizations, constraints, decisions, repeated problems, source files, examples.
3. **Round 3: Personalization and future usefulness** - communication style, advice preferences, writing voice, what AI gets wrong, what great help looks like, open loops, "wow-test" tasks.

After each round:

1. Summarize what you learned in a short bullet list.
2. Identify what is still unclear.
3. Generate the next round from the remaining gaps.

If a user's use case needs more depth after three rounds, ask a fourth targeted round. Do not stop at three rounds if major context is still thin.

Do not build the wiki immediately after the export unless the user explicitly says they want a shallow quickstart.

Use `references/interview-map.md` to choose the next questions. Prioritize branches that create immediate usefulness:

1. the user's chosen use case from the use-case routing section
2. what the user wants AI to help with first
3. current goals and priorities
4. active projects or recurring responsibilities
5. day-to-day work, school, business, creative, or life context
6. communication and advice preferences
7. constraints and privacy boundaries
8. important people, organizations, and decisions

Prefer useful prompts over generic questions. Examples:

- "You mention several projects, but I cannot tell which are active. Which ones matter this month?"
- "You have goals listed, but no constraints. What limits your time, money, energy, or attention?"
- "You mention a collaborator several times. Who are they, and how should future agents understand that relationship?"
- "This looks like a decision, but I do not know the rationale. Why did you choose this path?"
- "I see your resume, but not what you want next. What roles, clients, projects, or opportunities are you aiming for?"

Use section labels so the interview feels easy to answer. It is okay for one round to be long, but keep the wording plain and tell the user they can answer in a messy brain dump.

## Phase 6: Bootstrap the wiki

Create the initial wiki from confirmed context.

Write only pages that have enough substance to be useful. Prefer updating indexes and starter pages over creating many thin pages.

Use the standard page categories:

- `wiki/sources/` for processed source summaries
- `wiki/entities/` for people, organizations, places, products, and tools
- `wiki/concepts/` for recurring ideas, preferences, patterns, and frameworks
- `wiki/decisions/` for decisions with rationale
- `wiki/syntheses/` for cross-source analyses
- `wiki/projects/` for project-specific knowledge

Create or update `wiki/index.md` as a high-level catalog with links and one-line summaries.

Append the bootstrap operation to `wiki/log.md`:

```markdown
## [YYYY-MM-DD] bootstrap | Press Start guided LLM Wiki setup
```

Use the actual current date.

## Phase 7: Readiness report

End with a concise report:

- what the wiki is now good for
- what remains thin or uncertain
- what sources the user should add next
- the exact next command/prompt they can use, such as "Ingest these files into my LLM Wiki."
- one "wow-test" demo task from `references/interview-map.md` that shows how the wiki is better than normal web chat

Explain that Press Start has done its job once the setup is complete. The LLM Wiki is the ongoing system; Press Start is only the onboarding helper.

## Phase 8: Offer to remove Press Start

After setup is complete, ask:

```text
Press Start is only meant for first-time setup. Your LLM Wiki is now the thing future agents should use.

Do you want me to remove or disable the Press Start skill so it does not interfere with future sessions?
```

Only remove or disable the skill if the user clearly approves. If the user says yes and the agent has filesystem access, remove the local `press-start` skill folder or tell the user exactly how to remove it in their environment. If the user is using a shared or installed skill marketplace where deletion is not possible from the current session, explain how to stop invoking it.

Before removing the skill, make sure the LLM Wiki setup instructions are preserved in the user's wiki or agent instructions so future agents know how to use and maintain the wiki without Press Start.

Do not imply the wiki itself is finished forever. The setup is complete, but the point of LLM Wiki is ongoing maintenance.

## Quality bar

Press Start succeeded if:

- the canonical LLM Wiki pattern is installed or verified
- raw sources are preserved instead of overwritten
- the first wiki pages are grounded in confirmed context
- the user did not have to know the schema in advance
- future agents can read the wiki and understand what to do next
- the setup remains faithful to Karpathy's LLM Wiki idea
- the user understands Press Start can be removed after setup
