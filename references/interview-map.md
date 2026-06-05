# Interview Map

Use this reference during Press Start Phases 3-5. It tells the agent what information is useful for a new or existing LLM Wiki and how to ask questions that produce useful context.

Do not ask this as a giant form. Use it as an audit map:

1. Collect existing context first.
2. Identify which branches already have enough detail.
3. Ask at least three rounds of deep interview questions, customized to the user's use case and the gaps in the source material.
4. Confirm sensitive details before writing them into durable files.

Exports are not enough by themselves. They are draft source material. The interview is what turns a generic export into a useful LLM Wiki.

## The Core Test

The first wiki is useful when a future agent can answer:

- Who is this person or organization?
- What are they trying to do right now?
- What are the active projects?
- What do they want AI to help with first?
- What does good help look like to them?
- What constraints should the agent remember?
- What should the agent not assume?
- What files, people, tools, and decisions matter?
- What information is uncertain, stale, or private?

If the answer to any of those is unclear, ask follow-up questions.

Press Start should run during first-time setup or during a deliberate onboarding upgrade pass for an existing thin wiki. After the wiki is strong enough, future sessions should use the LLM Wiki directly instead of re-running this interview.

## Deep Interview Requirement

Press Start must run at least three customized interview rounds before building or upgrading the wiki unless the user explicitly requests a shallow quickstart.

Each round should include about 25 questions.

The user should be told:

```text
You can skip any question. If you do not know, say "I don't know." Messy answers are fine. The goal is not to sound polished; the goal is to give the wiki enough real context to help you later.
```

### Round 1: Foundation and Use Case

Purpose: understand who the user is, what they need help with, and what the wiki is for.

Customize questions around:

- identity and current situation
- primary use case
- current goals
- current responsibilities
- what they want AI to help with first
- current AI skill level
- privacy boundaries

### Round 2: Depth and Operating Context

Purpose: understand the real workflows, projects, people, constraints, and repeated problems.

Customize questions around:

- active projects or responsibilities
- day-to-day workflows
- important people and organizations
- decisions already made
- repeated tasks and open loops
- files, notes, documents, and sources
- what is stale, unclear, or sensitive

### Round 3: Personalization and Future Usefulness

Purpose: make the wiki feel personal enough that future answers are clearly better than normal web chat.

Customize questions around:

- communication style
- advice preferences
- writing voice
- taste and examples
- what AI usually gets wrong
- what good help feels like
- what the agent should never assume
- practical "wow-test" tasks the user wants to try

After each round, summarize what was learned and generate the next round from remaining gaps. If important context is still thin after three rounds, ask a fourth targeted round.

## Use-Case Routing

Do not assume every user's wiki is for job search, coding, or AI projects. First discover the user's highest-value use case, then ask deeper questions in that lane.

Ask early:

```text
What do you most want this AI memory system to help with first?

Common answers:
- career or job search
- current job and daily work
- business, clients, or freelancing
- school or learning
- personal life organization
- creative projects or content
- health, routines, and habits
- family, relationships, or caregiving
- research or writing
- technical/coding projects
- managing lots of documents or meetings
```

If the user is unsure, ask:

```text
What do you keep re-explaining to ChatGPT or Claude?
What would be most valuable if AI remembered it every time?
```

### Broad Use-Case Branches

Use these branches to decide which follow-up questions matter most.

#### Career or Job Search

Useful context:

- current role or employment situation
- target roles, industries, locations, compensation, and constraints
- resume, LinkedIn, portfolio, writing samples, and applications
- strongest proof points and stories
- companies applied to, interviews, rejections, follow-ups, and networking contacts
- what roles are poor fits and why

Good questions:

- What are you trying to get next: job, promotion, career change, internship, clients, or clarity?
- What roles or opportunities are you targeting?
- What roles are you not targeting, even if they look close?
- What are your strongest proof points?
- What are your constraints: location, remote, salary, schedule, visa, family, industry, values?
- What would make AI genuinely useful in this process: resumes, outreach, interview prep, tracking, research, confidence, or decision-making?

