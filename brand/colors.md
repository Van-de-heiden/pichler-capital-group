# Colours

Pichler Capital Group uses colour as a signal of authority, discretion and financial seriousness. The palette should not look like a fintech toybox. It should feel institutional, private and quietly modern.

## Primary colours

### Bordeaux

**Token:** `brand.bordeaux.700`  
**Hex:** `#5A0F1B`

Bordeaux is the signature colour. Use it for brand moments, primary buttons, key highlights, selected navigation states and premium visual anchors.

It should not flood the interface. Bordeaux is most powerful when it appears with discipline.

Recommended use:

- primary CTA backgrounds
- active navigation states
- important progress or ownership indicators
- selected cards or premium feature accents
- editorial dividers and small signature details

Avoid:

- full-page red-heavy layouts
- large blocks with weak contrast
- using Bordeaux for every clickable element
- pairing it with loud colours that cheapen the atmosphere

## Foundation colours

### White

**Token:** `base.white`  
**Hex:** `#FFFFFF`

White is the main spatial colour. It creates clarity, confidence and room for large imagery.

Use for:

- primary backgrounds
- cards
- content surfaces
- clean sections

### Ivory

**Token:** `base.ivory`  
**Hex:** `#F8F5EF`

Ivory brings warmth and keeps the brand from feeling clinical.

Use for:

- alternate page sections
- editorial blocks
- subtle panels
- premium content backgrounds

### Ink

**Token:** `neutral.ink`  
**Hex:** `#151417`

Ink is the primary text colour. It has more elegance than pure black and avoids the harshness of `#000000`.

Use for:

- main text
- headlines on light backgrounds
- navigation labels
- serious interface copy

### Charcoal

**Token:** `neutral.charcoal`  
**Hex:** `#262126`

Charcoal is a dark surface colour. It works well for premium footer areas, dark sections and high-contrast cards.

Use for:

- dark panels
- footer background
- overlays on large images
- secondary dark buttons

## Supporting neutrals

### Stone

**Token:** `neutral.stone`  
**Hex:** `#D8D2C8`

Stone is used for borders, muted backgrounds and understated divisions.

### Taupe

**Token:** `neutral.taupe`  
**Hex:** `#A99D90`

Taupe is a restrained secondary neutral. Use sparingly for muted text, icons and subtle labels.

### Mist

**Token:** `neutral.mist`  
**Hex:** `#EEEAE3`

Mist is ideal for background differentiation where white would feel too plain and ivory too warm.

## Accent colours

### Muted Gold

**Token:** `accent.gold.500`  
**Hex:** `#B89B5E`

Muted gold is a privilege, not a habit. It may support premium cues, small line details and status accents. It must never become ornamental glitter.

Use for:

- small separators
- subtle icons
- refined highlight lines
- premium labels

Avoid:

- gradients that resemble casino interfaces
- large gold buttons
- excessive metallic effects

### Profit Green

**Token:** `semantic.positive`  
**Hex:** `#2F6B4F`

Use only for positive financial indicators, confirmations and performance metrics.

### Risk Red

**Token:** `semantic.negative`  
**Hex:** `#9C2F3A`

Use for negative states, warnings and financial losses. Do not confuse it with brand Bordeaux.

## Suggested usage ratio

A strong Pichler Capital interface should roughly follow this distribution:

- 55–70% white or ivory
- 15–25% ink, charcoal and text tones
- 5–12% stone, mist and borders
- 3–8% Bordeaux
- 1–3% gold or semantic colours

This ratio keeps the brand expensive. Too much Bordeaux becomes heavy. Too much gold becomes insecure. Too much animation becomes a PowerPoint crime scene.

## Contrast rules

- Use `base.white` or `base.ivory` text on Bordeaux buttons.
- Use `neutral.ink` for most body text.
- Use `neutral.taupe` only for secondary text, never for critical information.
- Avoid gold text on ivory unless size and contrast are carefully checked.
- Large imagery should receive dark overlays before white text is placed on top.

## Practical examples

### Primary button

- background: `brand.bordeaux.700`
- text: `base.white`
- hover: `brand.bordeaux.800`
- border: none

### Premium card

- background: `base.white`
- border: `neutral.mist`
- title: `neutral.ink`
- highlight line: `brand.bordeaux.700`
- small accent: `accent.gold.500`

### Dark section

- background: `neutral.charcoal`
- text: `base.ivory`
- muted text: `neutral.stone`
- CTA: `brand.bordeaux.600` or outlined ivory
