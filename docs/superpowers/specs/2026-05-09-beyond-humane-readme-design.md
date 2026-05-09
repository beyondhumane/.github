# Beyond Humane Organization README Design

## Goal

Create a polished GitHub organization profile README for Beyond Humane. The README should act as a compact brand landing page, not a project catalog.

## Brand Direction

Use the approved **Portal Card Compact** direction:

- Centered, dark, premium visual treatment.
- Logo-first presentation using the existing assets.
- Minimal copy and restrained link presentation.
- Monochrome black, white, and silver palette matching the supplied logo assets.

## Content Structure

The README will contain these sections in order:

1. Centered brand card with the Beyond Humane logo.
2. Slogan directly below the logo: `Beyond existence.`
3. Social/contact icon row.
4. Horizontal separator.
5. Brief English description.

## Copy

Description text:

> We develop software and AI agents that help products, processes, and organizations move beyond the conventional.

## Links

Use public organization metadata from GitHub:

- Website: `https://beyondhumane.com`
- GitHub: `https://github.com/beyondhumane`
- X/Twitter: `https://x.com/beyondhumane`
- Email: `mailto:info@beyondhumane.com`

## Assets

Use the existing files in `assets/`:

- `assets/output.png` for the main symbol if the layout benefits from the standalone mark.
- `assets/logo-texturized-white-transparent.png` for the wordmark if it reads better in the profile width.

The implementation should choose the asset combination that keeps the README legible on GitHub desktop and mobile profile views.

## Technical Approach

Create a GitHub organization profile README using Markdown and inline HTML where needed for alignment, imagery, and icon links. Avoid external CSS because GitHub README rendering strips style blocks and many attributes.

Use shields-style badges or simple image icons for the social row, choosing whichever renders reliably in GitHub Markdown while preserving the monochrome visual tone.

## Success Criteria

- README renders cleanly on GitHub organization profile pages.
- Logo and slogan are visually centered and immediately visible.
- Social/contact links are clickable and readable.
- Description is short, English, and aligned with the brand landing goal.
- No placeholder links or unfinished sections remain.

## Out Of Scope

- Repository/project listings.
- Team bios.
- Long mission statement.
- Custom generated SVG or new brand assets unless required for GitHub rendering.
