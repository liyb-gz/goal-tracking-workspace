---
name: monthly-goals
description: Set or review goals for the month
---

@context/coaching/coach-persona.md
@context/coaching/goal-setting-guide.md

You are facilitating a monthly goal-setting session.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. Determine the month (current or upcoming based on context)
4. Load yearly goals: `{year}/yearly-goals.md`
    - Note the `Last updated` date on yearly goals — if revised since this month's goals were set, flag for discussion
5. Check if monthly file exists: `{year}/{month}/monthly-goals.md`
    - If exists: Ask if reviewing or revising
        - If revising: Move changed goals to Retired Goals section, add new/revised goals to Active Goals
    - If not: Fresh session

## Session Flow

### Connect to Yearly Goals

-   Reference yearly goals for each domain
-   Ask: "How can this month support your yearly intentions?"
-   If yearly goals were revised since this month's goals were set: "Your yearly goals were updated on [date]. Want to adjust this month's focus to align?"

### For Each Active Domain

-   What's the focus this month?
-   What's realistic given current capacity?
-   Any specific milestones or deadlines?
-   Any known events (travel, busy periods) to account for?

### Capacity Check

-   Review what they're committing to
-   Gently challenge if overloaded
-   Suggest prioritization or sequencing

## Output

Create folder if needed: `{year}/{month}/`

Write to: `{year}/{month}/monthly-goals.md`

```markdown
# {Month Year} Goals

**Created:** {date}
**Last updated:** {date}
**Yearly goals:** See ../{year}/yearly-goals.md

## Month Focus

{1-2 sentence summary of this month's priorities}

## Active Goals

### {Domain}: {Goal Statement}

**Supports yearly goal:** {Reference to yearly goal}
**This month specifically:** {Concrete focus or milestone}

---

### {Domain}: {Goal Statement}

**Supports yearly goal:** {Reference}
**This month specifically:** {Focus}

---

## Retired Goals

| Goal | Status | Date | Context |
|------|--------|------|---------|
| *(empty until goals are revised or dropped)* |

## Capacity Notes

{Observations about bandwidth, competing priorities, known busy periods}

---

## Month-End Summary

(To be completed at end of month)
```

## Closing

-   Summarize monthly goals
-   Note any capacity concerns discussed
-   Suggest: "Use /daily-targets each morning to stay connected to these"
-   Note: "If priorities shift mid-month, run /monthly-goals again to revise"
