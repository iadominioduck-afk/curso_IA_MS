# UX/UI and Structure Guide for Session Pages

Reference analyzed: [sesiones/sesion-01.qmd](/Users/michellegonzalez/Documents/GitHub/curso_IA/sesiones/sesion-01.qmd)

This document explains the UX, UI, structural, and pedagogical patterns used in `sesion-01.qmd` so the same language can be applied across `sesion-02.qmd` through `sesion-15.qmd`.

Use this file as:
- a style guide
- a migration checklist
- a prompt/spec for batch-updating the other session files

## Goal

The goal of the session pages is not just to look polished. The design is doing teaching work.

The reference session uses a consistent structure that:
- lowers intimidation
- makes abstract AI ideas feel concrete
- alternates explanation with interaction
- gives students repeated orientation cues
- ends with reflection and synthesis

The right standard is not “make every page pretty.” The right standard is:

“Make every page feel like an intentional learning experience with the same visual grammar, pacing, and pedagogical scaffolding as Session 1.”

## Core Design Principles

### 1. Story first, definition second

The session begins with a real-world, high-recognition hook before defining the concept.

Pattern:
- start with apps or behaviors students already know
- then define the concept
- then show how the concept works

Pedagogical reason:
- students engage faster when they first recognize the phenomenon
- once relevance is established, formal definitions become easier to absorb

### 2. Concrete to abstract to concrete

Session 1 repeatedly follows this loop:
- show a familiar example
- explain the underlying concept
- return to a familiar example or interactive

Pedagogical reason:
- students retain abstractions better when they can bounce between concept and example

### 3. One visual idea per block

Each content block has a clear job:
- banner for orientation
- intro phone for relevance
- definition card for shared language
- key-moment formula for conceptual compression
- demo shells for interaction
- central-idea card for synthesis

Pedagogical reason:
- each block reduces cognitive load by answering one question at a time

### 4. Interaction is explanatory, not decorative

The interactive demos are not “extras.” They are part of the explanation.

Each demo follows the same pattern:
- preview of what the student is about to see
- live stage where the interaction happens
- “Qué estás viendo”
- “Qué significa”
- status line
- actions

Pedagogical reason:
- students need interpretation, not just animation
- the explanation must stay close to the action

### 5. Repetition of structure builds confidence

Session 1 reuses a consistent shell for interactive content. This is important to preserve across all sessions.

Pedagogical reason:
- when layout stays stable, students can focus on ideas instead of re-learning the interface every time

## Structural Template for Session Pages

This is the structural pattern to replicate across sessions where appropriate.

### A. Frontmatter

Each session should keep a lightweight Quarto frontmatter:
- title
- `format: html`
- `toc: true`
- `toc-depth: 2`
- `number-sections: false`

### B. Session Banner

The page opens with a banner that includes:
- block label
- progress bar
- session number out of 15
- date
- duration
- link back to syllabus

Purpose:
- gives orientation immediately
- makes the course feel like a coherent sequence

### C. Page Assets

Near the top, the page links:
- the session-specific stylesheet in `styles/sessions/`
- the session-specific JS in `interactives/`

Pattern:
- keep shared global styling in `styles/sesion.css`
- keep session-specific additions in `styles/sessions/sesion-XX.css`
- keep per-session interactivity in `interactives/sesion-XX.js`

### D. Opening Capsule Sequence

Session 1 now uses a specific opening sequence that should be treated as a repeated course-wide convention.

Canonical order:
- `## Introducción a la IA`
- opening video capsule or placeholder
- the complement/disclaimer note
- `### Introducción`
- the written teaching sequence

This order matters because it makes the first learning unit feel consistent from session to session.

If a session has a real video:
- embed it in the opening capsule slot

If a session does not yet have a real video:
- keep the same opening slot
- use a polished placeholder instead of omitting the section
- preserve the complement/disclaimer note anyway so the learning logic stays consistent

### E. Video/Text Complement Disclaimer

This note should be standardized across sessions.

Requirements:
- same class: `capsule-complement-note`
- same structural placement, between the opening capsule and the written introduction
- ideally the exact same wording

Reference wording from Session 1:

“Los videos y el texto de esta sesión son complementarios. Los videos amplían el contexto histórico y conceptual; el texto va a los mecanismos y te pone a interactuar con ellos. Encontrarás ideas en los videos que el texto no repite exactamente. ¡Disfruta de esta dinámica!”

Purpose:
- tells students the video and text are complementary, not redundant
- reduces confusion about why both exist
- creates a repeated course rhythm students can trust

### F. Text Content Section

After the opening capsule and disclaimer, the page shifts to full text and interactive content.

Typical order in Session 1:
- introduction hook
- core definition
- myth correction / conceptual clarification
- key explanatory sequence
- interactive demos
- reflection
- central idea
- resources
- next/previous navigation

### G. Reflection and Closure

Every session should end with:
- a reflection block
- a central idea block
- a curated resources list
- previous/next session nav

