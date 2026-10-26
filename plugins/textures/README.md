# Textures for Claude Code

Textures (textures.dev) is a library of hover textures, animated backgrounds and brand textures for websites: fields of bars, dots, dashes or tiles that react to the pointer, each delivered as one self-contained React file with no dependency beyond react. This plugin brings it into Claude Code. It installs the Textures skill, which tells Claude when a Texture fits and how one installs, connects the textures.dev MCP server for searching the catalog and fetching a Texture, and adds the `/textures:texture` command.

## Install

```
/plugin marketplace add Textures-dev/plugins
/plugin install textures@textures
```

## First use

Free Textures work right away: Claude searches the catalog and installs the match with its shadcn command, `npx shadcn@latest add https://textures.dev/r/<slug>.json`. Pro Textures need a Textures account; the MCP server asks you to sign in through OAuth in your browser the first time one is requested. The plugin stores no keys and reads nothing from your machine.

## The command

`/textures:texture <what it is for>`, for example `/textures:texture the hero` or `/textures:texture a calm background behind the pricing cards`. Claude reads https://textures.md, searches for a match, installs the one file and mounts it where you asked, using the file as delivered.

Docs: https://textures.dev/agents · Privacy: https://textures.dev/legal/privacy · Terms: https://textures.dev/legal/terms
