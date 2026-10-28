# Awesome UX Patterns [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Shipped interactions worth stealing — macOS and web apps that solved an interaction problem unusually well.

Most design lists collect articles, libraries and design systems. This one collects **working software**, indexed by the pattern it demonstrates. If you are about to build a menu, a search field or a destructive action, start here and look at who already got it right.

## Contents

- [What qualifies](#what-qualifies)
- [Marking and radial menus](#marking-and-radial-menus)
- [Spring-loaded modifiers](#spring-loaded-modifiers)
- [Command palettes](#command-palettes)
- [Fuzzy launchers](#fuzzy-launchers)
- [Natural-language input](#natural-language-input)
- [Scrubbable values](#scrubbable-values)
- [Smart snapping and alignment](#smart-snapping-and-alignment)
- [Undo instead of confirmation](#undo-instead-of-confirmation)
- [Optimistic and local-first UI](#optimistic-and-local-first-ui)
- [Peek and preview](#peek-and-preview)
- [Keyboard-first navigation](#keyboard-first-navigation)
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
- [Blender](https://www.blender.org/) — pie menus for mode and shading switches, where muscle memory replaces reading.

## Spring-loaded modifiers

A mode that exists only while a key is held — Jef Raskin's "quasimode". Self-revealing state: your hand tells you which mode you are in.

- **macOS Finder** — hold <kbd>⌥</kbd> while dragging to copy, <kbd>⌘</kbd> to move, <kbd>⌥⌘</kbd> to alias; the cursor badge updates live.
- [Tangerine](https://tangerineformac.com/) — <kbd>⇧</kbd> / <kbd>⌘</kbd> / <kbd>⌃</kbd> pick between convert, tools and file actions during one drag.

## Command palettes

One keystroke, one text field, every command in the app — killing nested menus and the need to memorise shortcuts.

- [VS Code](https://code.visualstudio.com/) — <kbd>⌘⇧P</kbd>, the implementation everyone else copied.
- [Linear](https://linear.app/) — <kbd>⌘K</kbd> is context-aware: the same keystroke offers different verbs depending on what is selected.
- [Raycast](https://www.raycast.com/) — the palette *is* the app; there is no main window to return to.
- [Superhuman](https://superhuman.com/) — <kbd>⌘K</kbd> covers navigation and composition, so the mouse never enters the loop.

## Fuzzy launchers

Match on non-contiguous characters, rank by use, let typing three letters beat any hierarchy.

- [Raycast](https://www.raycast.com/) — scores by what you actually picked last time, so the right result climbs to the top.
- [Alfred](https://www.alfredapp.com/) — the original macOS version of this, with a keyword grammar on top.
- [fzf](https://github.com/junegunn/fzf) — the same pattern in a terminal; pipe anything into it and get interactive filtering.

## Natural-language input

Let people type the sentence they were already thinking, and parse it — instead of five dropdowns.

- [Fantastical](https://flexibits.com/fantastical) — "lunch with Ben tomorrow 1pm at Rosi" fills a whole event, with the parse shown live as you type.
- [Things](https://culturedcode.com/things/) — quick entry parses dates out of the title and strips them from the text.
- [Todoist](https://todoist.com/) — recurrence in plain words ("every 2nd monday"), highlighted inline so you can see what it understood.

## Scrubbable values

Numeric input as a drag target, not a text box with tiny arrows.

- [Figma](https://www.figma.com/) — drag any field label horizontally to scrub; hold a modifier for finer steps.
- [Blender](https://www.blender.org/) — drag across several fields at once to set X, Y and Z in one gesture.

## Smart snapping and alignment

Infer intent from near-alignment, show the guide, snap — so people stop nudging by one pixel.

- [Figma](https://www.figma.com/) — measurement labels appear between objects while dragging, so you see the spacing you are matching.
- **Keynote** — snapping to the centre and to equal gaps between objects, with the yellow guides that made this mainstream.

## Undo instead of confirmation

Stop asking "are you sure?" — do the thing and make it reversible. Faster for the 99% who meant it, and no safer for the 1% who did not.

- **Gmail** — "Undo Send" turned an irreversible action into a 30-second window and removed a confirmation step.
- [Linear](https://linear.app/) — deleting an issue shows a toast with undo rather than a modal.
- [Figma](https://www.figma.com/) — version history means destructive edits never need a dialog.

## Optimistic and local-first UI

Apply the change locally and sync behind the scenes, so the UI never waits on a network round trip.

- [Linear](https://linear.app/) — a local sync engine; everything is instant and conflicts resolve afterwards.
- [Superhuman](https://superhuman.com/) — built around a 100ms budget, which is a UX decision disguised as an engineering one.

## Peek and preview

Look inside something without committing to opening it.

- **macOS Quick Look** — <kbd>Space</kbd> on any selection, in a window that disappears as easily as it appeared.
- [GitHub](https://github.com/) — hovercards on issue, PR and user links give you enough to not break your reading flow.

## Keyboard-first navigation

Treat the keyboard as the primary input and the mouse as the fallback, not the other way round.

- [Superhuman](https://superhuman.com/) — every action is reachable by key; the onboarding exists mainly to teach them.
- [Linear](https://linear.app/) — consistent single-letter verbs across every view.
- [Vimium](https://github.com/philc/vimium) — retrofits link-hinting onto any web page, which is still better than most sites' own keyboard support.

## Contributing

Open a PR adding one entry under one pattern, in this shape:

```markdown
- [App name](https://example.com) — the one interaction, in one sentence, concrete enough to copy.
```

New pattern sections are welcome when you have at least two apps that demonstrate them. Keep it to apps people can actually run.

## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/)
