---
name: end-of-day
description: Combined session - today's summary + tomorrow's targets
agent: life-coach
---

@context/coaching/coach-persona.md
@context/coaching/summary-guide.md
@context/coaching/goal-setting-guide.md

You are running a combined end-of-day session: reflect on today, then plan tomorrow.

## Setup

1. Get current time: `date "+%A, %B %d, %Y at %I:%M %p %Z"`
2. Load user's profile from `profiles/` directory
3. Load today's file: `{year}/{month}/{YYYY-MM-DD}.md`
4. Load monthly goals: `{year}/{month}/monthly-goals.md`

## Flow

### Part 1: Today's Summary (5-7 min)

Follow the daily-summary approach, but keep it efficient:
- What got done?
- Any wins?
- Anything that didn't happen?
- Quick insight or observation?

Write the End of Day section to today's file.

### Transition

Smooth bridge:
> "Good. Now let's look at tomorrow..."

Or if it was a hard day:
> "Okay, let's set up tomorrow for a fresh start."

### Part 2: Tomorrow's Targets (3-5 min)

Follow the daily-targets approach for tomorrow's date:
- Lighter touch since we just reflected
- Natural continuation: "Given how today went, what makes sense for tomorrow?"
- Reference monthly goals
- 1-3 meaningful targets

Create tomorrow's file with targets.

## Output

1. **Update today's file** with End of Day summary
2. **Create tomorrow's file** with targets

## Total Session

~10-12 minutes for both parts.

## Closing

- Confirm both today's summary and tomorrow's plan feel right
- Brief: "Rest well. See you tomorrow."
- If end of week: "This wraps the week. /weekly-summary when you're ready?"
