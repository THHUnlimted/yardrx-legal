# yardrx-legal

Public legal pages for the YardRx iOS app, served via GitHub Pages.

**Live URLs:**
- Privacy policy: <https://thhunlimted.github.io/yardrx-legal/privacy/>
- Terms of service: <https://thhunlimted.github.io/yardrx-legal/terms/>

These URLs are referenced from `App/Config.swift` in the main YardRx repo
(D161). The org spelling `THHUnlimted` is intentional — single `i` between
T and m.

## Status

⚠️ **DRAFT — not legal-reviewed.** The current content is starter copy
authored to describe what the app actually does (data flows, third-party
processors, retention policy). It has not been reviewed by counsel and
should not be treated as final.

Each page carries a prominent draft banner so visitors and App Store
reviewers see the warning. Replace the banner + tighten the wording
before TestFlight cut.

## Structure

```
.
├── index.html             # landing page with links to both docs
├── privacy/index.html     # served at /privacy/
├── terms/index.html       # served at /terms/
├── style.css              # plain-language styling
└── README.md              # this file
```

Directory-style URLs (`/privacy/`, `/terms/`) ensure the App Store-facing
links resolve cleanly regardless of GitHub Pages' Jekyll permalink
behavior.

## Editing

Plain HTML — no build step. Edit in place, commit, and the GitHub Pages
deployment runs automatically (typically <1 minute).

When you remove the DRAFT banners, also bump the "Last updated" line at
the top of each document.

## Contact

Questions about the documents: see the contact section on each page.
The placeholder address `support@yardrx.app` should be replaced with a
working address before public release.
