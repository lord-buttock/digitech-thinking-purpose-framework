# Lesson Planning Workspace Instructions

This workspace contains a local education skill library at:

`education-agent-skills/skills/`

## Local education skills

When a task involves lesson planning, curriculum design, assessment, pedagogy, learning science, AI literacy, historical thinking, inclusive design, professional learning, student wellbeing, or related education work:

1. Search `education-agent-skills/skills/` for relevant `SKILL.md` files.
2. Read the best-matching skill file before producing the response or artifact.
3. Apply the skill's guidance as local context for this workspace only.
4. Prefer using a small number of directly relevant skills rather than loading the full library.

Do not assume the education skills are globally installed. Treat them as project-local reference material for this `Lesson planning` folder.

## Victorian Curriculum alignment

This workspace also has a local Victorian Curriculum reference folder at:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Education/Curriculum`

Phill's broader Education Obsidian vault is at:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Education`

The master index is:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Education/index.md`

Use this index to locate school resources, teaching strategy documents, writing resources, lesson plans, inquiry resources, reporting notes, and curriculum files. Phill will keep this index updated as new documents and folders are added, so treat it as the living source of truth and re-check it during future planning tasks rather than relying only on remembered resource paths.

For lesson planning or teacher-support tasks that may require local school documents:

1. Read `Education/index.md` first to find the relevant folder or indexed resource.
2. Follow the index to the most relevant local resource before relying on generic advice.
3. Prefer the Obsidian `.md` companion file when available, and use the linked PDF only when the markdown summary is missing, unclear, or the exact source wording/visual convention matters.
4. When choosing reflections, consult `Education/Teaching Strategies/Ngarri Reflect Phase.md` or its PDF companion.
5. When planning writing/editing lessons, check `Education/Writing/` and any relevant Teaching Strategies resources, including Rainbow Editing resources if they are indexed there.
6. When adapting or continuing lesson sequences, check `Education/Lesson Plans/` and any user-provided weekly planning files before assuming what students have already done.

When creating or adapting lesson plans, unit plans, learning goals, success criteria, assessment tasks, or teaching sequences:

1. Identify the year level and curriculum level from the user's request. For example, Year 3 uses `Year-3/` and English/Mathematics `Level 3`.
2. Identify the relevant learning area or capability. For example, Writing uses `Year-3/English.md`; Maths uses `Year-3/Mathematics.md`; sustainability inquiry may use both the relevant learning area and `Year-3/Sustainability.md`.
3. Read the relevant year-level index and subject file before finalising the plan. For example:

```bash
sed -n '1,220p' "/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Education/Curriculum/Year-3/index.md"
rg -n "VC2E3|writing|write|text|texts|paragraph|punctuation|persuasive|argument|opinion|audience|purpose" "/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Education/Curriculum/Year-3/English.md"
```

4. Align the lesson to the closest relevant curriculum content descriptions, achievement-standard language, and elaborations. For Year 3 writing, likely relevant codes include `VC2E3LA03`, `VC2E3LA04`, `VC2E3LY11`, and `VC2E3LY12`, depending on the lesson focus.
5. If the lesson idea does not clearly align with the expected year-level curriculum, flag the mismatch and suggest a small adjustment that keeps the user's intent.
6. Use relevant local education skills alongside the curriculum check. For curriculum mapping tasks, consider skills in `education-agent-skills/skills/curriculum-alignment/` as well as any subject-specific or pedagogy skill that matches the task.

When writing final lesson plans for the user, include curriculum alignment only when it helps the user. Keep it copy-paste friendly and concise, for example:

```text
Curriculum alignment:
VC2E3LY11 - create persuasive texts with ideas grouped in simple paragraphs.
VC2E3LA03 - describe how simple arguments use text structures and language features for purpose.
```

Do not output curriculum alignment as a table unless the user explicitly asks for a table.

## Digitech, edtech, and coaching resources

Phill is also a Digital Technologies learning specialist and uses this workspace for coaching, professional learning, and meaningful digital technology integration across the curriculum.

The Coaching Obsidian folder is:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Coaching`

The Coaching index is:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Coaching/index.md`

The Edtech Obsidian folder is:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Edtech`

The Edtech index is:

`/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Edtech/index.md`

When the user asks for coaching lessons, coaching cycles, professional learning, Digital Technologies lessons, iPad creativity tasks, edtech workflows, or ideas for integrating digital technologies meaningfully into curriculum:

1. Read the relevant Coaching and/or Edtech index before responding.
2. If the task is year-level specific, check the relevant year-level Coaching index when available, for example `Coaching/Year-3/index.md`.
3. Also check the Education curriculum folder and the Education index when the task involves curriculum alignment, lesson planning, assessment, inquiry, or classroom implementation.
4. Use the local education skills from `education-agent-skills/skills/` alongside these vault resources. Prefer skills related to curriculum design, authentic learning, formative assessment, learning progression, project design, inquiry, creativity, AI literacy, or digital technology integration where relevant.
5. Prefer meaningful integration over tool-first planning. Start from the learning intention, curriculum, thinking skill, creative purpose, audience, or classroom problem, then choose the technology only when it strengthens the learning.
6. For iPad tasks, aim for creative, student-centred uses such as making, explaining, documenting, designing, composing, coding, filming, animating, reflecting, collaborating, or publishing, rather than substituting a worksheet onto a screen.
7. If the user asks for coaching support for teachers, keep the tone collegial and practical: include the teacher goal, student learning purpose, small achievable next step, possible modelling/co-teaching move, and evidence of impact.

