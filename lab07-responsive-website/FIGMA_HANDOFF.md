# Figma handoff — Nova

## Frame plan
- `Desktop / 1440` — main full-page design
- `Tablet / 768` — responsive layout
- `Mobile / 375` — single-column layout

## Suggested semantic layer tree
- `Page / Nova Landing`
  - `Navbar` (Auto Layout: horizontal, space-between, padding 32/40, gap 24)
    - `Brand`
    - `NavigationLinks` (horizontal, gap 32)
    - `PrimaryButton`
  - `Main`
    - `HeroSection` (horizontal on desktop, vertical on mobile)
      - `HeroCopy`
      - `HeroArtwork`
    - `IntroBand`
    - `FeatureSection`
      - `SectionHeading`
      - `FeatureGrid` (horizontal desktop; vertical mobile)
        - `FeatureCard / Strategy`
        - `FeatureCard / Design`
        - `FeatureCard / Digital`
    - `StatementSection`
    - `ContactSection` (two columns desktop; one column mobile)
      - `ContactCopy`
      - `ContactForm`
        - `NameField`
        - `EmailField`
        - `ProjectTypeField`
        - `MessageField`
        - `SubmitButton`
  - `Footer`

## Variables / tokens
### Colors
- `color/ink` — #20201F
- `color/paper` — #F8F7F3
- `color/white` — #FFFFFF
- `color/purple` — #8C72E8
- `color/lilac` — #E9E2FF
- `color/peach` — #F8D8C9
- `color/mint` — #D8E9D9
- `color/muted` — #77766F

### Spacing
- `space/1` — 8
- `space/2` — 16
- `space/3` — 24
- `space/4` — 32
- `space/5` — 48
- `space/6` — 72
- `space/7` — 104

### Radius
- `radius/card` — 22
- `radius/pill` — 999

## Auto Layout and resizing
- Apply Auto Layout to every repeated card, button, nav group, and content section.
- Main content wrappers: width Fill container; height Hug contents.
- Cards: width Fill container; height Hug contents; internal vertical Auto Layout.
- Feature grid: horizontal Auto Layout with equal-width cards on desktop; vertical Auto Layout on mobile.
- Buttons: horizontal Auto Layout, center aligned, Hug contents.
- Form fields: vertical Auto Layout; input width Fill container.
- Avoid absolute positioning for content. Decorative artwork can use positioned shapes inside a clipped illustration frame.

## Export
- Mark decorative/icon vectors as SVG export assets.
- Give images descriptive alt text in the implementation.
- Prototype links: navbar anchors scroll to sections; CTA links to Features/Contact; submit button shows a demo confirmation.