Purpose:
- reflection consolidates learning
- the central idea compresses the session into one memorable takeaway
- resources extend learning without cluttering the body

Non-negotiable closing conventions:
- the heading must be exactly `### La idea central de esta sesión`
- the summary block must use the `central-idea` class
- the resources heading must be exactly `### Recursos para explorar más sobre el tema`
- the resources block must use the `resource-list` class

These four items should be standardized across all sessions even if the inner text and links change.

## Visual Language

### Typography

Session 1 uses a clear typography hierarchy:
- body: readable and friendly
- headings: geometric and assertive
- occasional serif or display accents for emphasis

Effect:
- body text feels accessible
- headings feel intentional and course-like
- emphasis moments feel special without turning gimmicky

### Color

The visual palette is:
- blue-forward
- light backgrounds
- navy text
- subtle accent tones for block-specific demos

Do:
- use color to group concepts and demo states
- use soft gradients and tinted backgrounds
- preserve strong contrast for text

Do not:
- use flat generic white cards everywhere
- introduce random new palettes per section
- use color only decoratively with no semantic role

### Cards and Surfaces

Session 1 uses several card types, each with a distinct role:
- session banner
- definition card
- demo preview card
- demo live shell
- insight cards
- reflection list
- resource cards/list

Rule:
- every card should have a job
- avoid adding more cards if plain Markdown can do the job better

Important example:
- the 8-student table works better as a plain Quarto table than as another decorative card

### Motion

Motion is present but restrained:
- reveal on scroll
- state changes inside demos
- annotation emphasis

Rule:
- motion should support explanation, not compete with it
- always respect reduced-motion behavior

### Mobile and Tablet Behavior

Session 1 is designed to collapse meaningfully on small screens.

Rules:
- stack columns into a clear reading order
- keep the main concept object first
- move secondary or reference material below
- avoid horizontal dependency between explanation and interaction

Pedagogical rule for small screens:
- the thing students must understand first should appear first

## Content and Pedagogical Patterns to Reuse

### 1. Intro hook with a familiar interface

Session 1 uses a TikTok-like phone mockup next to the opening text.

Pattern to reuse:
- pair opening copy with a concrete visual metaphor from student life

Good fits:
- chat UI
- map UI
- inbox UI
- playlist UI
- robot/game UI

### 2. Definition card after the hook

Definitions should not open the page. They should stabilize language after relevance has been established.

### 2.5. Repeated headers create cohesion

Session 1 now relies more strongly on repeated headers and repeated content transitions. These should be preserved across the course wherever the same structural role exists.

Important repeated headers:
- `## Introducción a la IA`
- `### Introducción`
- `### La idea central de esta sesión`
- `### Recursos para explorar más sobre el tema`

This consistency helps students quickly understand where they are in the learning arc of each session.

### 3. “Key moment” block

This is a signature teaching move.

Pattern:
- compress the core concept into one memorable phrase, formula, or visual

Examples:
- “La IA más simple empieza con una recta”
- “Una red neuronal ajusta pesos”
- “Un prompt no programa, orienta”

Purpose:
- gives students a durable anchor

### 4. Demo shell pattern

This is one of the most reusable structural elements in Session 1.

Every major interactive tends to have:
- `.demo-wrap`
- `.demo-shell`
- `.demo-shell-head`
- preview stage
- live stage
- insights
- footer/status/actions

This pattern should be reused as a course-wide convention.

### 5. “Qué estás viendo / Qué significa”

This explanatory pair is pedagogically excellent and should be preserved.

Purpose:
- separates observation from interpretation
- teaches students how to read models, not just watch them

### 6. Reflection as numbered prompts

The reflection block uses:
- short numbered prompts
- one clear question each
- no over-explaining

Purpose:
- helps students retrieve and connect ideas
- works well in class discussion or written follow-up

## Structural and Stylistic Elements That Should Be Standardized Across All 15 Sessions

These are safe to apply broadly in one pass.

### Safe Batch Updates

- Add the session banner at the top of every session.
- Standardize the page asset block that links session CSS and JS.
- Standardize the opening capsule sequence:
- `## Introducción a la IA`
- video embed or polished placeholder
- the exact complement/disclaimer note using `capsule-complement-note`
- `### Introducción`
- Standardize section rhythm with `---` separators between major phases.
- Use the same interactive shell pattern for demos.
- Add “Qué estás viendo” and “Qué significa” to interactive sections where missing.
- Add the reflection block near the end of each session.
- Add the exact heading `### La idea central de esta sesión` near the end using `central-idea`.
- Add the exact heading `### Recursos para explorar más sobre el tema` using `resource-list`.
- Add the previous/next session navigation footer.
- Maintain consistent wording for time/progress metadata.
- Keep Quarto TOC settings aligned with Session 1.

### Safe Style Updates

- Use the same banner styling.
- Reuse the same card radius and border softness.
- Reuse the same heading and body typography.
- Reuse the same visual hierarchy for demo titles, eyebrows, and copy.
- Reuse the same footer/action layout for demos.
- Reuse the same reflection and resource patterns.

