# Goal Tracking Workspace

An agentic workspace for goal setting and reflection, powered by a supportive AI life coach.

## What This Does

This workspace provides a structured system for:

- **Goal setting** at yearly, monthly, and daily levels
- **Reflection summaries** that roll up from daily → weekly → monthly → yearly
- **Adaptive coaching** that meets you where you are

The AI coach acts as a professional life coach — supportive but not sycophantic, gently corrective when needed, and focused on sustainable, meaningful goals.

## Supported Platforms

- **Cursor** — Full support with commands, agents, and rules
- **OpenCode** — Full support with commands and agents
- **Other Platforms** - Ask you AI agent to adapt it to your platform!

## Getting Started

### 1. Clone or copy this workspace

```bash
git clone https://github.com/liyb-gz/goal-tracking-workspace.git
cd goal-tracking-workspace
opencode # or cursor .
```

### 2. Run onboarding

Open the workspace in Cursor or OpenCode and run:

```
/onboard
```

This will:

- Ask for your preferences (language, timezone, life domains)
- Set up your coaching style
- Create your profile

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

The coaching approach is grounded in goal-setting research and combines:

| Approach                 | Purpose                                                          |
| ------------------------ | ---------------------------------------------------------------- |
| **Process-goal focused** | Steers toward controllable daily behaviors, not just outcomes    |
| **Domain-balanced**      | Ensures all life areas get attention                             |
| **Energy-aware**         | Prevents overcommitment                                          |
| **Motivation-aware**     | Explores _why_ you pursue goals, not just _what_                 |
| **Reflection-heavy**     | Connects goals to meaning; feedback loops make goal-setting work |
| **Flexibility-first**    | Revising goals is self-awareness, not failure                    |
| **SMART-lite**           | Specificity where helpful, flexibility where not                 |

### Research Foundation

The methodology draws on findings from four key studies:

- **Process goals dramatically outperform outcome goals** for both performance and self-efficacy (Williamson et al., 2022)
- **Goals without feedback don't work** — check-ins and summaries are what make goal-setting effective (Locke & Latham, 2002)
- **Learning goals outperform performance goals** on new/complex tasks where skills are still developing (Locke & Latham, 2002)
- **Approach motivation** (pleasure, growth) predicts better well-being and persistence than avoidance motivation (fear, obligation) (Ehrlich, 2023; Dickson et al., 2021)
- **Goal flexibility predicts well-being**; rigid tenacity does not (Dickson et al., 2021)
- **Short-term goals + long-term direction** outperform either alone (Williamson et al., 2022)

The coach carries these principles internally and surfaces them naturally when relevant — never as a lecture.

Full research notes: `context/coaching/research-notes.md`

You can customize coaching style during onboarding.

## Life Domains

Choose which areas to track:

- Health & Energy
- Career & Work
- Skills & Learning
- Finances
- Relationships
- Fun & Recreation
- Environment
- Contribution
- Spirituality / Mindfulness
- Creative Expression
- (Custom domains welcome)

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
│   ├── core/                   # Option menus (domains, coaching styles)
│   └── coaching/               # Behavior guides
│       ├── coach-persona.md    # Voice, tone, principles
│       ├── goal-setting-guide.md  # Goal session flow + research-backed techniques
│       ├── summary-guide.md    # Reflection sessions + weekly tracker
│       └── research-notes.md   # Research synthesis (4 articles)
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

- Browser history
- Calendar events
- App usage (ActivityWatch)
- Git commits
- Fitness data
- And more

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

1. **Process over outcome** — Focus on controllable daily behaviors, not results you can't control
2. **Supportive, not sycophantic** — Genuine encouragement, not empty praise
3. **Gentle course correction** — Issues are named kindly, not ignored
4. **Gaps are okay** — Missing days aren't failures, they're information
5. **Revision is healthy** — Changing goals is self-awareness, not giving up
6. **Holistic balance** — All life domains matter, not just productivity
7. **Feedback makes it work** — Check-ins and summaries aren't busywork, they're the mechanism
8. **Adaptive depth** — Quick sessions when you're tired, deeper when you have energy

## Contributing

Contributions welcome! Ideas for improvement:

- New coaching methodologies
- Additional life domains
- MCP server integrations
- Translations of context files

## License

MIT
