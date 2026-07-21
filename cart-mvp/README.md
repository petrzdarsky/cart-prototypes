# Notino Cart Prototypes

Living library of cart design prototypes. Browse via [the gallery](./index.html)
(published at your GitHub Pages URL).

## Structure

One folder per project. Each project folder is self-contained (its own HTML
files, no shared build step).

```
/cart-mvp/                    ← baseline cart screen (static + interactive)
    cart-reference.html       ← static 1:1 reference
    cart-interactive.html     ← working prototype (steppers, voucher, recalc)
/gift-wrapping/                ← (example) next project goes here
    ...
index.html                    ← tree/gallery — links to every project
README.md                     ← this file
```

## Workflow — adding a new prototype

1. Create a new folder at the root, named for the feature (e.g. `gift-wrapping/`).
2. Drop its HTML file(s) in that folder. Keep each project self-contained.
3. Open `index.html`, copy one `<li>` project entry, point its link at the new
   folder/file, and give it a short label + one-line description.
4. Commit straight to `main` — no branches needed for solo library work. Only
   branch if you want to protect the live gallery link while a prototype is
   mid-build (see note below).
5. Wait ~1–2 minutes for GitHub Pages to rebuild, then the new entry is live.

## When to use a branch instead

Only when you're actively sharing the current gallery link with someone and
don't want a half-finished prototype to appear. Create a branch, do the work,
merge via pull request when ready. Day-to-day, committing to `main` is fine —
this is a personal library, not a shared codebase.

## Design system

All cart prototypes follow the token set and component recipes in the
`notino-cart-design` skill (tokens, spacing, behavior spec). Keep new
prototypes consistent with it rather than inventing new values.
