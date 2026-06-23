# Digitech Thinking Purpose Framework

> Not more tech. Better tech.

A thinking-first framework for meaningful digital technology integration across Foundation–Year 6, developed by Phill Cantone, Year 3 classroom teacher and Digital Technologies Learning Specialist at Ngarri Primary School, Melbourne.

---

## For AI assistants — read this first

This repository is an AI-readable system. If you are an AI assistant helping Phill, start here, then follow the links below to the documents most relevant to your task.

**Who Phill is:**
- Year 3 classroom teacher (plans for his own class and the whole Year 3 team)
- Digital Technologies Learning Specialist / coach for Foundation–Year 6
- Based at Ngarri Primary School, Melbourne, Victoria, Australia
- Works within the Victorian Curriculum (VC2) and Victorian Teaching and Learning Model 2.0 (VTLM 2.0)
- UK English in all written output

**How to help Phill:**
- For lesson planning → start at [`planning-instructions/AGENTS.md`](planning-instructions/AGENTS.md) and [`planning-instructions/CLAUDE.md`](planning-instructions/CLAUDE.md)
- For framework questions → start at [`framework/vision/framework-core.md`](framework/vision/framework-core.md)
- For skill selection → start at [`skills/quick-finder.md`](skills/quick-finder.md)
- For curriculum alignment → check [`curriculum/indexes/`](curriculum/indexes/)
- For coaching or PL design → check [`coaching/index.md`](coaching/index.md)

---

## The framework in brief

Most technology integration fails the same way: the tool does the thinking. Students produce artefacts with no visible reasoning behind them. The conventional response — *"How can we use iPads in this lesson?"* — guarantees the failure it is trying to avoid.

This framework answers a different question: **what kind of thinking does this lesson require, and would technology genuinely enhance it?**

### The planning chain

```
learning purpose → thinking strategy → student role → technology enhancement → artefact → evidence of learning
```

Technology comes fourth. If the chain works without it, the lesson does not need it.

### The Removal Test

> **If you removed the technology's output entirely, would visible student thinking remain?**

- iPad form: *"Why not paper?"* — every activity must have an explicit answer.
- AI form: *"If you removed the AI output, would the student thinking still be visible?"*

If the answer is no, the task is substitution wearing a digital costume.

### The nine thinking-purpose categories

Rather than asking *what tool*, ask *what kind of thinking*:

| Category | What students do |
|---|---|
| Notice, Wonder & Explore | Slow observation, generating questions, first-encounter thinking |
| Compare, Classify & Analyse | Finding patterns, sorting, identifying features and relationships |
| Investigate, Connect & Explain | Building understanding, researching, explaining to an audience |
| Explore Objects, Systems & Design | Handling, testing, examining how things work |
| Explore Perspectives & Impacts | Taking different viewpoints, exploring consequences |
| Imagine, Design & Improve | Creating, prototyping, iterating |
| Code, Model & Simulate | Computational thinking, building models |
| Organise, Summarise & Show Understanding | Synthesising, curating, presenting learning |
| Reflect, Evaluate & Improve | Metacognition, reviewing, self-assessing |

Each category has a full guide specifying thinking strategies, student roles, strong digital artefacts, the substitution danger zone, and the required evidence of learning. See [`framework/meaningful-ipad-use/`](framework/meaningful-ipad-use/).

### Where this sits inside VTLM 2.0

VTLM 2.0 (the Victorian state pedagogical model) says nothing about technology integration. This framework fills that gap specifically at the **Supported Application → Apply learning and build mastery** stage — where students work independently with content they have already been explicitly taught. See [`framework/thinking-purpose/vtlm-alignment.md`](framework/thinking-purpose/vtlm-alignment.md).

---

## Repository structure

