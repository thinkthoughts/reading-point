# Reading Point Brand Style

## 1. Core mark

The Reading Point mark is an eight-position circular ring.

The eight positions represent the reduced residue classes modulo 30:

`{1, 7, 11, 13, 17, 19, 23, 29}`

These are the residue classes coprime to 30. Every prime greater than 5 occupies one of these classes, while composite integers may occupy them as well.

The logo uses eight equally spaced positions. Their angular spacing is visual geometry and does not encode the numerical spacing between the residue values.

One position may be highlighted to indicate a **reading point**.

## 2. Meaning

The mark follows three semantic rules:

**Geometry identifies Reading Point.**

The ring and its eight positions are the persistent identity.

**Position identifies the reading point.**

A highlighted position indicates the point currently being read, selected, or emphasized.

**Color specifies interface or operational state.**

Brand colors and operational colors have separate roles.

## 3. Brand colors

Reading Point uses a dark-mode and light-mode accent pair.

### Dark mode

* Background: `#050607`
* Foreground: `#FFFFFF`
* Structural gray: `#8F949C`
* Dark structural gray: `#6F747C`
* Reading Point pink: `#D03878`

Pink is the primary Reading Point accent on dark interfaces.

### Light mode

* Background: `#FFFFFF`
* Foreground: `#050607`
* Structural gray: `#8F949C`
* Dark structural gray: `#6F747C`
* Reading Point blue: `#367BF5`

Blue is the primary Reading Point accent on light interfaces.

Pink and blue are equivalent brand accents selected by interface mode. They do not represent different operational states.

## 4. Operational colors

Operational state uses a separate traffic-light system:

* Red: `#E53935`
* Yellow: `#FBC02D`
* Green: `#2EAD62`

These colors communicate operational state rather than brand identity.

Suggested meanings:

* **Red** — stop, constraint, failed requirement, or blocked state
* **Yellow** — caution, unresolved state, intermediate status, or review
* **Green** — supported, admissible, passing, or ready state

Operational colors may appear in either light or dark interfaces.

## 5. Color grammar

Use the following distinction throughout Reading Point artifacts:

`pink / blue → brand`

`red / yellow / green → operational state`

`black / white / gray → structure`

Operational colors should remain semantically meaningful rather than decorative.

## 6. Logo usage

The canonical logo should preserve:

* eight positions
* circular organization
* neutral structural geometry
* a single highlighted reading point where a highlight is used

The standard highlighted point uses the current interface accent:

* pink in dark mode
* blue in light mode

A context may highlight another one of the eight positions. Moving the reading point does not change the identity of the mark.

## 7. Mathematical accuracy

The logo is a reduced representation of the modulo-30 wheel.

It should not imply:

* that the eight classes contain only primes
* that membership in one of the eight classes proves primality
* that equal angular spacing represents the arithmetic distance between residues
* that a highlighted residue has a privileged mathematical status

The mathematical statement represented by the eight positions is:

> The reduced residue system modulo 30 is `{1, 7, 11, 13, 17, 19, 23, 29}`.

## 8. Asset hierarchy

SVG is the canonical format for logo geometry.

Recommended assets:

```text
brand/
├── README.md
├── STYLE.md
├── colors.css
└── logo/
    ├── reading-point-logo.svg
    ├── reading-point-badge-dark.svg
    └── reading-point-badge-dark-512.png
```

Additional light-mode, wordmark, and size-specific assets may be derived from the canonical SVG as needed.

## 9. Implementation

Applications should consume semantic CSS variables rather than hard-code mode-specific colors.

Examples:

```css
--rp-background
--rp-foreground
--rp-structure
--rp-accent
```

The active interface mode determines whether `--rp-accent` resolves to Reading Point blue or Reading Point pink.

This keeps application code separate from the underlying palette and allows the visual system to evolve without changing component semantics.
