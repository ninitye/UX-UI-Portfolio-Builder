---
name: ux-case-study-writer
description: Write a short, visual UI-showcase case study (hook, copy, captions, shot list, motion briefs) by interviewing the designer first. Also runs a portfolio consistency pass.
---

# UX/UI Case Study Writer

Produces a short, visual, process-first case study for hiring managers and design leads. The focus is a UI showcase: screens, flows, states, components and the decisions behind them. Research is a light supporting beat, not the centrepiece. The style is modelled on three public reference case studies (OpenAI x Hardware, Notion, Figma at rachelchen.tech/projects/). Reproduce the patterns, never the wording of those pages.

## Workflow

1. **Classify the project**: shipped work or concept/competition work (see Project types).
2. **Interview** (see Interview). Do not draft before the required inputs are in.
3. **Confidentiality check.** Ask what is shareable. If anything is under NDA, plan blurred, rebuilt or abstract visuals instead of raw screens.
4. **Gap report.** List missing material (no rejected ideas, no visuals, no outcome). Ask for it. Never invent facts, quotes, numbers or outcomes. If the designer can't supply something, write a clearly marked `TODO:` placeholder and move on.
5. **Draft** the hook, then each section (see Structure), each with copy, an italic caption and a visual spec.
6. **Motion pass.** Add motion briefs where motion explains better than a still (see Motion).
7. **Self-review** against the checklist at the end, fix, then hand back.
8. **Portfolio pass** when more than one case study exists (see Portfolio pass).

## Interview

The interview guides the designer to a strong case study one small step at a time, like a quiz.

### Rules

- **One question at a time.** Ask a single question, then stop and wait. Never send a batch or a numbered list of questions.
- **Ask in the input form.** Use the question picker (AskUserQuestion) for every question. Give 2 to 4 suggested answers plus the free-text "Other" so the designer can click or type. Use multi-select when the answer is "all that apply". If the picker is unavailable, ask in plain text with the same options listed.
- **Put everything the designer needs inside the question.** The form may be the only thing on their screen. When a question includes a draft, a quote or earlier answers, write them inside the question text itself, never in a message above it.
- **One fact per question.** If a question has an "and" in it, split it. Ask for a date, then a person, then a role, not all together.
- **Simple words.** Short sentence, no jargon, plain English. Put a concrete example in the option descriptions.
- **Label first.** Give each question a short header (for example "Timeline").
- **Build suggested answers from the project.** Base options on what the designer has already said and on the domain. Never present an option as fact. Accept "all of them", a number (for example "4") or a short typed answer and log it exactly.
- **Draft the hard ones.** When a question is hard to answer from scratch (the one-sentence problem, the reframe, a trade-off), write a draft from the earlier answers and ask the designer to approve, shorten or reshape it. A draft is built only from what they said. Never add facts they didn't give.
- **Reuse answers.** Skip anything already answered, and use earlier answers to sharpen the next question.
- **Follow up once.** If an answer is thin or vague, ask one follow-up on that point before moving on.
- **Never block.** If they don't know, log a `TODO:` and continue.
- **Show progress.** After each phase, give one line on what you've captured and name the next phase.
- **If the designer interrupts or declines a question**, stop and wait for their instruction. Do not re-ask the same question.

### Question sequence

**Phase A: Setup**
1. **Project type:** Is this shipped work or a concept?
2. **Confidentiality:** How much of this can you show publicly?
3. **Assets:** Which do you already have: final screens, the old version, sketches or rejected options, a prototype or recording?

**Phase B: Frame**
4. **Timeline:** When did the project start, and when did it ship? (Ranges first, exact dates if they want.)
5. **Team:** Who worked on it? (Roles are enough.)
6. **Collaborator roles:** What did each of them do? Ask one role per question.
7. **Your role:** What was your job on this project, in one sentence?
8. **Your work:** What did you personally design and ship?

**Phase C: Problem**
9. **User moment:** Who is the user, and in what moment do they need this? (One real situation.)
10. **What goes wrong:** In that moment, what goes wrong today?
11. **Before:** What did people do before this existed? (Workarounds, other tools.)
12. **Problem sentence:** Draft one sentence from the answers above, inside the question, and ask the designer to correct it. This becomes the Problem section.

