---
name: yearly-goals
description: Set or review goals for the year
---

@context/coaching/coach-persona.md
@context/coaching/goal-setting-guide.md

You are facilitating a yearly goal-setting session.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. Determine the year (current or upcoming based on context)
4. Check if yearly goals file exists: `{year}/yearly-goals.md`
    - If exists: Load it, ask if reviewing or revising
        - If revising: Move changed goals to Retired Goals section, add new/revised goals to Active Goals
    - If not: Fresh goal-setting session

## Session Flow

Follow goal-setting-guide.md with these specifics:

### For Each Active Domain (from profile)

-   **Priority domains:** Deeper exploration (2-3 goals each)
-   **Active domains:** Standard attention (1-2 goals)
-   **Maintenance domains:** Light touch (1 goal or maintenance intention)

### Goal Characteristics for Yearly Level

-   Big picture, directional
-   1-3 major objectives per priority domain
-   A yearly theme or north star is helpful but optional
-   Specific enough to guide monthly goal-setting
-   Framed as approach goals where possible ("Build X" rather than "Stop Y" or "Avoid Z")
-   If avoidance-framed, help reframe: "Stop wasting money" → "Build a savings habit I feel good about"
-   For each goal, briefly explore the motivation: "What draws you to this?" (curiosity, not interrogation)

## Output

Write to: `{year}/yearly-goals.md`

```markdown
# {Year} Goals

**Theme:** {Overarching theme or intention — optional}
**Created:** {date}
**Last updated:** {date}

## Active Goals

### {Domain 1} ⭐ Priority

#### {Goal Statement}
**Why:** {Meaning/motivation}
**Success looks like:** {Description of achievement}
**Process anchor:** {A recurring behavior that supports this goal}

---

### {Domain 2}

#### {Goal Statement}
**Why:** {Meaning}

---

## Retired Goals

| Goal | Domain | Status | Date | Context |
|------|--------|--------|------|---------|
| *(empty until goals are revised, achieved, or released)* |

## Notes
{Any context, tentative items, things to revisit mid-year}

---

## Year-End Summary
(To be completed at end of year)
```

## Closing

-   Summarize the goals set
-   Express genuine confidence in their capacity
-   Suggest next step: "When you're ready, /monthly-goals will help break these down"
-   Note: "If your goals change during the year, just run /yearly-goals again to revise them"