## Ngarri lesson-plan format

When writing or adapting lesson plans for Phill/Ngarri Primary School, use the school's planning format unless the user asks for a different format.

Use this table structure for lesson plans:

```text
| Session | ENGAGE | LEARNING GOAL / SUCCESS CRITERIA / VOCAB | TEACHING & LEARNING | PRACTISE & APPLY | REFLECTION / FEEDBACK |
```

This table structure is only a schema for understanding the school's planning sections. Do not output lesson plans as Markdown tables at any stage unless the user explicitly asks for a table. Instead, output copy-paste-friendly plain sections in this order:

```text
Session:

Engage:

Learning goal:

Success criteria:

Vocab:

Teaching & learning:

Practise & apply:

Reflection / feedback:

Resources:
```

Keep each section as unformatted plain text where practical so it can be copied into school planning documents easily.

For Maths lessons, use the school's Maths heading:

```text
| Session | ENGAGE Daily Review x 3 Number Talk x 1 Reasoning x 1 | LEARNING GOAL / SUCCESS CRITERIA / VOCAB | TEACHING & LEARNING | PRACTISE & APPLY | REFLECTION/FEEDBACK |
```

For final Maths lesson plans sent to the user, use the same plain-section approach, but label the first teaching section:

```text
Engage Daily Review x 3 Number Talk x 1 Reasoning x 1:
```

Use the school wording style:

```text
We are learning to [clear skill, concept, or learning action].

I can [observable student action].
I can [observable student action].
I can [observable student action].

Vocab: [key vocabulary]
```

Success criteria must be observable and student-facing. Prefer verbs such as identify, describe, explain, compare, justify, create, use, record, share, and reflect. Avoid vague criteria such as "I can understand..." unless the user specifically requests it.

## Preserving vs creating learning goals

When adapting an existing lesson plan:

- Preserve the existing learning goal, success criteria, vocabulary, lesson intent, differentiation labels, and classroom routines unless the user asks to change them.
- Preserve the sequence of prior learning and follow-on learning where possible.
- Make adaptations by changing resources, scaffolds, examples, grouping, timing, or teacher instructions rather than changing the learning destination.

When creating a new lesson plan from the user's ideas or rough notes:

- Generate an appropriate learning goal, success criteria, and vocabulary in the Ngarri format.
- Use `education-agent-skills/skills/original-frameworks/learning-target-authoring-guide/SKILL.md` to shape "I can..." statements with observable verbs.
- Use relevant subject or pedagogy skills from `education-agent-skills/skills/*/*/SKILL.md` alongside the Ngarri format.
- Keep the lesson practical for Year 3 unless the user specifies a different year level.

## Differentiation and classroom style

Use the school's differentiation labels when relevant:

```text
ENABLE:
AT:
EXTEND:
```

Differentiation should preserve the same learning goal while changing the amount of support, response format, examples, or level of reasoning.

For Reading, Writing, Inquiry, and Maths lessons, include resources at the bottom of the table when useful. If phonics or word work is requested as a short transition between Reading and Writing, write it as a separate "In-Between Activity" rather than embedding it inside the Reading planner.

For relief teacher plans, prioritise:

- clear step-by-step teacher directions
- low-tech options
- no assumptions about slides, videos, or printing unless the user confirms they are available
- use of normal classroom materials such as whiteboards, markers, writing sheets, reading journals, inquiry books, maths grid books, scrapbooks, dice, and pencils

## Phill/Ngarri lesson planning preferences learned from use

When writing lesson plans in this project:

- Check the prior lesson sequence before planning the next lesson. Build from what students have already done, including existing groups, topics, plans, notebooks, posters, or shared artefacts.
- For Writing lessons, do not include an Engage section by default because phonics usually occurs before Writing. If an opening activity is needed, include it inside Teaching & learning.
- Treat Writer's Workshop lessons as general writing craft or trait lessons. Do not force them to connect to the current unit unless the user asks. Students may apply the workshop focus to their current writing or another piece from their writer's notebook.
- For collaborative planning, prefer shared visible artefacts such as A3 paper, posters, or group planning sheets when the group needs to organise ideas together.
- Keep learning goals precise and aligned to what students are actually doing. Do not use stronger verbs such as strengthen, evaluate, or justify unless the lesson requires that thinking.
- Prefer three success criteria where possible. Make them observable, student-facing, and directly linked to the task students will complete.
- Use Ngarri classroom routines and named tools when provided, such as Rainbow Editing and the Ngarri Reflect options.
- Choose reflections from the Ngarri Reflect document that match the lesson objective and avoid repeating the same reflection in back-to-back lessons where possible.
- Keep final lesson-plan output copy-paste friendly: plain section headings, no Markdown tables unless explicitly requested.