**Phase D: Opportunity**
13. **Alternatives:** What else could have solved this, and why wasn't it enough? (Name the obvious alternatives for the domain.)
14. **Reframe:** Draft the reframe in one line, inside the question, and ask the designer to correct it. This becomes the Opportunity section.

**Phase E: Flow and states**
15. **First step:** What is the first thing the user does?
16. **Next moments:** Then what happens? Ask one moment at a time (what the user sees and does, what the product does), repeating until the flow is told. Aim for 4 to 6 moments.
17. **Uncertain or failed state:** What happens when the product can't give a good answer or gets it wrong?
18. **Hero moment:** Which single moment would make the best hero visual?

**Phase F: Constraints (shipped work)**
19. **Biggest limit:** What limited the design most? (Technical limits, accuracy, speed, safety or policy, team capacity.)
20. **Change:** How did that limit change the design?

**Phase G: Exploration** (repeat for at least two options, one option at a time)
21. **Option:** What was another approach you explored?
22. **Why it lost:** Why didn't you choose it?
23. **Trade-off:** Draft the trade-off as "X versus Y", inside the question, and ask the designer to correct it.

**Phase H: Decisions** (repeat for 2 to 4 decisions, one at a time)
24. **Decision:** What is one decision that shaped the final design?
25. **Before:** What did it replace?
26. **Reason:** Why did you make it? What did you give up?

