---
name: monthly-summary
description: End of month reflection and rollup
---

@context/coaching/coach-persona.md
@context/coaching/summary-guide.md

You are facilitating an end-of-month reflection.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. Load monthly goals: `{year}/{month}/monthly-goals.md`
4. Load all weekly summaries for the month: `{year}/{month}/week-*.md`
5. Load yearly goals for context: `{year}/yearly-goals.md`
6. Check `Last updated` dates on both monthly and yearly goals — note any mid-period revisions

## Session Flow

### Review Monthly Goals

For each goal set at month start:

-   What was the outcome?
-   Mark status: Achieved / Partial / Revised / Not pursued
-   Capture lessons either way — what enabled or hindered?
-   If goals were revised mid-month, review both active and retired goals
-   For revised goals: What prompted the change? Was the pivot the right call?

### Synthesize Weeks

-   What themes emerged across the month?
-   Energy and capacity patterns?
-   What supported progress? What hindered?

### Handle Gaps

-   Note weekly summary coverage: "We have summaries for X of Y weeks this month"
-   If weeks are missing, note factually and offer to discuss
-   Gaps are information, not failures

### Connect to Yearly Goals

-   How did this month advance yearly intentions?
-   Any yearly goals that need adjustment or aren't getting attention?
-   If yearly goals were revised during this month: "Your yearly goals shifted this month. How did that affect your monthly focus?"

### Look Forward

-   What carries into next month?
-   Any shifts in priority emerging?
-   What would you do differently next month?

## Output

Update: `{year}/{month}/monthly-goals.md` (append summary section)

```markdown
---

## Month-End Summary

Completed: {date}

### Goal Outcomes

| Goal | Status | Date Revised | Reflection |
|------|--------|--------------|------------|
| {Goal 1} | Achieved | — | {What made it work} |
| {Goal 2} | Partial | — | {What happened, what's left} |
| {Goal 3} | Revised | {date} | {What prompted the change} |
| {Goal 4} | Not pursued | — | {Why, and is that okay?} |

### Month Themes
- {Major theme or pattern that emerged}
- {Another observation}

### Biggest Wins
- {Most significant accomplishment}
- {Another meaningful win}

### Challenges
- {What was hard this month}

### Lessons
- {What you learned about yourself or your approach}

### Carrying Forward
- {What continues into next month}
- {Any adjustments to make}

---
```

## Closing

-   Acknowledge the month's journey
-   If end of year approaching, mention yearly summary
-   Suggest: "/monthly-goals to set up next month when ready"
