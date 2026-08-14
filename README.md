# PindBazaar — web build

Compiled output only. **Source lives in `pindgrid/app-frontend`**; nothing
here is edited by hand.

This repository exists because GitHub Pages cannot be enabled on the source
repo: it is private, and Pages on a private repository needs a paid plan.
Publishing the compiled bundle separately keeps the source private while
giving the app a URL.

Built from **`uat-web-app@80b78cc`** — the UAT reform branch, not `preprod`.
This build carries the restructured supply chain
(Farmer → VLE → Stockist → Transporter → Industry), phone-OTP-first sign-in,
signup ending at OTP with the profile built from home, per-plot land, the
rebuilt machine form and the VLE fleet dashboard.

Rebuild with:

    flutter build web --release --base-href "/pindbazaar-web/"

then copy `build/web/*` over this repo and push. `.nojekyll` must stay —
without it Pages skips the underscore-prefixed files Flutter emits.

Live at https://shubhamdreamworld.github.io/pindbazaar-web/
