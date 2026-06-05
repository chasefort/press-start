![Press Start banner](assets/readme-banner/press-start-banner.gif)

# Press Start

**Guided onboarding for [Andrej Karpathy's LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f), made for complete beginners.**

Press Start is an onboarding skill. It runs inside a file-working agent like Codex or Claude Code, installs or improves the proven Karpathy-style LLM Wiki pattern, collects useful context from existing AI chats and documents, asks deep customized interview questions, and bootstraps or upgrades useful wiki pages.

No AI background is assumed.

Press Start does **not** replace or redesign LLM Wiki. Karpathy's LLM Wiki is the backbone. Press Start is the beginner-friendly setup guide.

## Why This Exists

Most people start with AI in a web chat box. That works, but it means they keep re-explaining the same context: who they are, what they are working on, what they want, what matters, what they dislike, and what has already been decided.

LLM Wiki solves that by putting durable context into local markdown files an agent can read and maintain.

Press Start makes setup or enhancement easy enough for a beginner:

1. Explain what an AI memory folder is.
2. Detect whether an LLM Wiki already exists.
3. If there is no wiki, ask where the user wants the folder created.
4. If there is a wiki, audit what is already strong, thin, stale, or missing.
5. Collect context from ChatGPT, Claude, Gemini, Perplexity, documents, notes, and project files.
6. Confirm what is accurate, stale, private, or missing.
7. Run at least three rounds of deep, customized interview questions based on the user's actual use case.
8. Build or upgrade the wiki.
9. Offer to remove or disable itself once onboarding is complete.

## What It Does

- Points users to the canonical LLM Wiki source first.
- Explains why a local AI memory folder is different from normal web chat.
- Detects whether an LLM Wiki already exists and upgrades it instead of creating a duplicate.
- Asks where the user wants the wiki folder created and suggests Desktop as the easiest default.
- Verifies or creates the standard `raw/` and `wiki/` structure.
- Gives copy-paste prompts for ChatGPT, Claude, Gemini, Perplexity, and coding agents.
- Tells users to review and correct AI exports before treating them as source material.
- Helps users paste corrected messy context back into the setup chat.
- Finds missing, stale, sensitive, or contradictory information.
- Asks at least three rounds of targeted interview questions instead of treating an export as enough.
- Creates or improves wiki pages, indexes, and log entries.
- Offers to remove or disable itself after onboarding is complete.

## Who It Is For

Press Start is for people who:

- use ChatGPT, Claude, Gemini, or Perplexity in a browser
- want AI to remember more useful context
- are new to Codex, Claude Code, GitHub, markdown, or local files
- want a guided setup instead of a technical explanation
- are helping a friend, client, teammate, or family member set up an LLM Wiki

It works for broad use cases, including career planning, current job workflows, school, personal organization, business/freelancing, creative projects, research, coding, meetings, and document-heavy work.

## How It Works

Press Start uses a **collect -> confirm -> construct** flow.

### 1. Collect

The skill gives the user copy-paste prompts for the tools they already use, such as ChatGPT, Claude, Gemini, Perplexity, Codex, Claude Code, Cursor, Notion, Google Docs, or Obsidian.

The user pastes the results back into the setup chat or adds files to `raw/`.

AI exports are treated as source material, not automatic truth. The user is asked to read them, correct mistakes, remove anything too private, and add missing context before the wiki is built.

The export is only the starting point. Press Start then runs a deeper interview, usually three rounds of about 25 questions, customized to the person's use case and the missing context. Users can skip any question or say "I don't know."

### 2. Confirm

The skill reviews the material and reports:

- what is strong enough to turn into wiki pages
- what is missing
- what seems stale
- what may be sensitive
- what contradicts other sources

The user confirms what should be kept, excluded, or summarized more privately.

### 3. Construct

The skill creates the starter LLM Wiki structure and initial pages, then shows a practical "wow test" task that demonstrates why this is better than normal web chat.

## Repository Contents

```text
README.md
SKILL.md
agents/openai.yaml
references/interview-map.md
references/context-export-prompts.md
assets/readme-banner/
```

## If You Are Brand New

You do not need to understand AI, coding, GitHub, or the command line.

The basic idea is simple:

- ChatGPT and Claude in a browser mostly talk with you.
- The assistant running Press Start can work with files on your computer.
- LLM Wiki is a folder of text files that gives those assistants memory.
- Press Start walks you through setting that up.

If someone sent you this repo, open it in the agent environment they recommended. Then paste this:

```text
Use Press Start to help me set up a Karpathy-style LLM Wiki. I am a complete beginner, so explain everything one step at a time and do not assume I know AI, coding, Terminal, GitHub, markdown, folders, or files.
```

## If You Are Helping Someone

Install or copy the skill into their agent environment, then start with:

```text
Use $press-start to install a Karpathy-style LLM Wiki and guide me through first-run context intake.
```

The skill will start by sending you to the canonical LLM Wiki:

https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f

Then it will walk you through the beginner setup process step by step.

## Positioning

Press Start is intentionally narrow.

- It is not a new wiki architecture.
- It is not a replacement for Karpathy's LLM Wiki.
- It is not an ongoing daily workflow skill.
- It is setup scaffolding.

Once the user's wiki is ready or upgraded, Press Start should offer to remove or disable itself so future agents use the LLM Wiki directly.

## License

MIT
