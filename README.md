# Vadi Claude Plugins

A collection of Claude Code plugins by Vadivel.

## Installation

```bash
# Add the marketplace
claude plugin marketplace add vadivel-designer/vadi-claude-plugins

# Install individual plugins
claude plugin install notification-sound@vadi-claude-plugins
claude plugin install prompt-pro@vadi-claude-plugins
```

## Plugins

### 1. Notification Sound

Plays a sound when Claude Code sends notifications or stops.

**Features:**
- Plays the macOS "Glass" sound on **Notification** events
- Plays the same sound on **Stop** events (when Claude finishes a task)

**Customization:**
Edit `scripts/play-notification.sh` to use a different sound:

```bash
# Available macOS sounds in /System/Library/Sounds/
afplay /System/Library/Sounds/Ping.aiff &
afplay /System/Library/Sounds/Pop.aiff &
afplay /System/Library/Sounds/Purr.aiff &
afplay /System/Library/Sounds/Sosumi.aiff &
```

---

### 2. Prompt Pro

Professional prompt optimizer for Claude with smart question detection and 4-D methodology.

**Commands:**

| Command | Usage | Description |
|---------|-------|-------------|
| `/pp` | `/pp` then paste prompt | Full Prompt Pro experience |
| `/p` | `/p <your prompt>` | Quick inline optimization |

**Workflow:**
```
User Prompt → Smart Question Detection → 4-D Method → Improved Prompt
```

**Features:**
- **Smart Questions** - Only asks clarifying questions when necessary
- **4-D Methodology** - Deconstruct, Diagnose, Develop, Deliver
- **Claude Optimized** - Tailored for Claude's strengths

**Example:**
```bash
/pp
> Write me a marketing email for my SaaS product

# Or quick mode:
/p Help me debug this React component
```

## License

MIT
