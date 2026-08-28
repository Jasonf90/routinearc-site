# RoutineArc — public pages

The App Store-facing pages for the RoutineArc iPhone app: the privacy policy,
the user guide, and a small support landing page.

These files are **generated, not edited here**. The source of truth lives in
the app's private repository (`lib/privacyContent.ts`, `lib/guideContent.ts`)
— the same modules the app itself renders — and is exported with:

    node scripts/makePublicPages.mjs /path/to/this/repo

Editing the HTML directly means the hosted pages and the in-app screens drift
apart, which is the exact failure this setup exists to prevent. Change the
content modules in the app repo, run its tests, regenerate, commit here.

Published with GitHub Pages. The app's source code is not in this repository,
deliberately.
