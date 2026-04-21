> Official release page for ApexUtility — a lightweight staff utility built for modern Paper/Spigot environments.

# ApexUtility v1.0
by NathanFCS

ApexUtility is a lightweight staff utility script for Paper/Spigot servers using Skript.

Built for server teams that want essential moderation tools in one clean and reliable resource.

---

## Overview

ApexUtility combines several core staff utilities into one simple Skript project:

- Timed freeze system
- Inventory viewer
- Vanish toggle
- Personal and global chat tools

This project is designed for server owners who prefer lightweight utility scripts over larger plugin stacks.

---

## Requirements

- Paper or Spigot **1.19+**
- Skript **2.8+**

---

## Installation

1. Place `ApexUtility.sk` in `plugins/Skript/scripts/`
2. Run `/skript reload ApexUtility`
3. Done

---

## Commands

### Staff Only
Permission node: `apexutility.admin`

| Command | Description |
|---------|-------------|
| `/freeze <player> <duration>` | Freeze a player |
| `/unfreeze <player>` | Unfreeze a player |
| `/inv <player>` | View a player's inventory |
| `/vanish` | Toggle vanish |
| `/clearchat` | Clear chat for everyone |
| `/chatmute` | Toggle global chat mute |

### All Players

| Command | Description |
|---------|-------------|
| `/chatclear` | Clear your own chat |

---

## Duration Format

| Input | Duration |
|-------|----------|
| `30s` | 30 seconds |
| `5m` | 5 minutes |
| `2h` | 2 hours |
| `1d` | 1 day |

### Example

```text
/freeze Steve 10m
/freeze Aaron 1h
/freeze NathanFCS 1d
```

---

## Freeze System

- Frozen players **cannot move or use commands**
- Frozen players **can still chat**
- Freeze **persists through logout/login**
- Freeze **expires automatically** when duration ends
- Staff are notified when a player is frozen or unfrozen
- Frozen players can see who froze them

---

## Vanish System

- Vanished players are **hidden from regular players**
- Staff can **still see** vanished players
- Vanish state is handled correctly when players join

---

## Chat System

- `/chatclear` clears **your own** chat only
- `/clearchat` clears chat **for everyone**
- `/chatmute` prevents non-staff players from sending messages

---

## Changelog

```text
v1.0 - initial release
     - freeze with duration support (s/m/h/d)
     - freeze persists through logout/login
     - automatic unfreeze on expiry
     - inventory viewer
     - vanish with staff visibility
     - personal chat clear
     - global chat clear and chat mute
```

---

## Planned

- [ ] Freeze log to file
- [ ] Discord webhook on freeze event
- [ ] Spy mode for admins
- [ ] Freeze history per player

---

## License

This project is licensed under the **MIT License**.

---

## Notes

- This is a **Skript resource**, not a standalone `.jar` plugin
- Designed for **Paper/Spigot-based servers**
- Lightweight and easy to maintain
- Official links are provided below for safety and authenticity

---

## Official Links

### Profiles
- **GitHub:** https://github.com/NTHFCS
- **SpigotMC Profile:** https://www.spigotmc.org/members/nathanfcs.2521802/
- **skUnity Profile:** https://forums.skunity.com/members/nathanfcs.40131/

### Resource Pages
- **SpigotMC:** https://www.spigotmc.org/resources/apexutility.134427/
- **skUnity:** https://forums.skunity.com/resources/apexutility.1884/

### Community
- **Discord:** https://discord.gg/V8dpGdsMeT
