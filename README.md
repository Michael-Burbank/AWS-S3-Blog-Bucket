# AWS-S3-Blog-Bucket

┌─────────────────────────────────────────────────────────────┐
│ HEADER (Sticky) │
│ [Logo/Name] Home | About | Progress | Blog | Contact 🌙 │
└─────────────────────────────────────────────────────────────┘

## Color & Component Guidelines

### Palette Variables

Defined in `src/assets/css/style.css`:

```css
--blue: #4fc3f7; /* AWS accent (light) */
--green: #81c784; /* Security+ accent (light) */
--coral: #ff8a65; /* Full Stack accent (light) */
--purple: #7e57c2; /* Brand header */
--deep-purple: #a688da; /* Surface for update cards */
--dark: #263238; /* Base text */
--white: #ffffff; /* Inverse text */
--gray-50: #fafbfc; /* Neutral backgrounds */
--gray-100: #f0f3f5; /* Subtle surface */
--gray-300: #d2d7db; /* Borders */
--focus-ring: #ffca28; /* Accessible focus outline */
```

Light accent backgrounds (blue, green, coral) use dark text for WCAG contrast; darker surfaces (purple, deep-purple, dark) use white text. When adding new accent categories, prefer a light background + dark text or provide a darker variant if you need white text.

### Learning Update Cards (3 Topics)

In `index.html` each daily card uses the structure:

```html
<article class="update-card learning-card">
  <header class="learning-card-header">
    <h3>Day X</h3>
    <span class="learning-date">MMM DD, YYYY</span>
  </header>
  <div class="learning-topics">
    <div class="learning-topic topic-aws">
      <h4>AWS: Title</h4>
      <p>Description.</p>
    </div>
    <div class="learning-topic topic-fullstack">
      <h4>Full Stack: Title</h4>
      <p>Description.</p>
    </div>
    <div class="learning-topic topic-security">
      <h4>Security+: Title</h4>
      <p>Description.</p>
    </div>
  </div>
</article>
```

Add new days by copying an existing card; keep headings short (≤60 chars) and descriptions concise (≤140 chars) for layout stability.

### Accessibility Notes

- Skip link present at top of pages.
- Mobile nav toggle uses `aria-expanded` and is keyboard accessible.
- Focus outlines standardized via `--focus-ring`.
- Contrast: Avoid white text on light accent colors unless you darken the background.

### Future Enhancements (Optional)

- Dark mode via `prefers-color-scheme` media query.
- Extract a JSON data file for learning updates and render cards dynamically with JS.

┌─────────────────────────────────────────────────────────────┐
│ HERO SECTION │
│ [H1] Leveling Up Every Day │
│ [Subtext] Learning AWS, Security+, & Full Stack Dev │
│ [Buttons: View My Progress] [About Me] │
│ [Illustration / Profile Image →] │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ DAILY PROGRESS SECTION │
│ [Title] My Daily Learning Log │
│ [Tabs] All | AWS | Security+ | Full Stack │
│ ┌────────────┬────────────┬────────────┐ │
│ │ Date + Tag │ Date + Tag │ Date + Tag │ ← Progress Cards│
│ │ Title │ Title │ Title │ │
│ │ Excerpt │ Excerpt │ Excerpt │ │
│ └────────────┴────────────┴────────────┘ │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ FEATURED PROJECTS SECTION │
│ [Title] Featured Projects │
│ ┌────────────┬────────────┬────────────┐ │
│ │ Thumbnail │ Thumbnail │ Thumbnail │ │
│ │ Project │ Project │ Project │ │
│ │ Desc + CTA │ Desc + CTA │ Desc + CTA │ │
│ └────────────┴────────────┴────────────┘ │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ ABOUT ME SECTION │
│ [Profile Image ←] Hi, I'm Michael Burbank! |
│ [Short bio paragraph about your journey] │
│ [Resume Button] [Social Links] │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ BLOG SECTION │
│ [Title] Articles & Insights │
│ [Blog Card] [Blog Card] [Blog Card] ... │
│ [Load More ↓] │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ CONTACT SECTION │
│ [Title] Let’s Connect │
│ [Form: Name | Email | Message | Submit] │
│ [Social Icons Row] │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ FOOTER │
│ [Site Name + Tagline] | [Links] | [Social Icons] │
│ © 2025 [Your Name]. All rights reserved. │
└─────────────────────────────────────────────────────────────┘
