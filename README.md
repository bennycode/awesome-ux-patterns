# Awesome UX Patterns [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Shipped interactions worth stealing — macOS and web apps that solved an interaction problem unusually well.

Most design lists collect articles, libraries and design systems. This one collects **working software**, indexed by the pattern it demonstrates. If you are about to build a menu, a search field or a destructive action, start here and look at who already got it right.

Early days — two patterns so far. [Contributions welcome.](#contributing)

## Contents

- [What qualifies](#what-qualifies)
- [Marking and radial menus](#marking-and-radial-menus)
- [Spring-loaded modifiers](#spring-loaded-modifiers)
- [Planned patterns](#planned-patterns)
- [Contributing](#contributing)

## What qualifies

An entry has to be a **real app you can use**, and it has to be here for **one specific interaction**, named.

- ✅ "Figma — drag any number field left/right to scrub the value, no stepper arrows."
- ❌ "Figma — beautiful design tool." (no pattern named)
- ❌ A dribbble shot, a concept video, a component library, a blog post about radial menus.

One app can appear under several patterns. Entries that stop working get removed, not archived.

## Marking and radial menus

A circular menu placed at the cursor, where direction alone selects an item — so experts stop reading it and just flick. Coined by Gordon Kurtenbach (1993); still rare outside 3D tools and games.

- [Tangerine](https://tangerineformac.com/) — tap <kbd>⇧</kbd> mid-drag and a conversion wheel opens around the file; drop to apply. No window, no upload.
- [Autodesk Maya](https://www.autodesk.com/products/maya/overview) — the hotbox: hold <kbd>Space</kbd> and the entire menu system appears under the cursor, chosen by direction.

## Spring-loaded modifiers

A mode that exists only while a key is held — Jef Raskin's "quasimode". Self-revealing state: your hand tells you which mode you are in.

- [Tangerine](https://tangerineformac.com/) — <kbd>⇧</kbd> / <kbd>⌘</kbd> / <kbd>⌃</kbd> pick between convert, tools and file actions during one drag.
- **macOS Finder** — hold <kbd>⌥</kbd> while dragging to copy, <kbd>⌘</kbd> to move, <kbd>⌥⌘</kbd> to alias; the cursor badge updates live.

## Planned patterns

Sections I want to open once there are at least two good examples each:

command palettes · fuzzy launchers · natural-language input · scrubbable values · smart snapping and alignment · undo instead of confirmation · optimistic and local-first UI · peek and preview · keyboard-first navigation · progressive disclosure

Know an app that nails one of these? Open a PR and the section gets created.

## Contributing

Open a PR adding one entry under one pattern, in this shape:

```markdown
- [App name](https://example.com) — the one interaction, in one sentence, concrete enough to copy.
```

New pattern sections are welcome when you have at least two apps that demonstrate them. Keep it to apps people can actually run.

## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/)
