# Typography

Typography is where Pichler Capital Group earns its composure. The brand needs elegance, but not fragility; authority, but not institutional stiffness.

The guiding principle is simple: headlines may impress, body text must serve.

## Recommended font strategy

Use a refined serif for display moments and a highly legible sans-serif for interface and body text.

### Display / Headlines

Recommended options:

- **Cormorant Garamond** — elegant, editorial, classical
- **Playfair Display** — high contrast, luxurious, more dramatic
- **Libre Baskerville** — restrained, credible, less theatrical
- **Fraunces** — distinctive, modern editorial character

Best default recommendation: **Cormorant Garamond** for major headlines.

Use for:

- hero headlines
- campaign titles
- large editorial statements
- premium section titles
- selected brand moments

Avoid using display serif for:

- long paragraphs
- small UI labels
- dense financial tables
- legal text

A noble headline that cannot be read is not noble. It is merely expensive incompetence.

### Body / Interface

Recommended options:

- **Inter** — clean, reliable, excellent UI readability
- **Satoshi** — modern, slightly more distinctive
- **Manrope** — geometric, polished, accessible
- **IBM Plex Sans** — institutional and credible

Best default recommendation: **Inter** for body and UI.

Use for:

- paragraphs
- navigation
- buttons
- forms
- metrics
- cards
- tables
- captions

## Pairing recommendation

Primary pairing:

- Display: `Cormorant Garamond`
- Body/UI: `Inter`

Alternative, more modern:

- Display: `Fraunces`
- Body/UI: `Satoshi`

Alternative, more conservative:

- Display: `Libre Baskerville`
- Body/UI: `IBM Plex Sans`

## Type scale

Use a confident but controlled type scale.

### Display XL

- Size: `72px`
- Line height: `0.95–1.05`
- Letter spacing: `-0.04em`
- Font: display serif
- Use: landing hero, major brand statements

### Display L

- Size: `56px`
- Line height: `1.05`
- Letter spacing: `-0.035em`
- Font: display serif
- Use: page headers, campaign headers

### Heading 1

- Size: `44px`
- Line height: `1.08`
- Letter spacing: `-0.025em`
- Font: display serif or body sans depending on context

### Heading 2

- Size: `32px`
- Line height: `1.15`
- Letter spacing: `-0.015em`
- Font: display serif or body sans

### Heading 3

- Size: `24px`
- Line height: `1.25`
- Letter spacing: `-0.01em`
- Font: body sans, semibold

### Body L

- Size: `18px`
- Line height: `1.65`
- Font: body sans
- Use: important paragraphs, intro copy

### Body M

- Size: `16px`
- Line height: `1.6`
- Font: body sans
- Use: default content

### Body S

- Size: `14px`
- Line height: `1.5`
- Font: body sans
- Use: secondary text, supporting details

### Caption

- Size: `12px`
- Line height: `1.4`
- Letter spacing: `0.04em`
- Text transform: uppercase where appropriate
- Use: labels, small metadata, eyebrow headings

### Button

- Size: `14–15px`
- Line height: `1`
- Weight: `600`
- Letter spacing: `0.01em`
- Font: body sans

## Weight guidance

Use weight carefully.

- Display serif: `400–600`
- Body text: `400`
- Interface emphasis: `500–600`
- Avoid `700+` unless there is a clear reason

Luxury rarely shouts in bold.

## Layout guidance

### Line length

- Paragraphs: aim for `55–75` characters per line.
- Hero text: may be wider, but should not become a wall.
- Financial/legal copy: prioritize scanability with shorter sections.

### Alignment

- Left alignment is the default.
- Center alignment is acceptable for hero sections and short editorial blocks.
- Avoid centered long paragraphs.

### Case

- Use sentence case for most interface copy.
- Use uppercase only for small labels, not large paragraphs.
- Avoid all-caps headlines unless deliberately editorial.

## Example hierarchy

```text
EYEBROW / LABEL
Private capital with disciplined conviction.

Pichler Capital Group
A quiet, precise investment house for serious capital allocation.

We combine entrepreneurial judgment, market awareness and long-term thinking into a visual and verbal system built for trust.
```

## CSS starter

```css
:root {
  --font-display: "Cormorant Garamond", Georgia, serif;
  --font-body: "Inter", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}

.display-xl {
  font-family: var(--font-display);
  font-size: clamp(3.25rem, 8vw, 4.5rem);
  line-height: 1;
  letter-spacing: -0.04em;
  font-weight: 500;
}

.body-m {
  font-family: var(--font-body);
  font-size: 1rem;
  line-height: 1.6;
  font-weight: 400;
}
```