## Elements That Need Manual Review and Should Not Be Mass-Converted Blindly

These require human judgment or session-specific design work.

### Manual Content Review

- Opening hook copy
- Session-specific examples
- Definition language
- Reflection questions
- Central idea wording
- Resource links

### Manual UX Review

- Which sections deserve interactives
- Whether a table should be a plain Markdown table or a custom card
- Whether a concept needs a phone UI, diagram, chart, or simple callout
- Whether a demo should be preview + live, or just one static explanatory object

### Manual Technical Review

- JS demo logic
- session-specific assets
- logos and local image paths
- hidden wrappers like `::: {.content-hidden}`
- raw HTML blocks
- annotation scripts
- autoplay behavior

### Important Pitfall to Avoid

When editing raw HTML inside `.qmd` files:
- always use plain ASCII quotes, never smart quotes
- check that comments are properly closed
- check that ` ```{=html} ` blocks close correctly
- check that `::: ...` blocks close correctly

Several rendering bugs in Session 1 came from markup issues of exactly this kind.

## What to Keep Plain Instead of “Designing More”

A key lesson from Session 1 is that not everything should become a card.

Use plain Markdown when:
- the content is just setup context
- a table is only reference material
- a short list already reads clearly
- extra decoration would distract from the next interactive

Good example:
- the 8-student dataset works better as a simple Quarto table before the regression challenge than as a decorated card inside the interactive

## Recommended Migration Strategy for Sessions 2–15

### Pass 1: Safe structural alignment

Apply these to every session:
- top banner
- stylesheet and JS asset block
- opening capsule sequence:
- `## Introducción a la IA`
- video embed or placeholder
- the exact complement/disclaimer note
- `### Introducción`
- reflection block
- central idea block with exact heading and `central-idea`
- resources block with exact heading and `resource-list`
- session navigation block

### Pass 2: Demo-shell normalization

Where sessions already contain interactives:
- move them into the Session 1 demo-shell structure
- add preview/live split if it makes pedagogical sense
- add the insights pair
- add status/actions footer

### Pass 3: Session-specific visual and pedagogical refinement

Review manually:
- opening hook visual
- strongest “key moment”
- right metaphor for the topic
- where plain text beats extra UI

## Suggested Prompt for Batch Updating the Other Session Files

Use the following prompt as the base instruction for updating `sesion-02.qmd` through `sesion-15.qmd`:

---

Update these session `.qmd` files so they match the UX/UI and pedagogical style of `sesion-01.qmd`.

Goals:
- preserve each session’s actual content and learning objectives
- align the visual structure, pacing, and interaction grammar with Session 1
- standardize what is safe to standardize
- skip or flag anything that requires manual pedagogical judgment

Apply these patterns from `sesion-01.qmd`:
- session banner with block, progress, date, duration, and syllabus link
- session-specific CSS/JS include block
- opening capsule sequence in this order:
- `## Introducción a la IA`
- video embed or polished placeholder
- the exact complement/disclaimer note in `capsule-complement-note`
- `### Introducción`
- strong opening hook before formal definition
- clear content rhythm with separators and section hierarchy
- “key moment” style concept-compression block where appropriate
- demo-shell structure for interactives:
  `.demo-wrap` -> `.demo-shell` -> head -> preview/live -> insights -> footer
- “Qué estás viendo / Qué significa” explanatory pair for interactive sections
- reflection block near the end
- exact heading `### La idea central de esta sesión` using the `central-idea` class
- exact heading `### Recursos para explorar más sobre el tema` using the `resource-list` class
- previous/next session navigation

Do standardize:
- structure
- layout conventions
- visual hierarchy
- recurring UI components
- spacing rhythm
- card language
- footer patterns

Do not blindly standardize:
- examples
- metaphors
- datasets
- logos
- interactive logic
- diagrams whose content needs redesign
- sections intentionally hidden for later sessions

Important implementation rules:
- prefer plain Markdown for simple tables and setup lists
- only use custom cards when they add pedagogical value
- keep mobile stacking logical
- preserve repeated course headers exactly where they serve the same structural role
- preserve the complement/disclaimer note and its `capsule-complement-note` class
- preserve the exact heading `La idea central de esta sesión`
- preserve the `central-idea` class for that block
- preserve the exact heading `Recursos para explorar más sobre el tema`
- preserve the `resource-list` class for that block
- use plain ASCII quotes inside raw HTML
- avoid broken HTML comments and unclosed `:::`
- preserve accessibility labels and reduced-motion behavior

When in doubt:
- choose clarity over decoration
- choose a reusable structure over one-off styling
- choose teaching value over visual novelty

---

## Short Version

If the team only remembers five things from this guide, they should be:

1. Start from a familiar student-world example before defining the concept.
2. Reuse the Session 1 shell structure so every page feels like the same course.
3. Keep interactions explanatory, with “Qué estás viendo / Qué significa.”
4. Do not over-card simple content that can stay plain.
5. Standardize structure in batch, but review metaphors, examples, and demo logic manually.