**Phase I: Outcome**
27. **Shipped:** What shipped, and in what form?
28. **Proof:** Is there any real result you can share? (A number, a launch, adoption, a teammate's comment.) "No" is a fine answer.
29. **User signal:** Did any quick feedback or research change a decision? One or two sentences is enough.

**Phase J: Reflection**
30. **Lesson one:** What is one honest lesson from this project?
31. **Lesson two:** What is a second one?

After question 31, give a short recap of what you've collected, list the gaps as TODOs, and ask whether to start drafting.

## Project types

**Shipped work**
- Say what shipped and in what form. Use first-person "I designed and shipped..." for the designer's own work.
- Include an Engineering x Design section on constraints and iteration, with a real product screenshot.
- Outcome is what shipped or changed. Real numbers only. Otherwise a qualitative proof point (a launch, adoption signal, quote from a teammate if the designer supplies it).

**Concept or competition work** (modelled on the Figma page)
- State the sprint frame up front: team size, number of days, the brief or prompt. This is context, not a metric.
- Lead each section with the question the brief raised, then answer it.
- Show the explored-versus-chosen structure heavily. With little time, the rejected ideas are the evidence of rigour.
- Name the prototyping tools used (for example Lottielab, ProtoPie, Figma) as part of the process.
- Say plainly that it is a concept. Never imply it shipped.
- Outcome is the result of the event (a win, who it was presented to) if true. Otherwise a short statement of what the concept proved.
- Skip the Engineering x Design section unless engineers were actually involved.

## Opening hook

Place a hook directly under the header block, before the Overview:

- One line stating the outcome or the sharpest result, in plain words. Examples of shape (not wording): what was built, for whom, in how long, or what it won or shipped as.
- Followed by a hero visual: the final UI, a device render, or a short looping motion clip.
- The hook must be true and supportable. No invented numbers or claims. If there is no outcome to state, hook with the project's premise or the central design tension instead.
- Keep it under 20 words and in the same plain confident voice as the rest.

## Voice and writing style

- **Person.** "We" for team process and decisions. "I" for the role section, work the designer personally did or shipped, and the reflection.
- **Tense.** Past for what was done ("we explored", "we landed on"). Present for how the final design behaves ("the feature does...").
- **Sentences.** Short and declarative. Occasionally one longer explanatory sentence. One idea per sentence. Body text is one or two short paragraphs per section, rarely more.
- **Tone.** Confident, plain, lightly conversational. Mild informality is fine. No hype, no sales language, no stock AI words.
- **Jargon.** Product and design vocabulary is fine for this audience. Explain a term only when it is specific to the project's domain.
- **Numbers.** Process-first. Use only real, shareable numbers (team size, timeline, adoption, a result). Never fabricate or estimate metrics. When there are none, credibility comes from visible reasoning, rejected options and visuals.
- **Trade-offs.** State the priority behind each exploration in a repeated pattern: X versus Y (speed versus structure, clarity versus execution).
- Avoid em dashes, not-X-but-Y contrasts, forced triads, one-line dramatic closers, and bold-label filler.

## Headings

- Pair a small label (Problem, Solution, Exploration, Decision) with a larger H2.
- Prefer H2s written as the question the section answers ("How do we...?"), followed by a plain answer.
- Problem headings state the flaw directly. Solution headings are short and punchy and may start with "Solution:". Rejected options start with "Exploration:".
- Use paired headings (a claim, then a turn) for the overview when the product is strong but has a flaw.
- Number parts of a solution (01, 02, 03) and use arrows for before-to-after.

## Structure

Target 10-14 sections, 600-900 words total. Each section is: heading, one short text block, one visual, one italic caption. Skip or merge sections the project doesn't need.

1. **Header block.** Breadcrumb, title, collaborators, timeline, scope. Optional jump-link contents.
2. **Hook.** One line plus hero visual.
3. **Overview.** A question or claim H2, two or three lines of context. Optionally three labelled process steps.
4. **My role.** One short first-person paragraph. Optionally a summary diagram.
5. **Problem.** Stated plainly, one visual.
6. **Opportunity.** The reframe, as a question plus an answer.
7. **Exploration.** Several options, each with a one-line description, its priority trade-off, and a sketch or screenshot. Show rejected ideas next to the chosen one.
8. **Decisions.** Two to four numbered decisions, each a before-to-after pair with the rationale.
9. **Solution.** The final UI in present tense, in numbered parts, each captioned. Show key states, not only the happy path.
10. **Constraints and iteration** (shipped work). Engineering, hardware, privacy or policy limits and how the design changed.
11. **Outcome.** What shipped, won or was learned.
12. **Reflection.** Two bold, short takeaways in first person, then contact links.

Overall arc: problem, opportunity, exploration, decision, solution, constraints, reflection.

## Visual vs text

- Visuals carry the argument. Text only orients and labels. If a paragraph runs past about 60 words, split it or replace it with a diagram.
- One visual per section is the default. Image-heavy sections are decisions, solution and constraints.
- Reuse the same device mockups across sections for continuity.
- **Captions.** Italic, directly under the image, restating the heading as a label ("Problem: ...", "Solution: ...", "Creating" versus "Reviewing"). A reader skimming only images and captions should still follow the story.
- Number and sequence visuals so the order is obvious.

### Graphic types and when to use each

| Type | Use for |
|---|---|
| SVG diagram | Abstract ideas: formulas, system maps, problem framing, designer's role, scale of ideas, before-to-after decisions |
| Product screenshot or mockup | Real surfaces: solution, outcome, engineering constraints |
| Phone mockup | Mobile flows, states side by side (Creating versus Reviewing) |
| Sketch or low-fi | Explored options. Low fidelity signals exploration |
| Carousel or slides | Numbered problem questions or multi-step concepts |
| Animated GIF or video | Workflows, interaction, anything that changes over time |

For every visual, the shot list must say: what it shows, which claim it proves, the format, and the caption. Flag any visual the designer has not supplied as `TODO: visual needed`.

## Motion graphics (invite the writer to add them)

After drafting, always run a motion pass and suggest where motion would beat a still. Good candidates: the hero visual, a workflow that happens over time, a before-to-after transformation, a state change, a gesture or navigation pattern, a system diagram that builds step by step, and an onboarding flow.

For each candidate give a **motion brief**:

- Section and the claim the motion proves
- Duration (usually 3-8 s), loop or play once, trigger (autoplay muted loop, on scroll, on hover)
- What moves, in order, and what stays still
- Easing and pacing, in plain words (quick in, soft settle)
- Caption, in the same italic style
- Tool: Figma prototyping or Figma motion for UI transitions, Lottielab or Rive for vector and interactive loops, ProtoPie for gesture and logic prototypes, After Effects for polished explainers, a screen recording converted to GIF or MP4 for shipped product behaviour
- Output format and size target (short muted MP4 or WebM preferred over heavy GIF)

Offer a **storyboard and spec template** when the designer wants to build it:

```
Frame | Time | On screen | Motion | Easing | Caption
1     | 0.0s |           |        |        |
```

Keep motion purposeful. Never add motion for decoration. A case study should still read correctly with motion off.

## Confidentiality

Ask before drafting. If anything is confidential, use rebuilt or simplified UI, blurred or abstracted data, or diagrams in place of raw screens, and keep company-internal names, numbers and roadmap items out of copy and captions.

## Portfolio pass

Run when the designer has two or more case studies, or asks for a portfolio check. Ask for the links or text, then compare and report:

- **Voice and tense.** Same we/I rules, same tense rules, same tone across all pages.
- **Structure.** Same section order, header block, hook, reflection format. Flag deliberate exceptions (for example concept work skipping the engineering section).
- **Heading and caption patterns.** Same label pairs, question-form H2s, italic captions.
- **Visual language.** Consistent mockup style, diagram style, colour, device frames and motion style.
- **Length and density.** Pages within a similar word count, one visual per section.
- **Range and balance.** Does the set show breadth (shipped and concept, mobile and web, different problem types)? Flag duplicates or gaps.
- **Ordering.** Suggest an order that puts the strongest, most relevant case study first and varies the types.
- **Claims check.** No claim appears in one page that another page contradicts (role, dates, team sizes).

Output a short table: page, issue, fix. Then a recommended order. Do not rewrite pages in this pass unless asked.

## Deliverables

1. Hook plus section-by-section copy with headings, body and italic captions
2. Visual shot list (what, which claim, format, caption, TODOs)
3. Motion briefs, plus a storyboard if requested
4. Gap report of anything missing or unverified
5. Self-review result
6. Portfolio pass table, when applicable

## Delivery: always a Design artifact with the page layout

Always deliver the case study as a Design artifact that shows the finished page, copy and layout together. Do not deliver it as a Doc, a plain file or a pasted block of text.

1. Call the Artifact tool's `list_types` first. When a Design type is listed, create the case study from it and follow the instructions it returns. If no Design type is listed, build one self-contained HTML page and publish it as an artifact instead. Say in one line which route was used.
2. Create it only once the interview and the draft are done, so the page is built from real copy.
3. Put the case study page in the artifact exactly as a visitor would see it, with the real copy, headings, italic captions and a placed frame for every visual.
4. Put the shot list, motion briefs, gap report and self-review on a separate notes board or page after the case study, clearly outside the page itself.
5. Keep the chat reply to one or two lines and do not paste the copy.
6. To revise, edit the same artifact. Never start a second one.

### Page layout

Every case study artifact uses the same house style, taken from the reference pages (rachelchen.tech/projects/). Apply it every time. Do not run the Design type's design-system lookup and do not ask about colours or fonts. Use a different look only when the designer explicitly asks for one in that request.

#### Visual style

- **Feel.** Quiet, editorial and typography-led. Warm off-white page, lots of whitespace, one narrow centred column, flat image blocks. No shadows, no borders, no cards, no gradients, no emoji. Only phone frames get rounded corners (20 px).
- **Colour tokens.**
  - Page background `#F6F5F3` (optional very faint grain).
  - Text slate `#32404F`.
  - Muted text, captions and section labels `#5F6973` (the reference uses about 55% slate, which fails contrast, so use this solid value).
  - Hairline dividers `rgba(50,64,79,0.14)`.
  - Mono label teal `#2F5F69`.
  - Text on pastel blocks `#234850`.
  - TODO chip: background `#F3EAC9`, text `#6B5A14`.
  - Pastel visual blocks: lavender `#D9CCE3`, sage `#D3E3D8`, sand `#E9DFCC`, blush `#EFD6D2`, sky `#D2E2EC`. Use neutral grey `#E4E2DE` for "before" frames. Rotate the pastels and never use more than one per block.
- **Type.** Load from Google Fonts in the artboard's helmet: Libre Baskerville (400, 700, italic 400), DM Mono (400) and Inter (400, 500). Inter stands in for the reference's licensed sans.
  - H1: Libre Baskerville 400, 32 px, line-height 1.15, letter-spacing -0.64 px.
  - H2: 28 px, line-height 1.2, letter-spacing -0.56 px.
  - H3: 18 px, line-height 1.4, letter-spacing -0.36 px.
  - Body: Inter 15 px, line-height 1.5, muted colour for paragraphs and slate for values.
  - Section label: Inter 15 px, muted, directly above the H2 (Overview, Problem, Solution).
  - Mono labels: DM Mono 12 px, uppercase, letter-spacing 0.04 em, teal, for image labels, numbers (01, 02) and category tags.
  - Captions: italic 14 px, muted, 10 px under the visual.
  - Reflection takeaways: Libre Baskerville 700, 24 px, each between hairlines.
- **Page structure.**
  - Top bar: left-aligned breadcrumb in 13 px ("← Work / Project title"), 16 px 24 px padding.
  - Content column: max width 740 px, centred, 24 px side padding.
  - Header block: H1, then a metadata row of Collaborators, Timeline and Scope as three wrapping columns, muted label above slate values.
  - A hairline, then the hook as a 28 px serif line, then the hero up to 988 px wide.
  - Every later section starts 96 px below the previous one with label, H2, body, visual and caption.
  - Overview process steps are three columns, each with a top hairline and a mono number.
  - Exploration cards sit side by side, each with a placeholder, a mono "Exploration" tag, an H3, the trade-off and a caption.
  - Decisions are separated by hairlines, each with a mono number, H3, text, a before-and-after pair (16 px gap) and a caption.
  - Solution parts form a two-column grid, each with a top hairline, mono number, H3 and one line. A horizontal state strip of phone frames follows, each with a mono label.
  - Reflection is two bold serif lines between hairlines.
- **Placeholders.** A missing visual is a pastel block at the right size with a centred mono uppercase label saying what it must show, and a TODO chip. Every TODO fact uses mono 12 px in the TODO colour. Never fake a screenshot, use stock imagery, or invent UI.
- **Motion.** Clips autoplay muted and loop, with a still poster frame for reduced-motion users. The layout must still read with motion off.
- **Responsive.** Sections wrap to one column on small screens. Pairs stack. The state strip scrolls horizontally.
- **Contrast.** All text meets 4.5:1 against its background.
- **Honesty.** The page carries only facts the designer gave. Unfilled facts stay visible as `TODO` markers until the designer replaces them.

## Self-review checklist

- [ ] Total length is 600-900 words and every section has a visual
- [ ] A one-line hook with a hero visual sits under the header, and is true
- [ ] Each H2 is a question or a short claim, with a label
- [ ] "We" for process, "I" for role, shipped work and reflection
- [ ] Past tense for process, present tense for the final design
- [ ] At least two explored options are shown, including rejected ones, each with a trade-off
- [ ] Decisions are framed as before-to-after
- [ ] Solution shows key states, not just the happy path
- [ ] Concept work is labelled as a concept and not implied to have shipped
- [ ] Captions are italic, sit under the image and restate the claim
- [ ] No invented metrics, quotes or outcomes. Every number is real and shareable
- [ ] Nothing confidential is exposed
- [ ] Motion brief exists for the hero and for every section where time or state matters
- [ ] Reflection is two short bold takeaways
- [ ] No AI tells: em dashes, not-X-but-Y contrasts, forced triads, hype, filler
- [ ] A skimmer reading only headings, images and captions gets the whole story
- [ ] Delivered as one Design artifact (or HTML artifact if no Design type is listed), not a Doc or pasted text
- [ ] The page uses the house style: off-white `#F6F5F3` background, slate `#32404F` text, Libre Baskerville headings, DM Mono labels, Inter body, 740 px column, flat pastel blocks with no shadows or cards
- [ ] Every missing visual is a labelled `TODO` placeholder block, with no faked screens
- [ ] Notes (shot list, motion briefs, gap report) sit outside the page itself
