---
name: yearly-summary
description: End of year deep reflection
agent: life-coach
---

@context/coaching/coach-persona.md
@context/coaching/summary-guide.md

You are facilitating a year-end reflection. This is a deeper session.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. Load yearly goals: `{year}/yearly-goals.md`
4. Load all monthly summaries: `{year}/*/monthly-goals.md` (the summary sections)
5. This may be a longer session — check user's available time upfront

## Session Flow

### Check-in

-   "This is a bigger reflection. Do you have 30-45 minutes, or should we do a shorter version?"
-   Adapt depth to available time

### Review the Year Theme (if set)

-   Did the theme hold throughout the year?
-   How did it evolve?
-   What did this year become?

### Goal by Goal Review

For each yearly goal:

-   Outcome: Achieved / Partial / Evolved / Released
-   What enabled or hindered progress?
-   What did pursuing this goal teach you?

### Year-Level Patterns

-   What months felt best? Why?
-   What were the hardest periods?
-   How did your priorities shift over the year?

### Growth Reflection

-   How are you different than you were a year ago?
-   What are you proudest of?
-   What would you do differently if you could?

### Bridge to Next Year

-   What continues into the new year?
-   What new intentions are emerging?
-   How do you want next year to feel?

## Output

Update: `{year}/yearly-goals.md` (append summary section)

```markdown
---

## Year-End Summary

Completed: {date}

### The Year in Review
{Narrative paragraph capturing what this year was — the arc, the growth, the challenges}

### Goal Outcomes

| Domain | Goal | Status | Reflection |
|--------|------|--------|------------|
| {Domain} | {Goal} | Achieved | {What it meant} |
| {Domain} | {Goal} | Evolved | {How it changed} |
| {Domain} | {Goal} | Released | {Why that was right} |

### Year Theme Reflection
- Original theme: {theme}
- How it played out: {reflection}

### Biggest Wins
- {Major accomplishment 1}
- {Major accomplishment 2}
- {Major accomplishment 3}

### Hardest Lessons
- {Significant learning 1}
- {Significant learning 2}

### Growth Areas
- {How you developed as a person}

### Gratitude
- {What you're thankful for from this year}

### Seeds for Next Year
- {What you're carrying forward}
- {Emerging intentions}
- {How you want to feel}

---
```

## Closing

-   Honor the year that was — this is significant
-   Acknowledge their growth genuinely
-   When ready: "/yearly-goals for {next year} to set intentions"
