# ZBR Support Bot

The official Discord support bot for the ZBR scripting language, built entirely with ZBR. This repository serves as a production-ready example of how to build a comprehensive utility and support bot using the ZBR engine.

## Features

This bot provides a powerful pool of support commands to help developers discover and use ZBR functions:

- **Function Discovery**: Search for any ZBR function and get instant details on syntax, arguments, and examples.
- **Categorized Reference**: Browse functions by category (Moderation, Embeds, HTTP, etc.) using interactive buttons.
- **Support Utility**: Quickly find related functions or get a random function to learn something new.
- **Event Triggers**: Reference all available Discord gateway event triggers supported by ZBR.

## Commands

| Trigger | Description |
|---|---|
| `!help` | Shows all available commands. |
| `!find <fn>` | Detailed documentation for a specific function. |
| `!search <query>` | Search functions by name or description. |
| `!category` | Interactive menu to browse functions by category. |
| `!random` | Discover a random ZBR function. |
| `!related <fn>` | Find other functions in the same category. |
| `!triggers` | List all ZBR event triggers. |
| `!stats`  | Statistics about the ZBR language. |
| `!links` | Provide a list of important links related to ZBRLang and ZBR.|

## Quick Start

### Option 1: Webapp Editor (Beta)
Import the [zbr-export-support-bot.zip](/zbr-export-support-bot.zip) into the [ZBR Webapp](https://zbr-webapp.vercel.app) for a visual development experience:
1. Import the project.
2. Manage commands, variables, and settings visually.
3. Export your customized version as a ZIP.
4. Install the CLI, extract your ZIP, and run your bot with `zbr run`.

### Option 2: CLI (Manual)
1. **Prerequisites**
   Ensure you have the [ZBR CLI](https://github.com/zbrlang/zbr) installed:
   ```bash
   npm i -g @zbrlang/zbr -g
   ```

2. **Configuration**
   1. Clone this repository.
   2. Create a `.env` file from the provided `.env.example`.
   3. Fill in your `DISCORD_TOKEN`, `BOT_ID`, and `GUILD_ID`.

3. **Running the Bot**
   Simply run the following command in the project root:
   ```bash
   zbr run
   ```

## Production Ready

This bot is configured with:
- **Hot Reloading**: Changes in `commands/` are applied instantly.
- **Persistent Database**: Uses SQLite for server-specific variable caching.
- **Interaction Handlers**: Seamless pagination and message updates using `Zupdate{}`.

## License

All Rights Reserved. See [LICENSE](LICENSE) for details.

---

Built with ⚡ by [ZBRLang](https://zbrlang.vercel.app)
