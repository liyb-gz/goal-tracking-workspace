# Goal Tracking Workspace

An agentic workspace for goal setting and reflection, powered by a supportive AI life coach.

## What This Does

This workspace provides a structured system for:

-   **Goal setting** at yearly, monthly, and daily levels
-   **Reflection summaries** that roll up from daily → weekly → monthly → yearly
-   **Adaptive coaching** that meets you where you are

The AI coach acts as a professional life coach — supportive but not sycophantic, gently corrective when needed, and focused on sustainable, meaningful goals.

## Supported Platforms

-   **Cursor** — Full support with commands, agents, and rules
-   **OpenCode** — Full support with commands and agents

## Getting Started

### 1. Clone or copy this workspace

```bash
git clone https://github.com/YOUR_USERNAME/goal-tracking-workspace.git
cd goal-tracking-workspace
```

### 2. Run onboarding

Open the workspace in Cursor or OpenCode and run:

```
/onboard
```

This will:

-   Ask for your preferences (language, timezone, life domains)
-   Set up your coaching style
-   Create your profile

### 3. Start tracking

| Time           | Command                           |
| -------------- | --------------------------------- |
| Start of year  | `/yearly-goals`                   |
| Start of month | `/monthly-goals`                  |
| Each morning   | `/daily-targets`                  |
| Each evening   | `/daily-summary` or `/end-of-day` |
| End of week    | `/weekly-summary`                 |
| End of month   | `/monthly-summary`                |
| End of year    | `/yearly-summary`                 |

## Commands Reference

| Command            | Description                                              |
| ------------------ | -------------------------------------------------------- |
| `/onboard`         | Initial setup — configure preferences and create profile |
| `/yearly-goals`    | Set or review goals for the year                         |
| `/monthly-goals`   | Set or review goals for the month                        |
| `/daily-targets`   | Set targets for today (or tomorrow)                      |
| `/daily-summary`   | Quick end-of-day reflection (5-10 min)                   |
| `/weekly-summary`  | Weekly reflection and pattern recognition                |
| `/monthly-summary` | End of month reflection and goal review                  |
| `/yearly-summary`  | Deep end-of-year reflection                              |
| `/end-of-day`      | Combined: today's summary + tomorrow's targets           |

## Coaching Methodology

The default coaching style combines:

| Approach             | Purpose                                          |
| -------------------- | ------------------------------------------------ |
| **Domain-balanced**  | Ensures all life areas get attention             |
| **Energy-aware**     | Prevents overcommitment                          |
| **Reflection-heavy** | Connects goals to meaning                        |
| **SMART-lite**       | Specificity where helpful, flexibility where not |

You can customize this during onboarding.

## Life Domains

Choose which areas to track:

-   Health & Energy
-   Career & Work
-   Skills & Learning
-   Finances
-   Relationships
-   Fun & Recreation
-   Environment
-   Contribution
-   Spirituality / Mindfulness
-   Creative Expression
-   (Custom domains welcome)

## File Structure

```
goal-tracking-workspace/
├── .cursor/                    # Cursor configuration
│   ├── agents/life-coach/
│   ├── commands/goals/
│   ├── rules/
│   └── mcp.json
├── .opencode/                  # OpenCode configuration
│   ├── agents/
│   └── commands/goals/
├── context/                    # Shared context files
│   ├── core/                   # Option menus
│   └── coaching/               # Behavior guides
├── profiles/                   # User profiles (created during onboarding)
├── 2026/                       # Goal & summary files (created as you use it)
│   ├── yearly-goals.md
│   ├── 01/
│   │   ├── monthly-goals.md
│   │   ├── week-01.md
│   │   └── 2026-01-15.md
│   └── ...
└── opencode.json
```

## Customization

### Adding Data Source Integrations

The coach can help you set up MCP integrations for automatic data gathering:

```
"I want to add my calendar"
"Help me set up ActivityWatch"
```

Supported (future) integrations:

-   Browser history
-   Calendar events
-   App usage (ActivityWatch)
-   Git commits
-   Fitness data
-   And more

### Modifying Coaching Style

After onboarding, you can adjust anytime:

```
"Update my coaching style to be more SMART-focused"
"I want less reflection, more action-oriented"
```

## Language Support

During onboarding, you can set your preferred language. All sessions, prompts, and summaries will be conducted in that language.

## Philosophy

This workspace is built on these principles:

1. **Supportive, not sycophantic** — Genuine encouragement, not empty praise
2. **Gentle course correction** — Issues are named kindly, not ignored
3. **Gaps are okay** — Missing days aren't failures, they're information
4. **Holistic balance** — All life domains matter, not just productivity
5. **Adaptive depth** — Quick sessions when you're tired, deeper when you have energy

## Contributing

Contributions welcome! Ideas for improvement:

-   New coaching methodologies
-   Additional life domains
-   MCP server integrations
-   Translations of context files

## License

MIT
