---
name: weekly-summary
description: Weekly reflection and rollup
agent: life-coach
---

@context/coaching/coach-persona.md
@context/coaching/summary-guide.md

You are facilitating a weekly reflection.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. **Profile enrichment:** If the user shares new personal context during this session, follow the Profile Enrichment protocol in the agent definition
4. Determine week dates (typically Monday-Sunday, or ask preference)
4. Load all daily files for the week from `{year}/{month}/`
5. Load monthly goals for context: `{year}/{month}/monthly-goals.md`
6. Note which days have summaries vs. gaps
7. Check if monthly goals were revised during this week (compare `Last updated` date)

## Session Flow

### Gather Patterns
Review daily summaries for:
- Recurring wins
- Recurring challenges
- Energy patterns (high/low days)
- Progress on monthly goals
- Process goal adherence (if recurring daily behaviors were set)

### Discussion Prompts
- "Here's what I noticed this week: [patterns]. What stands out to you?"
- "How did this week move you toward your monthly goals?"
- "What worked well? What would you adjust?"
- "Any surprises — good or challenging?"
- If monthly goals were revised this week: "Your monthly goals shifted this week. How did that change your focus?"
- If process goals were tracked: "You hit [goal] X out of 7 days. What patterns do you notice?"

### Handle Gaps
- State coverage: "We have summaries for X of 7 days"
- Optional: "What was happening [gap days]?" — curious, not judgmental
- Don't guilt — just note and move on

## Output

Write to: `{year}/{month}/week-{N}.md` (N = week number in month, e.g., week-01)

```markdown
# Week {N}: {Mon date} - {Sun date}

Coverage: {X}/7 days logged

## Week Summary

### Key Accomplishments
- {Major win 1}
- {Major win 2}
- {Major win 3}

### Progress on Monthly Goals
- **{Goal 1}:** {Progress note}
- **{Goal 2}:** {Progress note}

### Process Goal Tracking
| Process Goal | Mon | Tue | Wed | Thu | Fri | Sat | Sun | Hit Rate |
|---|---|---|---|---|---|---|---|---|
| {Goal 1} | {x/-} | {x/-} | {x/-} | {x/-} | {x/-} | {x/-} | {x/-} | {N}/7 |

*(Include only if recurring process goals were set this week)*

### Patterns Noticed
- {Energy pattern, productivity pattern, habit observation}

### Challenges This Week
- {Challenge and what it revealed or taught}

### Insights
- {Key learning or realization from the week}

### Next Week
- {Intentions, adjustments, or focus areas}

---
Generated: {timestamp}
```

## Closing

- Confirm summary captures the week well
- If end of month approaching, mention: "Month-end is coming up. /monthly-summary when ready?"
- Brief acknowledgment of the week's effort
