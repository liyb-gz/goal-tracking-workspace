---
name: monthly-summary
description: End of month reflection and rollup
agent: life-coach
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

## Session Flow

### Review Monthly Goals
For each goal set at month start:
- What was the outcome?
- Mark status: Achieved / Partial / Revised / Not pursued
- Capture lessons either way — what enabled or hindered?

### Synthesize Weeks
- What themes emerged across the month?
- Energy and capacity patterns?
- What supported progress? What hindered?

### Connect to Yearly Goals
- How did this month advance yearly intentions?
- Any yearly goals that need adjustment or aren't getting attention?

### Look Forward
- What carries into next month?
- Any shifts in priority emerging?
- What would you do differently next month?

## Output

Update: `{year}/{month}/monthly-goals.md` (append summary section)

```markdown
---

## Month-End Summary

Completed: {date}

### Goal Outcomes

| Goal | Status | Reflection |
|------|--------|------------|
| {Goal 1} | Achieved | {What made it work} |
| {Goal 2} | Partial | {What happened, what's left} |
| {Goal 3} | Not pursued | {Why, and is that okay?} |

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

- Acknowledge the month's journey
- If end of year approaching, mention yearly summary
- Suggest: "/monthly-goals to set up next month when ready"