```
digitech-thinking-purpose-framework/
│
├── README.md                          ← You are here
│
├── planning-instructions/             ← AI planning system (start here for lesson requests)
│   ├── CLAUDE.md                      ← Claude Code–specific instructions
│   ├── AGENTS.md                      ← Shared format: lesson schema, curriculum workflow
│   └── context/
│       ├── pedagogy.md                ← Framework summary, thinking strategies, differentiation
│       └── audiences.md               ← Who plans are for (Year 3 team, F–6 coaching)
│
├── framework/
│   ├── vision/                        ← Unified framework (principles, roadmap)
│   │   ├── framework-core.md          ← Five principles + Removal Test (start here)
│   │   ├── working-compass.md         ← Internal north star: unified thesis + two lenses
│   │   ├── roadmap.md                 ← 6-project build sequence
│   │   └── index.md
│   ├── thinking-purpose/              ← Where the framework meets VTLM 2.0
│   │   ├── vtlm-alignment.md          ← Full alignment map: 4 elements × framework role
│   │   └── thinking-strategies-and-ipad-enhancements.md
│   └── meaningful-ipad-use/           ← Category guides (iPad layer of the framework)
│       ├── index.md
│       ├── notice-wonder-explore.md   ← Current guide (V2)
│       └── investigate-connect-explain.md
│
├── skills/                            ← Education Agent Skills catalog
│   ├── index.md                       ← All 164 skills A–Z with descriptions + domain table
│   ├── quick-finder.md                ← Skills grouped by planning task (start here)
│   └── domains/                       ← 20 domain folders × individual skill files
│       ├── AI Learning Science/       ← 14 skills
│       ├── AI Literacy/               ← 7 skills
│       ├── Curriculum Assessment/     ← 13 skills
│       ├── Student Learning/          ← 13 skills (retrieve→apply→transfer)
│       └── ... (16 more domains)
│
├── teaching-strategies/
│   ├── vtlm-2-0/                      ← VTLM 2.0 companion notes
│   │   ├── index.md
│   │   ├── guide-pack.md              ← Full 15-page guide summary
│   │   ├── implementation-rubric.md
│   │   └── reflection-tool.md
│   └── thinking-tools/
│       └── index.md                   ← Thinking routines: VTR, DATT, Hats, HoM, Thinker's Keys
│
├── curriculum/
│   └── indexes/                       ← Victorian Curriculum year-level indexes (F–6)
│       ├── Foundation-index.md
│       ├── Year-1-index.md
│       └── ... through Year-6
│
└── coaching/
    └── index.md                       ← Coaching resources overview
```

---

## Education Agent Skills

164 skills are available via Claude's plugin system, created by Gareth Manning (open source: [education-agent-skills](https://github.com/GarethManning/education-agent-skills)).

To find the right skill for a task: [`skills/quick-finder.md`](skills/quick-finder.md)

To see all skills by domain: [`skills/index.md`](skills/index.md)

To invoke a skill, ask Claude: *"Use the `backwards-design-unit-planner` skill to…"*

---

## What is not in this repository

- Student names, individual student data, or learning profiles
- Parent contact records
- Semester reporting notes
- PDFs from the Victorian Department of Education (DET copyright)
- The full Victorian Curriculum VC2 data files (use the official [Victorian Curriculum website](https://victoriancurriculum.vcaa.vic.edu.au/) or Phill's local Obsidian vault)

---

## Status

The framework is under active development. Current state (June 2026):

| Component | Status |
|---|---|
| Framework Core (5 principles + Removal Test) | ✓ Written |
| VTLM 2.0 alignment | ✓ Written |
| 9 thinking-purpose categories (overview) | ✓ Defined |
| Thinking-purpose category guides | 2 of 9 written (Notice/Wonder/Explore, Investigate/Connect/Explain) |
| Education Agent Skills catalog | ✓ 164 skills, 20 domains |
| AI planning instruction system (CLAUDE.md / AGENTS.md) | ✓ Active |
| Planning database (Obsidian searchable) | In progress |
| PTCCD pattern (AI task design) | Draft |

---

*Developed by Phill Cantone, Ngarri Primary School. Private repository.*
