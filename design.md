# Redwood Relay: Design Spec

Independent growth studio building brands. Portfolio homepage for web.
Vibe: bold, verdant, commercial.

## Colors

| Token | Hex | Use |
|---|---|---|
| Forest 950 | #06150F | Page canvas |
| Forest 900 | #0A2018 | Nav, sections |
| Forest 800 | #123425 | Cards, hover surfaces |
| Moss 600 | #2E5E3A | Gradient start |
| Moss 400 | #5C8A3C | Gradient mid |
| Moss 300 | #8DAA2F | Gradient end |
| Mint 100 | #DDF7E6 | Headlines |
| Mint 300 | #A8CDB5 | Body copy, nav links |
| Lime 400 | #C8F321 | CTA, frame, kicker |
| Lime 300 | #D9FF4D | CTA hover |

Contrast: Mint 100 on Forest 950 and Forest 950 on Lime 400 both pass WCAG AAA.

## Typography

- Headline: Space Grotesk, 700, tight leading (1.0), letter-spacing -0.03em
- Body and UI: Hanken Grotesk, 400/500/600
- Kicker: Hanken Grotesk, 600, uppercase, 0.14em tracking, lime

| Role | Size |
|---|---|
| Display (4-line headline) | clamp(2.75rem, 7vw, 5.5rem) |
| Body | 1.0625rem, line-height 1.6 |
| Nav / button | 0.9375rem |
| Kicker | 0.8125rem |

## Spacing

4px base: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128.
Page max width 1200px, side gutter 24px (mobile) / 48px (desktop).

## Layout

- Nav bar: logo left, links center or right, "Start a project" button far right
- Hero: two columns on desktop
  - Left: kicker, four-line headline, supporting copy below (lower left)
  - Right: gradient image block with a thin lime frame
- Mobile: single column, gradient block below the copy

## Components

**Nav links**: Mint 300, hover Mint 100 with a 2px lime underline.

**Start a project button**: Lime 400 fill, Forest 950 text, 600 weight, pill radius.
Hover: Lime 300, translateY(-1px). Focus: 2px mint outline, 3px offset.

**Kicker label**: small uppercase lime text, optionally preceded by a 24px lime rule.

**Gradient panel**: 135deg Moss 600 to Moss 400 to Moss 300, radius 24px,
1px lime frame inset 12px from the edge via outline or a pseudo-element.

## Motion

200ms ease-out on color and transform. Respect prefers-reduced-motion.