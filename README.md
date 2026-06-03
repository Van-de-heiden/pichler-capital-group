# Pichler Capital Group Design System

A restrained, premium design foundation for Pichler Capital Group.

The system is built around a simple principle: capital should feel precise, calm and enduring. The visual language avoids noise, novelty for its own sake and anything that smells faintly of a template. Bordeaux and white form the core; warm neutrals, ink tones and disciplined motion provide the supporting architecture.

## Brand character

Pichler Capital Group should feel:

- confidential, not secretive
- ambitious, not loud
- modern, not trend-chasing
- elevated, not theatrical
- precise, not sterile

In short: the brand should enter the room in a tailored suit, not with a confetti cannon.

## System files

- `brand/colors.md` — colour philosophy, roles and usage rules
- `brand/typography.md` — type hierarchy, pairing logic and practical guidance
- `brand/motion.md` — animation principles, easing, timing and restraint
- `brand/voice.md` — verbal identity, tone, writing rules and examples
- `tokens/colors.json` — machine-readable colour tokens for implementation

## Core palette

The primary palette is Bordeaux and white, supported by near-black ink, warm ivory, soft stone and muted metallic accents.

The hierarchy is deliberate:

1. **Bordeaux** for authority, emphasis and brand ownership.
2. **White / Ivory** for space, confidence and clarity.
3. **Ink / Charcoal** for typography and serious interface surfaces.
4. **Stone / Taupe** for secondary panels and quiet depth.
5. **Muted Gold** only as an accent, never as decoration.

## Design principles

### 1. Restraint is the luxury

Use fewer elements, but give them better proportion, spacing and polish. Empty space is not unused space; it is discretion made visible.

### 2. Motion must feel expensive

Animations should be subtle, smooth and purposeful. Hover states, gentle reveals and refined transitions are welcome. Bouncing, wobbling, spinning and excessive page theatre are not.

### 3. Typography carries authority

Headlines may use an elegant serif to create distinction. Body text should remain highly legible and calm. If a font looks impressive but reads badly, it is ornamental weakness.

### 4. Interfaces should guide, not perform

Buttons, cards, images and navigation should feel alive through spacing, elevation and micro-interaction. The user must never feel that the interface is auditioning for attention.

## Recommended implementation order

1. Import colour tokens from `tokens/colors.json`.
2. Set global background, text, border and brand colours.
3. Establish typography styles for display, heading, body, caption and button text.
4. Add motion tokens and standard transitions to buttons, cards, navigation and image overlays.
5. Review all components against the voice and restraint principles.

## Quote to keep in mind

> “Simplicity is the ultimate sophistication.” — commonly attributed to Leonardo da Vinci

Whether or not every attribution survives historical scrutiny, the principle does. The brand should be simple because it is strong enough not to beg for attention.