#### Current Job and Daily Work

Useful context:

- real responsibilities and workflows
- weekly recurring tasks
- meetings, reports, emails, decisions, and stakeholders
- bottlenecks, politics, deadlines, and success metrics
- information that must stay private or abstract

Good questions:

- What does your actual work week look like?
- What do you repeat every week that AI could help with?
- Who depends on your work?
- What would make you faster, clearer, or less overwhelmed?
- What company or client information should not go in the wiki?

#### Business, Clients, or Freelancing

Useful context:

- offer, customers, pricing, sales process, delivery process, and operations
- current pipeline, leads, partners, and client history
- positioning, proof, objections, and follow-up cadence
- documents like proposals, decks, notes, contracts, and SOPs

Good questions:

- What do you sell or want to sell?
- Who is the ideal customer?
- What problem do you solve for them?
- How do leads currently come in?
- What work do you repeat across clients?
- What should AI help with first: sales, delivery, follow-up, documentation, strategy, or operations?

#### School or Learning

Useful context:

- classes, assignments, deadlines, learning goals, and skill gaps
- study habits, professor expectations, and academic constraints
- notes, readings, papers, rubrics, and project requirements

Good questions:

- What are you studying or trying to learn?
- What deadlines or assignments matter soon?
- What topics are confusing?
- How do you like to study?
- What should AI help with: explanations, plans, flashcards, writing, research, or accountability?

#### Personal Life Organization

Useful context:

- routines, chores, safe high-level finances, errands, and life admin
- recurring responsibilities, calendar pressure, and decision fatigue
- preferences around planning, reminders, tone, and privacy

Good questions:

- What parts of life feel scattered or hard to keep up with?
- What recurring tasks or decisions drain you?
- What does a good week look like?
- What should AI remind you of or help organize?
- What should stay out of the wiki?

#### Creative Projects or Content

Useful context:

- creative identity, audience, platforms, taste, references, and voice
- projects, ideas, drafts, publishing cadence, and constraints
- examples of work the user likes and dislikes

Good questions:

- What are you making?
- Who is it for?
- What style, tone, or taste should AI understand?
- What platforms or formats matter?
- What ideas keep coming back?
- What should AI help with: brainstorming, editing, planning, publishing, or critique?

#### Health, Routines, and Habits

Useful context:

- goals, routines, constraints, preferences, energy patterns, and accountability style
- non-sensitive summaries only unless the user explicitly wants more detail

Good questions:

- What routines or habits are you trying to build?
- What usually gets in the way?
- What kind of accountability helps you?
- What information should stay private or be summarized generally?

Do not provide medical advice. Keep health content framed as personal organization unless the user asks for licensed professional guidance.

#### Family, Relationships, or Caregiving

Useful context:

- roles, responsibilities, communication preferences, boundaries, and recurring decisions
- privacy-sensitive summaries instead of unnecessary detail

Good questions:

- Are there people or responsibilities the assistant should understand to help you plan better?
- What context matters without over-sharing?
- What communication or scheduling patterns should AI remember?
- What should never be stored?

#### Research or Writing

Useful context:

- topics, questions, sources, thesis, audience, and output formats
- citation expectations, writing voice, open questions, and source quality preferences

Good questions:

- What are you researching or writing?
- What question are you trying to answer?
- What sources do you already have?
- Who is the audience?
- What should AI help with: synthesis, outlining, critique, citations, or drafting?

#### Technical or Coding Projects

Useful context:

- repos, architecture, commands, tools, environments, errors, and decisions
- product goals, users, deployment, risks, and project history

Good questions:

- What are you building?
- Where are the files?
- What commands run, test, or deploy it?
- What decisions have already been made?
- What keeps breaking or slowing you down?
- What should AI read before touching the project?

#### Documents, Meetings, or Knowledge Management

Useful context:

- document types, meeting cadence, source folders, recurring decisions, and stakeholders
- privacy policy and what should be summarized vs stored verbatim

