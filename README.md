# Family Zoo — v13 — Custom Actions

Adds entirely new verbs — feed, photograph, snap — that stdlib does not know about. Walks through the four-phase Action interface and how to teach the parser and language provider about story-specific vocabulary.

Step 13 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- The Action interface with validate, execute, report, and blocked phases
- getCustomActions on the Story class
- extendParser with grammar.define and mapsTo
- extendLanguage for registering message IDs and text
- context.sharedData for passing state between phases

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v13
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v13
python C:/code/ifhub/tools/ship.py familyzoo-v13
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
