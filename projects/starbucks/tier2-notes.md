# Tier 2 Notes — Starbucks

The following additions are required in Figma after the token push. They are not included in tokens.json.

## font_primitives — additional weight variable

Add manually under the `font_primitives` collection:

| Token name       | Value | Notes                                      |
| ---------------- | ----- | ------------------------------------------ |
| weight.light     | 300   | Used in UI contexts (nav labels, captions) |

## font_primitives — additional family variables (optional)

If Pike (condensed) or Lander (serif) display moments are in scope for this project, add:

| Token name       | Value              | Notes                                    |
| ---------------- | ------------------ | ---------------------------------------- |
| family.condensed | Neue Haas Grotesk  | Substitute for Pike; use Condensed width |
| family.serif     | —                  | No direct substitute for Lander; decide with designer |

Note: All original Starbucks typefaces (SoDo Sans, Pike, Lander) are proprietary and unavailable in Figma without brand licensing. This project uses Neue Haas Grotesk as the approved substitute throughout.