Good questions:

- What kinds of documents or meetings do you want AI to remember?
- Where do those materials live?
- What do you wish AI could answer from them?
- What should be copied into raw sources, and what should stay out?

## Target Starter Pages

Use the user's answers to create only pages with enough substance. These are common first pages for a personal or mixed personal/work wiki:

- `wiki/entities/user-profile.md` - who the user is, current situation, background, location/timezone if useful, and current season of life.
- `wiki/projects/_index.md` - active projects and what each one is for.
- `wiki/projects/<project>/overview.md` - one page per active project with goal, status, next steps, blockers, and relevant files.
- `wiki/concepts/preferences.md` - recurring preferences, principles, taste, work style, communication style, and advice style.
- `wiki/concepts/ai-usage.md` - current AI skill level, tools used, workflows, fears, habits, and what they want AI to help with.
- `wiki/decisions/` - important choices already made, with rationale and watch-outs.
- `wiki/syntheses/current-priorities.md` - the best current read on goals, active constraints, and what matters this month.
- `wiki/sources/` - summaries of AI exports, documents, resumes, notes, and other raw materials.

Do not force all of these pages. Use them as destinations when the source material supports them.

## Topic Branches

### 1. Identity and Current Life

Useful when the wiki is for a person. Ask enough to orient future agents without becoming invasive.

Good questions:

- What is the short version of who you are?
- Where are you based, and does timezone or location affect your work?
- What is your current season of life: building, job searching, studying, running a business, changing careers, stabilizing, exploring, or something else?
- What details about your background help explain how you think or work today?
- What do people usually misunderstand about you?

Ask follow-ups when:

- the user gives only a resume-style answer
- current reality differs from past history
- location, schedule, family, school, visa, money, health, or work situation affects decisions

### 2. Work and Responsibilities

Useful because many "AI help" requests depend on real job context.

Good questions:

- What do you actually do day to day?
- What are you responsible for that other people depend on?
- What repeated tasks, messages, reports, meetings, decisions, or deliverables do you deal with?
- What part of your work is easiest for you?
- What part drains you or creates bottlenecks?
- Who are the important teams, customers, clients, managers, collaborators, or stakeholders?
- What work information should not be stored, or should only be summarized generally?

Ask follow-ups when:

- the user gives a title but no workflow
- they mention clients, customers, managers, or coworkers without context
- there is sensitive company data involved

### 3. Goals and Direction

Useful because agents make better suggestions when they know what direction matters.

Good questions:

- What are your top goals for the next 30 days?
- What are your top goals for the next 3 months?
- What are your longer-term goals?
- What are you trying to build, grow, fix, change, or escape?
- Which goals are real commitments, and which are just ideas?
- What would make this wiki setup feel successful within one week?

Ask follow-ups when:

- goals conflict with each other
- goals lack deadlines, stakes, or next actions
- the user has many goals but no priority order

### 4. Active Projects

Useful because project pages are where the wiki starts feeling alive.

Good questions:

- What projects are active right now?
- Which projects matter most this month?
- For each project: what is it, why does it matter, what is the current status, and what is the next useful step?
- What files, docs, links, chats, or notes belong to each project?
- What is blocked, confusing, stale, or undecided?
- What would a helpful AI assistant do for this project every week?

Ask follow-ups when:

- the user mentions a project name without explaining it
- it is unclear whether a project is active, paused, abandoned, or aspirational
- the next action is missing

### 5. AI Experience and Tooling

Useful because Press Start is often moving the user from web chat into file-working agents.

Good questions:

- Which AI tools do you use today: ChatGPT, Claude, Gemini, Perplexity, Cursor, Codex, Claude Code, or something else?
- What do you usually ask AI for?
- What does AI currently do well for you?
- What does AI get wrong, miss, or make annoying?
- Have you ever used Terminal, GitHub, code editors, or local files with an AI assistant?
- What feels intimidating or confusing about this setup?
- What would make you say, "Oh wow, this is way better than normal ChatGPT"?

