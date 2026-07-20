# Jesus-The True Light Gospel Ministries — build notes

**Type:** Lovable rebuild (CLAUDE.md §0 case B) — not a fresh build, moving the church onto our own domain.

## Brand
- Palette: `gold` generator base (ink/ember/blaze/gold/bone), with `--sky: #7EC8E8` added on top per
  the church's real corporate colours (Gold, Black, White, Sky — from WDF onboarding).
- Sky blue used as a second accent: hero/CTA glow gets an extra top radial in sky, the scroll-progress
  bar sweeps sky → gold → ember, eyebrow icon and favicon swapped from the template's default 🔥 to 🌅
  (fits "Arise, shine, for your light has come" / dawn-light-over-nations theme better than the fire motif).
- Theme/images: "dawn light rising over nations globe open bible".
- Hero: "Arise, shine," / "your light has come." — Isaiah 60:1.

## Real content (from WDF onboarding, not placeholders)
- Service times: Tuesday 17:30 · Friday 17:30 · Sunday 10:00 (times & place section + service list).
- Address: S23/415 Vryburg Stop, Kagung Village, Kuruman, 8446 (times & place section + map embed + footer).
- Pastor's cell: 078 884 7002 (tel: links — CTA "Call the church" + footer).
- Church email: waonepelesi@jesusthetruelight.org (footer mailto:).

## Phase 2 refine (2026-07-20) — real content carried over from Lovable
Source: https://jesusthetruelightofeverynation.lovable.app (screenshots + live HTML fetch — the SSR
markup exposed real asset URLs, so the church's actual logo and photos were downloaded directly rather
than re-generated). Originals kept unmodified in `assets/img/original/`; in-use copies are
`logo.jpg` (nav/footer/hero emblem), `hero.jpg` (hero bg), `mission-bg.jpg` (Mission section bg,
worship hands), `scripture-bg.jpg` (Scripture section bg, open Bible in window light).

- Vision and Mission sections added (new), using the pastor's FULL text as given to WDF — not the
  shortened paraphrase that was live on the Lovable site. "Breaking the walls of divisions" (pastor's
  own plural wording) is now its own heading.
- Ministries section replaced with their real four pillars: Word & Worship, Children & Youth,
  Empowerment, Community Care (exact names + descriptions from the original site).
- Scripture section (pinned/signature moment) now quotes the KJV wording the church actually uses
  ("for thy light is come... is risen upon thee") with their "Rev. 22 · Isaiah 60:1–22" citation,
  instead of the modern-paraphrase placeholder. Hero headline keeps the modern phrasing
  ("Arise, shine, / your light has come.") as directed.
- Old site's WRONG service times (Sunday 9:00, Wednesday 6:30pm) and placeholder email
  (hello@truelightgospel.org) were not carried over — WDF's real data (Tue/Fri 17:30, Sun 10:00;
  waonepelesi@jesusthetruelight.org) stayed in place from the v1 build.
- Ember particle palette swapped one fire tone for sky-blue, so the rising-particle motion reads as
  light rather than fire, matching this church's actual gold/black/sky identity (not a "fire" church).
- Logo now appears live: nav (small circle), footer (small circle), and a slowly-turning emblem in the
  hero (soft radial mask dissolves its white card background into the dark hero, right side, lg+ only).
