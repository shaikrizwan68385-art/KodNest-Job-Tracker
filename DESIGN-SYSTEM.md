# KodNest Premium Build System

Design system for a serious B2C product. Calm, intentional, coherent, confident. One mind designed it.

---

## Design philosophy

- **Calm** — No visual noise. Restful hierarchy.
- **Intentional** — Every element has a purpose. No decoration for its own sake.
- **Coherent** — Same rules everywhere. No drift between screens.
- **Confident** — Clear typography and spacing. No hedging.

**Out of scope:** Flashy, loud, playful, hackathon-style. No gradients, glassmorphism, neon colors, or animation noise.

---

## Color system

Maximum **4 colors** across the entire system.

| Role        | Token            | Value     | Use                    |
|------------|------------------|-----------|------------------------|
| Background | `--color-bg`     | `#F7F6F3` | Page and surface       |
| Primary text | `--color-text` | `#111111` | Body and headings      |
| Accent     | `--color-accent` | `#8B0000` | Primary actions, focus |
| Success    | `--color-success`| `#4A5D4A` | Success, shipped      |
| Warning    | `--color-warning`| `#7A5C0A` | In progress, caution  |

Success and warning are muted and used only for status and feedback.

---

## Typography

- **Headings:** Serif (`Libre Baskerville`). Large, confident, generous spacing. No decorative fonts.
- **Body:** Sans-serif (`Source Sans 3`). 16–18px, line-height 1.6–1.8. Max width **720px** for text blocks.
- **Sizes:** No random sizes. Use design tokens only.

---

## Spacing system

Only these values. Never use arbitrary values (e.g. 13px, 27px).

| Token       | Value |
|------------|-------|
| `--space-1`| 8px   |
| `--space-2`| 16px  |
| `--space-3`| 24px  |
| `--space-4`| 40px  |
| `--space-5`| 64px  |

Whitespace is part of the design. Use the scale consistently.

---

## Global layout structure

Every page follows this order:

1. **Top Bar** — Project name (left), progress (center), status badge (right).
2. **Context Header** — One large serif headline, one-line subtext. Clear purpose. No hype.
3. **Primary Workspace (70%)** — Main product interaction. Clean cards, predictable components.
4. **Secondary Panel (30%)** — Step explanation, copyable prompt box, actions.
5. **Proof Footer** — Persistent checklist. User proof per item.

---

## Top Bar

- **Left:** Project name.
- **Center:** Progress (e.g. “Step 2 / 5”).
- **Right:** Status badge: **Not Started** | **In Progress** | **Shipped**. Same style; color differentiates.

---

## Context Header

- One large serif headline.
- One-line subtext.
- Clear purpose. No marketing or hype language.

---

## Primary Workspace

- 70% width.
- Main product interaction lives here.
- Clean cards, predictable components. No crowding.

---

## Secondary Panel

- 30% width.
- Short step explanation.
- Copyable prompt box.
- Buttons: **Copy**, **Build in Lovable**, **It Worked**, **Error**, **Add Screenshot**.
- Calm styling. No visual competition with the workspace.

---

## Proof Footer

- Persistent bottom section.
- Checklist: □ UI Built □ Logic Working □ Test Passed □ Deployed.
- Each item requires user proof input.

---

## Component rules

- **Primary button:** Solid deep red (`--color-accent`). Secondary: outlined, same radius and hover behavior.
- **Hover and radius:** Same transition and border radius everywhere (`--radius`, `--transition`).
- **Inputs:** Clean borders. No heavy shadows. Clear focus state (accent border + light ring).
- **Cards:** Subtle border. No drop shadows. Padding from spacing scale.

---

## Interaction rules

- **Transitions:** 150–200ms, ease-in-out. No bounce, no parallax.

---

## Error and empty states

- **Errors:** Explain what went wrong and how to fix it. Never blame the user.
- **Empty states:** Provide the next action. Never feel dead or abandoned.

---

## File reference

- **Tokens and components:** `kodnest-design-system.css`
- **Showcase:** `index.html` — layout and components only. No product features.

Use the same classes and tokens everywhere. No visual drift.
