# ⚔️ PvP Vote Addon for BedWars1058

An addon for **BedWars1058** that allows players to vote for their preferred PvP combat system before the game starts.

## 📦 Features

- 🗳️ **Voting System**: Players can vote for their preferred PvP mode:
  - 🪓 **Old PvP** – 1.8-style combat with cooldown bypass and critical hits.
  - ⚔️ **New PvP** – Default combat system used in newer Minecraft versions.
- 📋 **Interactive GUI**: Voting menu with sword icons representing each option.
- 🔄 **Seamless Integration**:
  - Works with the [OldCombatMechanics](https://www.spigotmc.org/resources/oldcombatmechanics-disable-1-9-hit-cooldown.19510/) plugin.
  - Automatically enables/disables OldCombatMechanics based on the majority vote result.

## 🛠️ Installation

1. Install [BedWars1058](https://www.spigotmc.org/resources/bedwars1058.75105/).
2. Install [OldCombatMechanics](https://www.spigotmc.org/resources/oldcombatmechanics-disable-1-9-hit-cooldown.19510/) to enable PvP mode switching.
3. Download and place the `.jar` file of this addon into your `/plugins` folder.
4. Restart your server.

## 💬 Commands

| Command     | Description                  |
|-------------|------------------------------|
| `/pvp`      | Opens the PvP voting menu     |
| `/pvp 1`    | Vote for **Old PvP**          |
| `/pvp 2`    | Vote for **New PvP**          |

## 🔧 Requirements

- Minecraft **1.20.4** (Paper)
- Java **17+**
- [BedWars1058](https://www.spigotmc.org/resources/bedwars1058.75105/)
- (Optional) [OldCombatMechanics](https://www.spigotmc.org/resources/oldcombatmechanics-disable-1-9-hit-cooldown.19510/)

### 📄 BedWars1058 Configuration

To show the PvP voting item in the pre-game phase, add the following to your `config.yml` under `pre-game-items`:

```yaml
pre-game-items:
  pvp:
    command: pvp
    material: DIAMOND_SWORD
    data: 0
    enchanted: true
    slot: 6
