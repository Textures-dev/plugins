---
description: Find and install a Texture (hover texture, animated background or brand texture) for a place in this project
argument-hint: what it is for, e.g. "the hero" or "a calm background behind the pricing cards"
---
Install a Texture from textures.dev for: $ARGUMENTS

Do it the Textures way, nothing more:

1. Fetch https://textures.md first and read what Textures are and how they install.
2. Search for a match: call the Textures MCP server's `search_textures` with the user's words (this plugin connects it; if it is not connected yet, fetch https://textures.dev/llms.txt and pick from the list).
3. Install the match with its shadcn command, `npx shadcn@latest add https://textures.dev/r/<slug>.json`, or write the one file `get_texture` returns exactly as returned, at the path it names.
4. Mount it inside an element with `position: relative` and a size, where the user asked. Use the installed file as delivered; do not recreate or restyle a Texture by hand.
5. A Pro Texture without access answers with its price and a checkout link: tell the user and stop.

Then say what was installed (its name and page) and where it is mounted.
