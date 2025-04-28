# Minecraft PVP Bot

A Minecraft bot that can automatically engage in PVP combat, guard areas, and defend against hostile mobs using the Mineflayer library.

## Features

- Auto-equips swords and shields when collected
- Guards a specified location
- Automatically attacks hostile mobs
- Engages in PVP combat with players
- Uses pathfinding to navigate efficiently
- Manages armor automatically

## Installation

1. Clone this repository:
   ```bash
   https://github.com/hansajasandeepabadalge/Minecraft-Bot
   cd Minecraft-Bot
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure the bot in [config.js](config.js)

4. Start the bot:
   ```bash
   node index.js
   ```

## Configuration

Edit the [config.js](config.js) file to change the bot settings:

```javascript
const SERVER_CONFIG = {
    host: 'your-server-ip',  // Minecraft server IP
    port: 25565              // Minecraft server port
}

const BOT_CONFIG = {
    username: 'BotName',     // Bot's username
    logErrors: false         // Whether to log errors
}

const GUARD_CONFIG = {
    entityDetectionRange: 16 // Range to detect entities to attack
}
```

## Usage

The bot responds to the following in-game chat commands:

| Command | Description |
|---------|-------------|
| `guard` | Bot will guard your current location and attack hostile mobs |
| `fight me` | Bot will attack you (for practice) |
| `stop` | Bot will stop guarding and attacking |

## Dependencies

- [mineflayer](https://github.com/PrismarineJS/mineflayer) - The core Minecraft bot API
- [mineflayer-pvp](https://github.com/PrismarineJS/mineflayer-pvp) - PVP plugin for combat
- [mineflayer-pathfinder](https://github.com/PrismarineJS/mineflayer-pathfinder) - Navigation and pathfinding
- [mineflayer-armor-manager](https://github.com/PrismarineJS/mineflayer-armor-manager) - Automatic armor management

## Author

- Hansaja Sandeepa
