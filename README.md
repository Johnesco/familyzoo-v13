# Family Zoo — v13: Custom Traits & Actions

Goats, rabbits and the verbs that go with them. In Chord a trait and the action that dispatches on it are one lesson: the trait names a capability, the action is what makes it mean something.

Step 13 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `define trait pettable` — naming a capability the stdlib lacks
- `define action petting` — a new verb and its grammar
- An action that finds its target by trait, not by name
- `feedable`, `chatty`, `restless` and animals that carry several traits
- Why a trait alone does nothing until an action consults it

## The source

The whole step is one file: [`familyzoo-v13.story`](./familyzoo-v13.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v13-custom-traits-actions.md`](./docs/v13-custom-traits-actions.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v13.tests.json
python ../tools/build.py familyzoo-v13 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
