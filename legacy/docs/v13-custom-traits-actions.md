# v13 — Custom Traits & Actions

Goats, rabbits and the verbs that go with them. In Chord a trait and the action that dispatches on it are one lesson: the trait names a capability, the action is what makes it mean something.

## What this step adds

- `define trait pettable` — naming a capability the stdlib lacks
- `define action petting` — a new verb and its grammar
- An action that finds its target by trait, not by name
- `feedable`, `chatty`, `restless` and animals that carry several traits
- Why a trait alone does nothing until an action consults it

## The source

The whole step is one file: [`familyzoo-v13.story`](../familyzoo-v13.story). Read it top to bottom — it is the previous step plus what is listed above.

## Running it

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v13.tests.json
```

Chord language reference: <https://sharpee.net/chord/>