Ask follow-ups when:

- the user only knows web chat
- the user confuses model memory with local files
- the user has had bad AI experiences or is anxious about privacy

### 6. Preferences, Taste, and Communication

Useful because agents need to adapt to how the user actually wants help.

Good questions:

- How do you like people to explain things to you: short, detailed, visual, step-by-step, blunt, encouraging, strategic, or hands-on?
- What kind of advice do you actually use?
- What kind of advice annoys you?
- What should an AI never assume about you?
- What should an AI do before giving major advice?
- What writing voice should AI use for you?
- Are there words, tones, formats, or styles you dislike?

Ask follow-ups when:

- the user says "make it sound like me" but gives no writing samples
- they dislike AI-sounding writing but cannot explain why
- they want different tones for work, friends, clients, or public content

### 7. Constraints and Boundaries

Useful because constraints prevent bad suggestions.

Good questions:

- What limits your time, energy, money, attention, location, tools, access, or schedule?
- What privacy boundaries should the wiki respect?
- What topics should not be stored in local files?
- What sensitive topics can be summarized abstractly instead of written directly?
- Are there employer, client, school, legal, or family boundaries the agent should remember?
- What is safe for the agent to help with, and what should require your explicit approval?

Ask follow-ups when:

- constraints are implied but not stated
- the user shares sensitive details without deciding how they should be stored
- work or client information may be confidential

### 8. People, Organizations, and Relationships

Useful because names without context are hard for future agents to use.

Good questions:

- Who are the important people in your work or life that an assistant should understand?
- For each person: who are they, how are you connected, what context matters, and what should the AI be careful about?
- What organizations, clients, companies, schools, communities, or groups matter?
- Are any relationships sensitive or private enough to omit or summarize lightly?

Ask follow-ups when:

- a person or organization appears repeatedly in the source dump
- relationship status, role, or importance is unclear
- the agent might otherwise over-assume familiarity

### 9. Decisions and Open Loops

Useful because decisions are where memory compounds.

Good questions:

- What decisions have you already made that future AI should not relitigate?
- What decisions are still open?
- What tradeoffs are you weighing?
- What did you try before, and what happened?
- What keeps coming up again and again?
- What should the AI remind you of when you drift or overthink?

Ask follow-ups when:

- the source material includes "I decided" or "I might" but no rationale
- the same issue appears in multiple sources
- the user keeps asking AI the same question

### 10. Sources and Raw Materials

Useful because the wiki should be grounded.

Good questions:

- What files or notes should we include first?
- Do you have resumes, bios, project docs, meeting notes, pitch decks, plans, research, old AI chats, or writing samples?
- Which sources are current?
- Which sources are outdated but still useful as history?
- Which sources should be kept out for privacy or policy reasons?

Ask follow-ups when:

- the user gives a conclusion without a source
- old and new files conflict
- the user has more material but has not gathered it yet

## Missing-Context Audit

After reading the source dump, score each branch:

- Strong: enough detail to write useful wiki content.
- Thin: some facts exist, but future agents would still ask obvious questions.
- Missing: little or no useful context.
- Sensitive: useful but needs abstraction or exclusion.
- Stale: likely outdated.
- Contradictory: sources disagree.

Then tell the user:

```text
I found strong context for:
- ...

I need to ask a few questions about:
- ...

I will not write these sensitive items unless you approve how to store them:
- ...
```

## The Wow-Test Demo

After the first wiki is created, prove the value with one real task.

Pick a demo from the user's own goals:

- draft an email in their style using relationship and project context
- create a weekly plan using active goals and constraints
- summarize a project and propose next steps
- turn a messy idea into a project page
- help prepare for a meeting using people, goals, and open loops
- improve a document using their writing preferences

Explain the contrast:

```text
Normal web chat would answer from this prompt alone. Your LLM Wiki lets the agent answer using your background, goals, projects, preferences, constraints, and previous decisions.
```
