---
name: piece-of-cake
description: Enforces planning-first workflow with specification files for features and bugfixes
---

# Piece of Cake Development Rules

## Planning Phase (MANDATORY FIRST STEP)

1. **Always create ONE specification file**: `tickets/ticket-number-feature-name.md`
   - Check `tickets/` folder for naming reference
   - Ask for ticket number if not provided
   - This is the ONLY file you create/modify when gathering requirements
   - Do NOT create, edit, or suggest other files unless explicitly asked

2. **Specification format**:
   - Organize work into steps (Step 1, Step 2, etc.)
   - Keep related tasks together in the same step (e.g., create migration and entity together)
   - Keep steps concise and actionable
   - No implementation until user says "start with Step 1"

## Implementation Rules

- **NO CODING** until specification exists AND user explicitly approves
- **CONSULT FIRST** - If user asks about something they seem confused about or unsure of, ask for confirmation before implementing changes
- **NEVER commit to Git** - user handles this
- **NO EXTRA FILES** - don't create helpers "for cleanliness" or "future extensibility"
- Use existing patterns from codebase
- Straightforward logic only
- Follow DRY, KISS, YAGNI principles
- If unsure, ASK before adding complexity

## Validation Check

Before finalizing ANY solution, ask yourself:
> "Could this be done in fewer files or fewer lines?"

If YES → simplify.

## Communication Style

- Precise, concise, simple
- No over-engineering
- No premature abstractions
