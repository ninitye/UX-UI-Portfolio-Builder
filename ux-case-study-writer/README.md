# UX/UI Case Study Writer

A Claude skill that interviews you about a design project, one question at a time, then writes a short, visual, process-first UI case study: hook, section copy, italic captions, a visual shot list and motion briefs. It can also check a set of case studies for consistency.

It is modelled on the structure and voice of three public case studies (OpenAI x Hardware, Notion, Figma at rachelchen.tech/projects). It copies the patterns, not the wording, and is not affiliated with the original author.

## What it does

- Interviews you in a quiz-style form: one small question at a time, with suggested answers and a free-text box
- Handles shipped work and concept or competition work differently
- Writes a one-line hook plus hero visual, then 10 to 14 short sections (600 to 900 words)
- Uses question-form headings, we/I voice rules, and an explored-versus-chosen structure
- Produces a visual shot list and motion briefs (duration, trigger, easing, tool, storyboard template)
- Delivers the case study as a Design artifact in a fixed house style: warm off-white page, slate text, serif headings, mono labels, one narrow column, flat pastel placeholder blocks
- Puts the shot list, motion briefs and gap report on a separate notes board beside the page
- Asks what is confidential and redacts or rebuilds visuals
- Never invents metrics, quotes or outcomes. Gaps become `TODO:` markers
- Runs a portfolio pass across multiple case studies: voice, structure, visuals, range, order, contradictions

## Install

**Claude.ai or Claude desktop**
1. Download `ux-case-study-writer.zip` from this repo (or zip the `ux-case-study-writer` folder yourself).
2. Go to Settings, then Capabilities (or Customize), then Skills, and upload the zip.
3. Turn the skill on.

**Claude Code**
```
mkdir -p ~/.claude/skills
cp -r ux-case-study-writer ~/.claude/skills/
```
For a single project, copy it to `.claude/skills/` inside that project instead.

## Use

Start a chat and say something like:

- "Write a case study for my project using the ux-case-study-writer skill"
- "Run the portfolio pass on these three case studies"

Claude asks one question at a time. Answer by clicking a suggestion or typing your own. Say "I don't know" at any point and it logs a TODO and moves on.

## Customise

Everything lives in `SKILL.md`. Common edits:

- **Voice:** change the "Voice and writing style" section
- **Length:** change the target in "Structure" and the self-review checklist
- **Questions:** edit the "Question sequence" list
- **Reference style:** swap the three reference pages in the intro for your own favourites
- **Page look:** edit the "Visual style" section (colours, fonts, spacing). The skill builds a Design artifact when your Claude account offers one, and falls back to a single HTML artifact otherwise

## Files

```
ux-case-study-writer/
  SKILL.md    the skill
  README.md   this file
```
