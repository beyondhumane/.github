# Beyond Humane README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a compact GitHub organization profile README for Beyond Humane.

**Architecture:** The implementation is a single GitHub-rendered Markdown file using inline HTML for centering, image sizing, and link layout. It reuses the existing assets and external badge/icon services that render reliably in README Markdown.

**Tech Stack:** GitHub Flavored Markdown, inline HTML, existing PNG assets, shields.io badges, GitHub README rendering.

---

## File Structure

- Create: `profile/README.md` - GitHub organization profile README shown on the Beyond Humane organization page.
- Keep: `assets/output.png` - standalone mark available for future use; not required for compact wordmark-first layout.
- Use: `assets/logo-texturized-white-transparent.png` - main centered logo/wordmark.
- Keep: `docs/superpowers/specs/2026-05-09-beyond-humane-readme-design.md` - approved design record.

## Task 1: Create Organization Profile README

**Files:**
- Create: `profile/README.md`

- [ ] **Step 1: Create the GitHub profile README**

Create `profile/README.md` with this complete content:

```markdown
<div align="center">
  <br />
  <img src="../assets/logo-texturized-white-transparent.png" alt="Beyond Humane" width="720" />
  <h3>Beyond existence.</h3>
  <p>
    <a href="https://beyondhumane.com"><img src="https://img.shields.io/badge/Web-beyondhumane.com-f5f5f5?style=for-the-badge&logo=googlechrome&logoColor=111111&labelColor=111111" alt="Website" /></a>
    <a href="https://github.com/beyondhumane"><img src="https://img.shields.io/badge/GitHub-beyondhumane-f5f5f5?style=for-the-badge&logo=github&logoColor=111111&labelColor=111111" alt="GitHub" /></a>
    <a href="https://x.com/beyondhumane"><img src="https://img.shields.io/badge/X-@beyondhumane-f5f5f5?style=for-the-badge&logo=x&logoColor=111111&labelColor=111111" alt="X" /></a>
    <a href="mailto:info@beyondhumane.com"><img src="https://img.shields.io/badge/Email-info@beyondhumane.com-f5f5f5?style=for-the-badge&logo=gmail&logoColor=111111&labelColor=111111" alt="Email" /></a>
  </p>
  <br />
  <hr />
  <br />
  <p>
    We develop software and AI agents that help products, processes, and organizations move beyond the conventional.
  </p>
  <br />
</div>
```

- [ ] **Step 2: Verify required content is present**

Run:

```bash
rg "Beyond existence\.|We develop software and AI agents|beyondhumane.com|github.com/beyondhumane|x.com/beyondhumane|info@beyondhumane.com" profile/README.md
```

Expected: output contains matches for the slogan, description, website, GitHub, X, and email links.

- [ ] **Step 3: Verify referenced local image exists**

Run:

```bash
Test-Path -LiteralPath "assets/logo-texturized-white-transparent.png"
```

Expected: `True`

- [ ] **Step 4: Review working tree**

Run:

```bash
git status --short
```

Expected: `profile/README.md` appears as an untracked or modified file, with existing design/plan docs also present if they have not been committed.

- [ ] **Step 5: Commit if requested by the user**

Only if the user explicitly requests a commit, run:

```bash
git add profile/README.md docs/superpowers/specs/2026-05-09-beyond-humane-readme-design.md docs/superpowers/plans/2026-05-09-beyond-humane-readme.md
git commit -m "docs: add organization profile readme"
```

Expected: commit succeeds and `git status --short` shows no remaining changes from this task except intentionally ignored local brainstorm files.

## Self-Review

- Spec coverage: the task creates the README, uses the logo, places the slogan below it, adds website/GitHub/X/email icon links, adds a separator, and includes the approved English description.
- Placeholder scan: no placeholder URLs, copy, or file paths remain.
- Type consistency: all paths and URLs match the approved design spec and discovered GitHub organization metadata.
