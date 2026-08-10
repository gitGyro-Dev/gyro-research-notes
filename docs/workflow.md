# Research Review Workflow

## Objective

This repository supports a repeatable cycle for developing exploratory ideas while keeping the original reasoning, external critiques, and later revisions traceable.

## Standard cycle

1. **Brainstorm and organize with ChatGPT**
   - Explore the problem conversationally.
   - Keep provisional language provisional.
   - Separate observations, hypotheses, unresolved questions, and tentative definitions.

2. **Create an idea checkpoint**
   - Commit a coherent unit under `ideas/<topic>/`.
   - Prefer dated or clearly versioned Markdown files when the topic evolves over time.
   - The file should state what is provisional and what is currently treated as a working assumption.

3. **Request independent AI reviews**
   - Use `prompts/review_common.md` as the baseline review prompt.
   - Ask at least Claude and Gemini when a checkpoint is important enough to review.
   - Share the GitHub file URL when practical; otherwise provide the exact file contents.

4. **Preserve the critiques**
   - Prefer one GitHub Issue per research theme / review cycle.
   - Add each AI critique as a separate comment, clearly identifying the reviewer and the source checkpoint.
   - Do not silently rewrite critiques before recording them. Editorial notes can be added separately.

5. **Return to the main reasoning loop**
   - Compare critiques rather than accepting any single reviewer as authoritative.
   - Identify agreements, disagreements, possible counterexamples, and terminology debt.
   - Continue the discussion with ChatGPT.

6. **Revise the idea checkpoint**
   - Update or create the next idea file.
   - Preserve meaningful changes in Git history.
   - Repeat the review cycle when the conceptual change is substantial.

## Recommended directory structure

```text
ideas/
  information/
  <future-topic>/

prompts/
  review_common.md

docs/
  workflow.md
```

## Issue convention

Recommended issue title format:

```text
[Review] <topic> — <checkpoint or date>
```

Recommended issue body:

- Source file
- Commit SHA or checkpoint date
- Current working question
- Known provisional terms
- Requested review focus

Each review comment should begin with a reviewer marker such as:

```text
## Claude review
```

or

```text
## Gemini review
```

## Research discipline

- Do not promote brainstorm terminology into Gyro Logic definitions merely because it resembles existing Gyro terminology.
- Similarity to `Slice`, `Stability`, `Trajectory`, `Operator Orientation`, or other Gyro concepts is not evidence of equivalence.
- Prefer counterexamples over additional explanatory diagrams once a candidate concept starts to stabilize.
- Distinguish a concept being established at a particular point from that result being retained, retrievable, or usable later.
- Distinguish time order from establishment order when the distinction matters.
- Keep external theory comparisons as comparison targets, not as automatic mappings.

## Promotion gate

An idea should remain in this repository until there is enough reason to consider formal integration.

Before promotion, at minimum check:

- Is the working definition stable enough to state without repeated caveats?
- Are there known counterexamples or boundary cases?
- Has at least one independent review challenged the idea?
- Is the relationship to existing theories understood well enough to avoid obvious reinvention?
- Is the relationship to existing Gyro concepts explicit rather than assumed?
- Can the original motivating problem still be connected to the developed model?

Passing this gate does not itself change Gyro Logic. It only means the idea is mature enough for a separate integration discussion.
