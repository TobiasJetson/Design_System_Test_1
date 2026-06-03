# Jetson Air — Components

Connected repository: https://github.com/TobiasJetson/Design_System_Test_1

Before using any component, read all referenced token files in the connected GitHub repository. Treat token values as the authoritative source of truth. Never substitute, assume, or approximate a token value.

---

## Card

### Definition
A card is a container that groups related content. In a feed context, cards can communicate a state within a sequence of other cards.

### Purpose
- Present content and actions related to a single topic
- Enable effortless scanning of pertinent and actionable information
- Communicate hierarchy through deliberate arrangement of text, images, and actions

---

### Placement
- Cards can appear in a grid, vertical list, or carousel
- Can be positioned at the top, middle, or bottom of a screen
- Always pair with a heading when placed as a section

---

### Interaction
Cards are either static or clickable. Clickable cards support the following optional states:

| State | When to use |
|---|---|
| Default | Resting state |
| Hovered | Cursor over card (desktop) |
| Focused | Keyboard or assistive navigation |
| Pressed | Active tap or click |
| Selected | Card chosen within a selection context |

Cards may optionally include:
- Action buttons
- Links within supporting text
- A dismiss icon to remove the card from view
- Footer accessories that promote interaction (large card variant only)

---

### Accessibility
- Long text or accessibly scaled text may wrap to 2 lines maximum
- Clickable cards must have a clearly defined focus state
- Dismiss controls must have an accessible label

---

### Default Tokens

All token values below are mandatory for the default card state unless explicitly overridden by a variant.

| Property | Token | Reference file |
|---|---|---|
| Width | `315px` | — |
| Height | `435px` | — |
| Corner radius | `xl` | `Corner_Radii.tokens.json` |
| Body fill | `App_Off White` from `App Colours` | `Colours.tokens.json` |
| Shadow | `Level 5 Shadow` | `Shadows.tokens.json` |
| Border width | `m` | `Borders.tokens.json` |
| Border colour | `App_Soft Gray` from `App Colours` | `Colours.tokens.json` |

---

### Rules
- Do not mix colour tokens from outside the `App Colours` collection
- Do not override corner radius unless building a named card variant
- Shadow and border must always appear together in the default state — never one without the other
- Do not invent new card sizes — use the default or a named variant

---

*Additional card variants (e.g. compact, large, promo) will be added here as they are defined.*
