![Press Start banner](assets/readme-banner/press-start-banner.gif)

# Press Start

**Guided first-run onboarding for [Andrej Karpathy's LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f), made for complete beginners.**

Press Start is a one-time setup skill. It helps someone move from ChatGPT or Claude in a browser to a file-working agent like Codex or Claude Code, install the proven Karpathy-style LLM Wiki pattern, collect useful context from existing AI chats and documents, answer targeted follow-up questions, and bootstrap the first useful wiki pages.

No AI background is assumed.

Press Start does **not** replace or redesign LLM Wiki. Karpathy's LLM Wiki is the backbone. Press Start is the beginner-friendly setup guide.

## Why This Exists

Most people start with AI in a web chat box. That works, but it means they keep re-explaining the same context: who they are, what they are working on, what they want, what matters, what they dislike, and what has already been decided.

LLM Wiki solves that by putting durable context into local markdown files an agent can read and maintain.

Press Start makes the first setup easy enough for a beginner:

1. Explain the move from web chat to a file-working agent.
2. Set up the Karpathy-style LLM Wiki structure.
3. Collect context from ChatGPT, Claude, Gemini, Perplexity, documents, notes, and project files.
4. Confirm what is accurate, stale, private, or missing.
5. Ask targeted questions based on the user's actual use case.
6. Build the starter wiki.
7. Offer to remove or disable itself once setup is complete.

## What It Does

- Points users to the canonical LLM Wiki source first.
- Explains the difference between web chat and a file-working agent in plain language.
- Walks beginners toward Codex or Claude Code one step at a time.
- Verifies or creates the standard `raw/` and `wiki/` structure.
- Gives copy-paste prompts for ChatGPT, Claude, Gemini, Perplexity, and coding agents.
- Helps users paste messy context back into the setup chat.
- Finds missing, stale, sensitive, or contradictory information.
- Asks targeted follow-up questions instead of a generic form.
- Creates the initial wiki pages, index, and bootstrap log entry.
- Offers to remove or disable itself after setup is complete.

## Who It Is For

Press Start is for people who:

- use ChatGPT, Claude, Gemini, or Perplexity in a browser
- want AI to remember more useful context
- are new to Codex, Claude Code, Terminal, GitHub, markdown, or local files
- want a guided setup instead of a technical explanation
- are helping a friend, client, teammate, or family member set up an LLM Wiki

It works for broad use cases, including career planning, current job workflows, school, personal organization, business/freelancing, creative projects, research, coding, meetings, and document-heavy work.

## How It Works

Press Start uses a **collect -> confirm -> construct** flow.

### 1. Collect

The skill gives the user copy-paste prompts for the tools they already use, such as ChatGPT, Claude, Gemini, Perplexity, Codex, Claude Code, Cursor, Notion, Google Docs, or Obsidian.

The user pastes the results back into the setup chat or adds files to `raw/`.

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
- Codex and Claude Code can also work with files on your computer.
- LLM Wiki is a folder of text files that gives those assistants memory.
- Press Start walks you through setting that up.

If someone sent you this repo, ask them to help you open Codex or Claude Code first. Then paste this:

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

Useful official setup links:

- Codex: https://developers.openai.com/codex/explore
- Claude Code: https://docs.anthropic.com/en/docs/claude-code/getting-started

## Positioning

Press Start is intentionally narrow.

- It is not a new wiki architecture.
- It is not a replacement for Karpathy's LLM Wiki.
- It is not an ongoing daily workflow skill.
- It is setup scaffolding.

Once the user's wiki is ready, Press Start should offer to remove or disable itself so future agents use the LLM Wiki directly.

## License

MIT
