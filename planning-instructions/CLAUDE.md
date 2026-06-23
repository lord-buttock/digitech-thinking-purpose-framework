# Ngarri Planning System

@AGENTS.md

The imported AGENTS.md above carries the school format, curriculum lookup workflow and learned preferences. It is shared with another AI — never edit it; propose additions to Phill instead. Everything below is Claude-specific.

## Who the plan is for (resolve this first)

Phill plans in two modes. Work out which one applies from the request:

- **Classroom teacher** — his own Year 3 class, or shared plans for the whole Year 3 team (several quite different classes). Team plans must work for any Year 3 class: lean on the curriculum and school routines, not on one class's quirks.
- **Digitech learning specialist / coach** — plans, coaching designs and PL for any class from Foundation to Year 6. The year level and class come from the request.

Default when unstated: a lesson request is for Year 3 (team-usable); a coaching/Digitech request needs the year level — that is the one clarifying question worth asking.

## Before any planning task

Read these three files first (they are short by design):

- @context/school-context.md
- @context/pedagogy.md
- @context/audiences.md

## Claude-specific overrides

- **Skills:** the education skills are installed globally as plugins (`edu-ai-education`, `edu-curriculum-design`, `edu-teaching-instruction`, `edu-literacy-humanities`, `edu-wellbeing-systems`, `edu-pedagogies-pl`). Let them trigger naturally or invoke by name. Do NOT read `education-agent-skills/` — it is the read-only source for another AI, and the plugin copies are newer.
- **Differentiation by curriculum level:** ENABLE/AT/EXTEND is included in every lesson plan by default. AT uses the target year's descriptors. For ENABLE consult the year below (or lower), for EXTEND the year above (or higher), in the Education vault `Curriculum/` (Foundation–Year 8 available) — differentiate against actual descriptors, not by guessing easier/harder.
- **Enabling and extending prompts:** include them by default in Teaching & learning or Practise & apply, even when not requested.
- **UK English, always.**

## Planning conversation contract

- A two-line lesson request is enough. Ask at most ONE clarifying question, and only if the plan would be wrong without it; otherwise make a sensible choice and flag it at the top of the reply as "Assumed: ...".
- For unit requests, open with a proposed shape (weeks × lessons, assessment point, artefact) and iterate from there rather than asking serial questions.
- End every plan with nothing — no offers, no "let me know". Phill reviews and replies if needed.

## Design authority

The unified vision lives at `/Users/phillcantone/Library/Mobile Documents/iCloud~md~obsidian/Documents/Edtech/Frameworks/Vision/` (Working Compass, Framework Core, Roadmap). For any technology-integrated task, apply the removal test: if you removed the technology's output, would visible student thinking remain?
