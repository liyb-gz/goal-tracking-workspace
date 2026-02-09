# Goal Setting Sessions

How to facilitate goal-setting at any level (yearly, monthly, daily).

## Session Flow

### Opening

1. **Check context:** What period are we setting goals for?
2. **Load parent goals:** If monthly, show yearly; if daily, show monthly
3. **Gauge energy:** "How are you feeling about goal-setting today?"

### Exploration (Adaptive)

**If user is vague:**

-   Walk through each active domain
-   Ask about aspirations, challenges, opportunities
-   Help them articulate what "better" looks like

**If user has ideas:**

-   Clarify and refine what they've shared
-   Check alignment with parent goals
-   Probe for gaps in their thinking

### Refinement

For each emerging goal, check:

1. **Clarity** — Is it specific enough to know when it's done? (SMART-lite)
2. **Meaning** — Why does this matter? (Reflection-heavy)
3. **Feasibility** — Is this realistic given current capacity? (Energy-aware)
4. **Balance** — How does this fit with other domains? (Domain-balanced)

Don't enforce rigid SMART format, but ensure goals are actionable and meaningful.

### Prioritization

If multiple goals:

-   Ask which 1-3 are highest priority
-   Suggest sequencing others rather than dropping
-   Flag if load seems unsustainable

### Closing

1. Summarize agreed goals
2. Write to appropriate file (yearly/monthly/daily)
3. Note any open questions or tentative items
4. Express genuine confidence in their capacity (not over-the-top)

---

## Goal Hierarchy

| Session | Load Parent Goals                            |
| ------- | -------------------------------------------- |
| Yearly  | None (top level)                             |
| Monthly | Current yearly goals                         |
| Daily   | Current monthly goals (yearly for reference) |

Reference parent goals to maintain alignment:

> "Your yearly goal is to build financial foundation. How does this month support that?"

---

## By Session Type

### Yearly Goals

-   Big-picture visioning
-   Cover all active domains
-   1-3 primary themes or objectives per priority domain
-   A yearly theme is helpful but optional

### Monthly Goals

-   Derive from yearly goals
-   Specific focus areas for the month
-   Capacity check: What's realistic this month?
-   Account for known events, travel, busy periods

### Daily Targets

-   Concrete actions for today
-   Aligned with monthly goals
-   1-3 meaningful targets, not a huge list
-   Energy-appropriate (morning = more ambitious, evening = less)

---

## Goal Quality Checklist

For each goal, ensure:

-   [ ] Clear enough to know when done
-   [ ] Connected to why it matters
-   [ ] Realistic given current capacity
-   [ ] Balanced with other life areas

Don't enforce rigidly — adapt to user's style.

---

## Goal File Format

Goal files use an Active/Retired structure:

- **Active Goals** section: Current, living goals the user is working toward
- **Retired Goals** section: Table of goals that were achieved, revised, or released — with date and context

When goals change:
1. Move the old goal to the Retired Goals table with status, date, and context
2. Add the new/revised goal to Active Goals
3. If revised, add a brief provenance note: *revised {date}, was: "{old goal}"*
4. Update the `Last updated` date at the top of the file

### Valid Goal Statuses

| Status | Meaning | Where it appears |
|--------|---------|-----------------|
| Active | Currently being pursued | Active Goals section (implicit) |
| Achieved | Completed successfully | Retired Goals table |
| Revised | Changed to something new | Retired Goals table (with → new version) |
| Released | Intentionally let go | Retired Goals table (with reason) |
| Dropped | Abandoned without replacement | Retired Goals table |
| Evolved | Organically transformed (yearly only) | Retired Goals table |

### Cascading Revisions

When yearly goals change, downstream goals may need adjustment:
- `/monthly-goals` checks yearly goals' `Last updated` date and flags if stale
- `/daily-targets` shows monthly goals as context; divergence is noted gently
- Summaries track whether goals were revised during their period

---

## Handling Resistance

If user seems reluctant:

-   Check if timing is off: "Is now a good time for this?"
-   Reduce scope: "What if we just picked one focus?"
-   Name it: "You seem hesitant. What's coming up?"

Don't push. Sometimes the answer is "not today."
