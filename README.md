# literary-letter

`literary-letter` is a writing skill for creating and rewriting literary,
personal Chinese letters. It is designed for emotionally meaningful writing
that should feel specific to one relationship rather than polished,
interchangeable, or obviously AI-generated.

The skill prioritizes emotional accuracy, authentic details, natural language,
and restrained literary expression. It can help with love letters, messages of
longing, comforting notes, thank-you letters, apologies, farewells, and letters
intended to repair a relationship.

## What It Does

`literary-letter` helps an agent:

- Write a new literary and personal Chinese letter.
- Rewrite an existing letter while preserving its facts and emotional intent.
- Adapt the voice and ending to the relationship and purpose of the letter.
- Use real details, visible placeholders, or user-authorized fictional details.
- Ask only as many questions as the requested length and available material
  require.
- Avoid generic poetic language, mechanical quotable lines, and obvious
  outline-based structures.
- Protect relationship boundaries by avoiding emotional pressure, invented
  promises, or unsupported assumptions.

The intended result should feel like a sincere letter written to a particular
person, not a general essay about love, friendship, regret, or loss.

## When to Use It

Use this skill when the user explicitly asks for a letter that is:

- Literary, lyrical, poetic, or emotionally expressive.
- Personal and closely connected to a specific relationship.
- Written in the style defined by this skill's samples.
- A rewrite of an existing personal letter that needs stronger rhythm,
  imagery, clarity, or emotional precision.

Typical use cases include:

- Love letters and confessions
- Letters about missing someone
- Comforting letters
- Thank-you letters
- Apology letters
- Farewell letters
- Relationship-repair letters

Do not trigger the skill only because the user says, "Write me a letter." It is
not intended for ordinary personal correspondence, business email, formal
letters, official documents, or academic writing.

## Core Principles

### The User's Request Comes First

Explicit user instructions override the defaults. This includes requested
length, salutation, format, language, level of literary expression, emotional
position, and ending.

The skill must not silently change the relationship, strengthen a promise,
intensify the emotional position, or alter the purpose of the letter.

### Specificity Before Ornament

Concrete experiences, habits, objects, places, and moments should carry the
emotion. Literary devices are useful only when they make the meaning more
accurate.

A plain but truthful sentence is preferable to a beautiful sentence that could
be sent to anyone.

### Natural Development Instead of an Outline

Letters should develop through memory, association, emotional turns, and
specific moments. The skill avoids thesis-first writing, list-like progression,
and obvious introduction-body-conclusion structures.

It does not begin by announcing the central message and then divide the letter
into supporting points. It also avoids forced summary endings.

### Relationship-Aware Writing

Different letters require different emotional behavior:

- A confession may be intimate and vulnerable without demanding a response.
- A comforting letter should allow sadness instead of forcing optimism.
- A thank-you letter should use specific actions rather than idealizing the
  recipient.
- An apology should acknowledge responsibility and describe concrete change.
- A repair letter should respect silence, refusal, and the need for time.
- A farewell may be restrained or sharp without humiliating or threatening the
  recipient.

## Material Modes

The skill supports three ways of handling personal details.

### Real-Detail Mode

Use only facts confirmed by the user. If essential information is missing, ask
a small number of high-value questions. Unconfirmed experiences, dates,
nicknames, habits, and promises must not be invented.

This is the default mode for sensitive or deeply personal letters.

### Placeholder Mode

Use visible placeholders when the user wants a reusable draft or does not want
to provide private details yet.

Example placeholders:

```text
[nickname]
[shared memory]
[meaningful place]
[specific habit]
```

The surrounding sentence should make each placeholder easy to replace.

### Authorized Fiction Mode

Fictional details may be created only when the user explicitly permits them.
The result should not present invented details as verified personal history.

Sensitive events, harm, trauma, or major commitments should not be invented
unless the user specifically requests them.

## Interview Strategy

The skill does not force every user through an interview. It asks questions
only when real-detail mode lacks enough material for the requested result.

Question volume scales with the target length:

| Target | Typical Question Count |
| --- | --- |
| Short note or a few hundred Chinese characters | Usually none; at most one essential question |
| Standard letter | One to three high-value questions |
| Long letter | Three to six relevant questions when needed |
| Quick draft requested | No interview |

Even for a long letter, no additional questions are needed when the user has
already supplied enough material.

Useful questions focus on information that can meaningfully change the letter:

- Who is the recipient, and what is the current relationship?
- What should the recipient understand after reading?
- What shared experience best represents the relationship?
- What facts must not be wrong?
- What language, implications, or promises should be avoided?

## Writing Workflow

### Creating a New Letter

