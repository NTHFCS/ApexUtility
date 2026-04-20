# ApexUtility v1.0
by NathanFCS

Lightweight staff utility script for Paper/Spigot servers.
No dependencies required beyond Skript.

---

## Requirements

- Paper or Spigot 1.19+
- Skript 2.8+

---

## Install

1. Drop `ApexUtility.sk` into `plugins/Skript/scripts/`
2. Run `/skript reload ApexUtility`
3. Done.

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

Example:
```
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
- Staff get notified when a player is frozen/unfrozen
- Frozen player sees who froze them

---

## Vanish System

- Vanished players are **invisible to regular players**
- Staff can **still see** vanished players
- Vanish state **persists through login** (other staff see you correctly)

---

## Chat System

- `/chatclear` — clears **your own** chat only, doesn't affect others
- `/clearchat` — clears chat **for everyone**
- `/chatmute` — prevents non-staff from sending messages

---

## Changelog
```
v1.0 - initial release
     - freeze with duration (s/m/h/d)
     - freeze persists on logout
     - auto unfreeze on expire
     - invsee
     - vanish with staff visibility
     - chatclear (personal)
     - clearchat + chatmute (admin)
```
---

## Planned

- [ ] Freeze log to file
- [ ] Discord webhook on freeze event
- [ ] Spy mode for admins
- [ ] Freeze history per player

---

## Issues / Suggestions

Post in the discussion section on SpigotMC or Modrinth.