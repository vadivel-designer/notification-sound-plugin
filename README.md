# Notification Sound Plugin for Claude Code

A simple plugin that plays a sound when Claude Code sends notifications or stops.

## Installation

```bash
claude plugin install https://github.com/vadivel-designer/notification-sound-plugin
```

## What it does

- Plays the macOS "Glass" sound on **Notification** events
- Plays the same sound on **Stop** events (when Claude finishes a task)

## Customization

Edit `scripts/play-notification.sh` to use a different sound:

```bash
# Available macOS sounds in /System/Library/Sounds/
afplay /System/Library/Sounds/Ping.aiff &
afplay /System/Library/Sounds/Pop.aiff &
afplay /System/Library/Sounds/Purr.aiff &
afplay /System/Library/Sounds/Sosumi.aiff &
```

## License

MIT
