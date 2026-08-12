# Legal

The consent documents MyBI shows at first run, one file each, so a link can point at the licence
without dragging the other two along.

| File | Document |
|---|---|
| [EULA.md](EULA.md) | End User Licence Agreement |
| [Privacy-Policy.md](Privacy-Policy.md) | Privacy Policy |
| [AI.md](AI.md) | AI & Data Use |

Read from 26.1 onwards. Earlier releases read a single `consent.json` here; they no longer find it,
fall back to the copy inside the app and carry on — the fetch was only ever an update check.

## What the app does with these

The text that a user actually agrees to is **bundled in the app**, so first run works offline and the
words accepted are the words reviewed at release. These files are the published mirror: the app
fetches them at boot and, if they differ from what that user last accepted, asks them to read the
terms again. Unreachable means the bundled copy stands and nothing blocks.

Acceptance is recorded as a hash of every document's `id`, `title` and body together, in the order
above. So:

- **Changing any word here re-prompts every user on their next launch.** That is the point of the
  mechanism, and the reason not to commit a typo fix and a policy change in one go.
- **`id` never changes.** It is what ties a published document to the one inside the app.
- **The order above never changes**, and a new document goes on the end.
- **All three must be present.** The app takes the set or none of it, rather than hashing a partial
  set and asking everyone to re-accept terms with a document missing.

## Format

```
---
id: eula
title: End User Licence Agreement
summary: How you may use MyBI.
---

First paragraph.

Second paragraph.
```

`summary` is the one line shown under the title in the document picker, and is optional.

Below the front matter it is plain paragraphs separated by blank lines. A single newline inside a
paragraph is a soft wrap and reads as a space, so these files can be wrapped to a sensible width
here and still arrive in the app as one flowing paragraph. There is no markdown in the body — it is
rendered as read-only text, so headings, lists and emphasis would arrive as literal characters.
