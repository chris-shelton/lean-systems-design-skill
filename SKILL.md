---
name: simplify-then-ship
description: "Use this skill when the user wants to simplify, implement, redesign, debug, plan, optimize, or de-risk a system, workflow, codebase, architecture, process, research plan, or technical objective. Apply a first-principles execution loop: challenge requirements, delete parts, simplify what remains, accelerate feedback, then automate only stable work. Especially useful when work feels overcomplicated, slow, brittle, approval-heavy, or prematurely automated."
---

# Simplify Then Ship

Apply this as an operating mode, not a lecture. Drive toward a smaller, clearer system with faster proof.

## Start

1. State the objective in one sentence.
2. Name the constraint that matters most: time, cost, safety, correctness, maintainability, user value, compliance, or learning speed.
3. Sketch the current system as requirements, steps, components, handoffs, assumptions, and feedback loops.
4. If facts are missing, mark them as assumptions and keep moving with the smallest reversible next step.

## Action Loop

Run these passes in order. Do not optimize, automate, or add tooling before deletion and simplification.

### 1. Challenge Requirements

- Attach each requirement to a named source, evidence, and intended outcome.
- Convert fuzzy requirements into measurable success criteria.
- Treat inherited rules, "best practices," and department preferences as hypotheses.
- Ask what fails if the requirement is removed, relaxed, delayed, or scoped to fewer cases.
- Keep only requirements that protect the objective or a real constraint.

### 2. Delete Parts

- List the code paths, process steps, meetings, approvals, interfaces, artifacts, research tasks, or design elements.
- Try to remove each one before improving it.
- Delete "just in case" work unless it has a concrete trigger and owner.
- Prefer fewer states, fewer variants, fewer handoffs, fewer dependencies, and fewer documents.
- If a removed item must return, re-add the smallest version with the reason recorded.

### 3. Simplify What Remains

- Merge duplicate paths and standardize names, interfaces, defaults, and decision rules.
- Collapse handoffs where one owner can carry the work.
- Replace broad abstractions with direct flows when the abstraction is not paying rent.
- Optimize only the remaining critical path.
- Stop polishing anything that should not exist.

### 4. Accelerate Feedback

- Define the fastest safe learn loop: build-measure-learn, read-test-decide, prototype-review, or run-observe-fix.
- Reduce batch size until progress can be validated quickly.
- Parallelize only independent work.
- Add leading indicators that reveal drift before the final outcome fails.
- Prefer reversible experiments over large speculative plans.

### 5. Automate Last

- Automate only stable, frequent, well-understood work.
- Keep humans in the loop where judgment, ambiguity, safety, or low volume dominate.
- Remove redundant in-process checks once end quality is consistently high.
- Keep a manual fallback and a drift signal for every automation.

## Apply By Work Type

- Code: remove unused branches, duplicate state, speculative abstractions, needless dependencies, and slow test loops before tuning.
- Architecture: reduce services, queues, contracts, layers, and cross-team ownership until the data/control flow is obvious.
- Product or design: cut features, modes, settings, and edge-case UI before improving visual polish.
- Process: remove approvals, meetings, status artifacts, and handoffs that do not prevent a named failure.
- Research: narrow the question, delete low-yield sources, test the riskiest assumption first, and stop when the decision is informed enough.

## Output

Return the lean result in the smallest useful format:

- Objective and primary constraint.
- Deletions: what to remove or not do.
- Simplified design: the new minimal path.
- Fastest validation loop: how to learn whether it works.
- Automation candidates: only if the work is stable enough.
- Risks or guardrails: the few that actually matter.

For implementation tasks, make the change after the loop when the path is clear. For planning tasks, produce a ranked action plan with the first reversible step.

## Guardrails

- Do not use this skill to justify reckless cuts to safety, security, compliance, accessibility, data integrity, or user trust.
- Do not delete something merely because it is inconvenient; delete it because its purpose is weak or better served elsewhere.
- Do not replace discovery with bravado. When uncertainty is material, run the smallest test that can collapse it.
- Do not automate ambiguity.