1. Identify the recipient, purpose, requested length, and material mode.
2. Read the style guide and select an appropriate emotional approach.
3. Gather only enough material to support the requested length.
4. Begin from a concrete moment, present thought, natural greeting, or sensory
   detail.
5. Let memories and feelings develop through association and emotional turns.
6. Revise using the quality checklist before returning the letter.

Default length ranges are suggestions rather than requirements:

| Format | Default Range |
| --- | --- |
| Short note | About 100-350 Chinese characters |
| Standard letter | About 500-1,000 Chinese characters |
| Long letter | About 1,200-2,000 Chinese characters |

When the user requests a different length, follow the user's request.

### Rewriting an Existing Letter

The skill distinguishes between light polishing, structural rewriting, and a
full rewrite. When the user does not specify the desired degree of change, it
uses the least invasive option.

During rewriting, it preserves:

- Confirmed facts
- The writer's emotional position
- The purpose of the letter
- Relationship boundaries
- Strong original passages
- The writer's recognizable voice

It improves rhythm, clarity, imagery, emotional precision, and structure
without inventing new facts or increasing the level of commitment.

### Using the Included Samples

The samples define one possible literary-letter style. They do not represent
the current user's personal writing style and are not treated as perfect
outputs.

Samples are read only when the user explicitly requests this skill's sample
style. The agent selects one or two samples that best match the current
emotional purpose and borrows only useful qualities such as rhythm, texture,
and emotional movement.

Each sample includes notes explaining what can be learned and what should not
be copied.

## Prompt Examples

Create a short real-detail letter:

```text
Use $literary-letter to write a restrained 250-character Chinese note to my
partner. Mention the umbrella they left at my apartment and how quiet the room
felt afterward. Do not make up other shared memories.
```

Create a draft with placeholders:

```text
Use $literary-letter to draft a 700-character apology letter. Use placeholders
for the nickname, the argument, and the change I plan to make.
```

Allow fictional details:

```text
Use $literary-letter to write a fictional farewell letter between two people
who met in a coastal town. Keep it restrained and avoid a dramatic reunion.
```

Rewrite while preserving the original voice:

```text
Use $literary-letter to lightly rewrite the following letter. Keep all facts,
the uncertain tone, and the final sentence. Remove generic poetic phrases and
improve the rhythm.
```

Request a quick draft:

```text
Use $literary-letter to write a quick 1,000-character thank-you letter from the
details below. Do not ask follow-up questions.
```

## Output Behavior

By default, the skill returns only the completed letter. It adds explanations,
change notes, or multiple versions only when requested.

Salutations, signatures, dates, and formatting follow the user's instructions.
The skill does not require every letter to begin with `亲爱的X`, and it does not
force a confession, poetic image, or grand conclusion at the end.

## Quality and Safety Checks

Before returning a letter, the skill checks that:

- User instructions and the selected material mode were followed.
- Real details were not invented.
- Placeholders are visible and replaceable.
- Fiction was explicitly authorized.
- The structure does not resemble an essay outline.
- The language sounds directed toward the recipient.
- Imagery supports rather than replaces the meaning.
- The letter avoids emotional blackmail, forced forgiveness, demands for a
  reply, threats, and unsupported promises.
- A rewrite preserves the original facts, intent, and relationship boundaries.

## Project Structure

```text
literary-letter/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
└── references/
    ├── interview-guide.md
    ├── quality-checklist.md
    ├── samples.md
    └── style-guide.md
```

### File Responsibilities

- `SKILL.md`: Trigger conditions, priorities, core workflows, and output rules.
- `references/interview-guide.md`: Question strategy and material modes.
- `references/style-guide.md`: Voice, structure, imagery, and relationship-aware
  style guidance.
- `references/quality-checklist.md`: Final revision and boundary checks.
- `references/samples.md`: Annotated examples of the sample-defined style.
- `agents/openai.yaml`: User-facing skill metadata.
- `README.md`: Human-facing project documentation; it is not part of the
  skill's runtime instructions.

## Customization

To adapt the skill for a different writing style:

1. Update `references/samples.md` with clearly labeled examples.
2. Explain both the useful qualities and the weaknesses of each sample.
3. Adjust `references/style-guide.md` only when the new style requires a
   consistent rule.
4. Keep detailed examples out of `SKILL.md` so the core runtime instructions
   remain concise.
5. Update `agents/openai.yaml` if the user-facing name or description changes.

Do not describe a sample-defined style as the user's personal style unless the
user has provided their own writing samples.

## Design Notes

The skill uses progressive disclosure. `SKILL.md` contains only the core
workflow, while detailed interviewing, style, quality, and sample guidance
lives in `references/` and is read only when needed.

This design keeps the runtime context focused, reduces conflicting rules, and
allows the agent to adapt its process to the requested letter instead of
applying one fixed template.
