# Motion

Motion for Pichler Capital Group must feel deliberate, quiet and precise. It should give the interface life without making it perform like a nightclub website.

The correct impression is: responsive, refined, controlled.

## Motion principles

### 1. Purpose before spectacle

Every animation must clarify an interaction, reveal hierarchy or create polish. If motion exists only because it can, remove it.

### 2. Subtlety over theatre

Hover transitions, soft image movement, refined opacity shifts and slight elevation changes are appropriate. Spinning elements, exaggerated parallax and playful bounces are not.

### 3. Fast enough to feel sharp, slow enough to feel premium

A luxury interface should never feel sluggish. It should feel composed.

## Timing tokens

Use these durations as defaults:

| Token | Duration | Use |
|---|---:|---|
| `motion.duration.fast` | `120ms` | small hover feedback, icon colour changes |
| `motion.duration.base` | `180ms` | buttons, nav states, card transitions |
| `motion.duration.slow` | `280ms` | modals, image overlays, section reveals |
| `motion.duration.luxury` | `420ms` | hero reveals, major page transitions |

Avoid animations longer than `500ms` unless the user is entering a new page or campaign experience.

## Easing tokens

| Token | Value | Character |
|---|---|---|
| `motion.ease.standard` | `cubic-bezier(0.2, 0, 0, 1)` | smooth and reliable |
| `motion.ease.enter` | `cubic-bezier(0.16, 1, 0.3, 1)` | refined entrance |
| `motion.ease.exit` | `cubic-bezier(0.7, 0, 0.84, 0)` | decisive exit |
| `motion.ease.subtle` | `cubic-bezier(0.33, 1, 0.68, 1)` | premium softness |

## Standard interactions

### Buttons

Default button motion:

- background transition: `180ms`
- transform: `translateY(-1px)` on hover
- optional shadow increase on hover
- active state: `translateY(0)`

```css
.button {
  transition:
    background-color 180ms cubic-bezier(0.2, 0, 0, 1),
    border-color 180ms cubic-bezier(0.2, 0, 0, 1),
    color 180ms cubic-bezier(0.2, 0, 0, 1),
    transform 180ms cubic-bezier(0.2, 0, 0, 1),
    box-shadow 180ms cubic-bezier(0.2, 0, 0, 1);
}

.button:hover {
  transform: translateY(-1px);
}

.button:active {
  transform: translateY(0);
}
```

### Cards

Cards may lift slightly on hover. The movement must remain subtle.

- transform: `translateY(-3px)` maximum
- shadow: slightly stronger, never harsh
- image scale: `1.02` maximum

```css
.card {
  transition:
    transform 220ms cubic-bezier(0.2, 0, 0, 1),
    box-shadow 220ms cubic-bezier(0.2, 0, 0, 1),
    border-color 220ms cubic-bezier(0.2, 0, 0, 1);
}

.card:hover {
  transform: translateY(-3px);
}
```

### Images

Large images should feel cinematic but not restless.

Recommended effects:

- slow reveal on page load
- subtle hover scale between `1.015` and `1.03`
- gentle overlay fade
- no aggressive zooms

```css
.image-frame img {
  transition: transform 420ms cubic-bezier(0.16, 1, 0.3, 1);
}

.image-frame:hover img {
  transform: scale(1.02);
}
```

### Navigation

Navigation should communicate state clearly.

Recommended effects:

- colour fade on hover
- thin underline expansion
- active indicator in Bordeaux or muted gold

```css
.nav-link::after {
  content: "";
  display: block;
  width: 0;
  height: 1px;
  background: currentColor;
  transition: width 180ms cubic-bezier(0.2, 0, 0, 1);
}

.nav-link:hover::after,
.nav-link[aria-current="page"]::after {
  width: 100%;
}
```

### Page and section reveals

Use sparingly. Important content may fade and rise gently.

- opacity: `0 → 1`
- translateY: `12px → 0`
- duration: `280–420ms`

Never stagger every tiny element. Staggering is seasoning, not soup.

## Reduced motion

Respect user settings.

```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 1ms !important;
    animation-iteration-count: 1 !important;
    scroll-behavior: auto !important;
    transition-duration: 1ms !important;
  }
}
```

## What to avoid

Avoid:

- bouncy easing
- elastic effects
- infinite decorative motion
- cursor-following gimmicks
- loud parallax
- hover effects that move layout
- animations that delay access to important information

The interface should feel alive, not needy.

## Motion checklist

Before adding motion, ask:

1. Does it clarify what changed?
2. Does it make the interface feel more premium?
3. Is it subtle enough to survive daily use?
4. Does it respect reduced-motion preferences?
5. Would it still feel appropriate in a financial meeting?

If the answer is no, cut it.
