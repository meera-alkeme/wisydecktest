<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<title>Wisy — From shelf to HQ</title>
<style>
/* ============================================================
   WISY DESIGN SYSTEM — Foundations
   Source of truth: Brand Style Tile (assets/Brand_Style_Tile.png)
   ============================================================ */

@import url('https://fonts.googleapis.com/css2?family=Figtree:wght@300;400;500;600;700;800&family=Roboto+Mono:wght@400;500;600&display=swap');

:root {
  /* ----------  COLOR — RAW TOKENS  ---------- */

  /* Brand accents */
  --wisy-indigo:      #5354ED;   /* Primary accent — logo, CTAs, links */
  --wisy-lime:        #DDF45B;   /* Secondary accent — highlights, callouts */

  /* Neutrals */
  --wisy-black:       #000000;
  --wisy-gray-500:    #AAAAAA;   /* Mid gray — placeholders, captions */
  --wisy-gray-50:     #F5F5F5;   /* Surface tint — large soft cards */
  --wisy-white:       #FFFFFF;

  /* Indigo tints (the soft lavender family from the tile) */
  --wisy-indigo-200:  #CDD1FF;   /* Strong tint — secondary surfaces */
  --wisy-indigo-100:  #F0F1FF;   /* Wash — section backgrounds, tags */

  /* Derived shades for hover / press / focus (kept inside the indigo hue) */
  --wisy-indigo-700:  #3F3FD5;   /* Hover on primary */
  --wisy-indigo-800:  #2B2BB8;   /* Press on primary */
  --wisy-indigo-300:  #A8AFFF;   /* Soft border / focus ring */
  --wisy-lime-700:    #C5DC3D;   /* Hover on lime */

  /* Semantic helpers (kept neutral; brand favors restraint) */
  --wisy-success:     #1F8A5B;
  --wisy-warning:     #E08A00;
  --wisy-danger:      #D24A3C;

  /* ----------  COLOR — SEMANTIC ROLES  ---------- */

  /* Foreground */
  --fg:               var(--wisy-black);
  --fg-1:             var(--wisy-black);           /* Primary text */
  --fg-2:             #4A4A4A;                     /* Body secondary */
  --fg-3:             var(--wisy-gray-500);        /* Captions, placeholders */
  --fg-on-indigo:     var(--wisy-white);
  --fg-on-lime:       var(--wisy-black);
  --fg-accent:        var(--wisy-indigo);

  /* Background */
  --bg:               var(--wisy-white);
  --bg-1:             var(--wisy-white);           /* Page background */
  --bg-2:             var(--wisy-gray-50);         /* Soft surface — large cards */
  --bg-3:             var(--wisy-indigo-100);      /* Tint surface — callouts */
  --bg-inverse:       var(--wisy-black);
  --bg-accent:        var(--wisy-indigo);
  --bg-accent-soft:   var(--wisy-indigo-100);

  /* Border */
  --border-1:         #E6E6E6;                     /* Default border */
  --border-2:         var(--wisy-indigo-200);      /* Accent border */
  --border-strong:    var(--wisy-black);

  /* ----------  TYPOGRAPHY — FAMILIES  ---------- */
  --font-sans:   "Figtree", ui-sans-serif, system-ui, -apple-system, "Helvetica Neue", Arial, sans-serif;
  --font-mono:   "Roboto Mono", ui-monospace, "SF Mono", Menlo, Consolas, monospace;

  /* ----------  TYPOGRAPHY — SCALE  ---------- */
  /* Display sizes follow the tile: large weight 500/600, very tight leading. */
  --fs-display-xl: 96px;   --lh-display-xl: 0.95;
  --fs-display-l:  72px;   --lh-display-l:  1.00;
  --fs-display-m:  56px;   --lh-display-m:  1.02;
  --fs-display-s:  44px;   --lh-display-s:  1.05;

  --fs-h1:         36px;   --lh-h1:         1.10;
  --fs-h2:         28px;   --lh-h2:         1.15;
  --fs-h3:         22px;   --lh-h3:         1.20;
  --fs-h4:         18px;   --lh-h4:         1.30;

  --fs-body-l:     18px;   --lh-body-l:     1.50;
  --fs-body:       16px;   --lh-body:       1.50;
  --fs-body-s:     14px;   --lh-body-s:     1.45;

  --fs-caption:    13px;   --lh-caption:    1.35;
  --fs-tag:        12px;   --lh-tag:        1.20;    /* mono, all-caps */
  --fs-micro:      11px;   --lh-micro:      1.20;

  /* Weights */
  --fw-regular:    400;
  --fw-medium:     500;
  --fw-semibold:   600;
  --fw-bold:       700;

  /* Tracking */
  --ls-tight:      -0.02em;     /* display */
  --ls-snug:       -0.01em;     /* headings */
  --ls-normal:     0;
  --ls-wide:       0.06em;      /* mono caps */
  --ls-wider:      0.12em;      /* mono caps small */

  /* ----------  SPACING  ---------- */
  --space-1:  4px;
  --space-2:  8px;
  --space-3:  12px;
  --space-4:  16px;
  --space-5:  20px;
  --space-6:  24px;
  --space-8:  32px;
  --space-10: 40px;
  --space-12: 48px;
  --space-16: 64px;
  --space-20: 80px;
  --space-24: 96px;

  /* ----------  RADII  ---------- */
  /* Wisy uses GENEROUSLY rounded corners on large cards and pill capsules. */
  --radius-xs:   4px;
  --radius-sm:   8px;
  --radius-md:  12px;
  --radius-lg:  20px;
  --radius-xl:  28px;
  --radius-2xl: 40px;
  --radius-pill: 999px;

  /* ----------  SHADOWS  ---------- */
  /* Subtle and crisp — Wisy is "clean", not "fluffy". No big glows. */
  --shadow-xs: 0 1px 0 rgba(16, 24, 64, 0.04);
  --shadow-sm: 0 1px 2px rgba(16, 24, 64, 0.06), 0 1px 1px rgba(16, 24, 64, 0.03);
  --shadow-md: 0 6px 14px rgba(16, 24, 64, 0.07), 0 2px 4px rgba(16, 24, 64, 0.04);
  --shadow-lg: 0 18px 40px rgba(16, 24, 64, 0.10), 0 4px 8px rgba(16, 24, 64, 0.05);
  --shadow-indigo: 0 12px 28px rgba(83, 84, 237, 0.18);

  /* ----------  MOTION  ---------- */
  --ease-out:   cubic-bezier(0.16, 1, 0.30, 1);   /* default snappy */
  --ease-in-out: cubic-bezier(0.65, 0, 0.35, 1);
  --dur-fast:   120ms;
  --dur-base:   200ms;
  --dur-slow:   360ms;
}

/* ============================================================
   SEMANTIC TYPOGRAPHY CLASSES
   Use these on real elements. Keep raw vars for one-offs.
   ============================================================ */

.t-display-xl,
.t-display-l,
.t-display-m,
.t-display-s {
  font-family: var(--font-sans);
  font-weight: var(--fw-medium);
  letter-spacing: var(--ls-tight);
  color: var(--fg-1);
  text-wrap: balance;
}
.t-display-xl { font-size: var(--fs-display-xl); line-height: var(--lh-display-xl); }
.t-display-l  { font-size: var(--fs-display-l);  line-height: var(--lh-display-l);  }
.t-display-m  { font-size: var(--fs-display-m);  line-height: var(--lh-display-m);  }
.t-display-s  { font-size: var(--fs-display-s);  line-height: var(--lh-display-s);  }

.t-h1, .t-h2, .t-h3, .t-h4 {
  font-family: var(--font-sans);
  font-weight: var(--fw-semibold);
  letter-spacing: var(--ls-snug);
  color: var(--fg-1);
}
.t-h1 { font-size: var(--fs-h1); line-height: var(--lh-h1); }
.t-h2 { font-size: var(--fs-h2); line-height: var(--lh-h2); }
.t-h3 { font-size: var(--fs-h3); line-height: var(--lh-h3); }
.t-h4 { font-size: var(--fs-h4); line-height: var(--lh-h4); }

.t-body-l { font-family: var(--font-sans); font-weight: var(--fw-regular); font-size: var(--fs-body-l); line-height: var(--lh-body-l); color: var(--fg-1); }
.t-body   { font-family: var(--font-sans); font-weight: var(--fw-regular); font-size: var(--fs-body);   line-height: var(--lh-body);   color: var(--fg-1); }
.t-body-s { font-family: var(--font-sans); font-weight: var(--fw-regular); font-size: var(--fs-body-s); line-height: var(--lh-body-s); color: var(--fg-2); }
.t-caption{ font-family: var(--font-sans); font-weight: var(--fw-regular); font-size: var(--fs-caption);line-height: var(--lh-caption);color: var(--fg-3); }

/* Mono — always uppercase, always letter-spaced. Used for tags, labels, kickers. */
.t-tag, .t-kicker, .t-mono-caps {
  font-family: var(--font-mono);
  font-weight: var(--fw-medium);
  font-size: var(--fs-tag);
  line-height: var(--lh-tag);
  letter-spacing: var(--ls-wide);
  text-transform: uppercase;
  color: var(--fg-2);
}

.t-mono { font-family: var(--font-mono); font-weight: var(--fw-regular); }

/* Inline link style (indigo, underline on hover) */
.t-link {
  color: var(--fg-accent);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color var(--dur-fast) var(--ease-out);
}
.t-link:hover { border-bottom-color: var(--fg-accent); }

/* ============================================================
   BASE ELEMENT BINDINGS
   Apply via class on a wrapper to opt in (e.g. <body class="wisy">)
   ============================================================ */

.wisy { font-family: var(--font-sans); color: var(--fg-1); background: var(--bg-1); }
.wisy h1 { font-size: var(--fs-h1); line-height: var(--lh-h1); font-weight: var(--fw-semibold); letter-spacing: var(--ls-snug); }
.wisy h2 { font-size: var(--fs-h2); line-height: var(--lh-h2); font-weight: var(--fw-semibold); letter-spacing: var(--ls-snug); }
.wisy h3 { font-size: var(--fs-h3); line-height: var(--lh-h3); font-weight: var(--fw-semibold); }
.wisy h4 { font-size: var(--fs-h4); line-height: var(--lh-h4); font-weight: var(--fw-semibold); }
.wisy p  { font-size: var(--fs-body); line-height: var(--lh-body); }
.wisy code, .wisy kbd, .wisy pre { font-family: var(--font-mono); }

</style>
<style>
  /* -------- Deck scale (1920×1080) -------- */
  :root {
    --type-title:     112px;
    --type-display:   96px;
    --type-subtitle:  44px;
    --type-h:         60px;
    --type-body:      30px;
    --type-body-l:    36px;
    --type-small:     24px;
    --type-mono:      20px;

    --pad-top:    96px;
    --pad-bottom: 96px;
    --pad-x:      120px;
    --gap-title:  56px;
    --gap-item:   28px;
  }

  html, body { margin: 0; padding: 0; background: #000; font-family: var(--font-sans); color: var(--fg-1); }

  deck-stage { background: var(--wisy-white); }

  /* -------- Slide base -------- */
  section {
    box-sizing: border-box;
    background: var(--wisy-white);
    color: var(--fg-1);
    overflow: hidden;
    font-family: var(--font-sans);
  }

  /* Standard padded slide */
  .slide-pad {
    padding: var(--pad-top) var(--pad-x) var(--pad-bottom);
  }

  /* -------- Reusable text -------- */
  .kicker {
    font-family: var(--font-mono);
    font-weight: 500;
    font-size: 24px;
    line-height: 1.2;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--fg-2);
    display: inline-flex;
    align-items: center;
    gap: 14px;
  }
  .kicker .dot {
    width: 10px; height: 10px; border-radius: 999px;
    background: var(--wisy-indigo);
    display: inline-block;
  }
  .kicker.on-dark { color: var(--wisy-indigo-200); }
  .kicker.on-dark .dot { background: var(--wisy-lime); }

  .title {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: var(--type-title);
    line-height: 0.97;
    letter-spacing: -0.025em;
    color: var(--fg-1);
    margin: 0;
    text-wrap: balance;
  }
  .title .ink-indigo { color: var(--wisy-indigo); }
  .title .ink-lime {
    background: var(--wisy-lime);
    padding: 0 14px 6px;
    border-radius: 12px;
    box-decoration-break: clone;
    -webkit-box-decoration-break: clone;
  }

  .subtitle {
    font-family: var(--font-sans);
    font-weight: 400;
    font-size: var(--type-subtitle);
    line-height: 1.18;
    letter-spacing: -0.012em;
    color: var(--fg-2);
    margin: 0;
    text-wrap: balance;
  }

  .body {
    font-family: var(--font-sans);
    font-weight: 400;
    font-size: var(--type-body-l);
    line-height: 1.45;
    color: var(--fg-1);
    margin: 0;
  }
  .body-s {
    font-size: var(--type-body);
    color: var(--fg-2);
    line-height: 1.45;
    margin: 0;
  }

  /* Pills / chips */
  .pill {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    height: 56px;
    padding: 0 26px;
    border-radius: 999px;
    background: var(--wisy-indigo-100);
    color: var(--wisy-indigo);
    font-family: var(--font-mono);
    font-size: 20px;
    font-weight: 500;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }
  .pill.lime { background: var(--wisy-lime); color: var(--wisy-black); }
  .pill.ink  { background: var(--wisy-black); color: var(--wisy-white); }
  .pill.outline { background: transparent; color: var(--wisy-black); border: 1.5px solid var(--wisy-black); }

  /* Page chrome — slide number + brand */
  .chrome {
    position: absolute;
    inset: auto 0 36px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 var(--pad-x);
    font-family: var(--font-mono);
    font-size: 16px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-3);
    pointer-events: none;
  }
  .chrome.on-dark { color: rgba(255,255,255,0.55); }
  .chrome .brand { display: inline-flex; align-items: center; gap: 12px; }
  .chrome .brand .w {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 18px;
    letter-spacing: -0.02em;
    text-transform: lowercase;
    color: var(--wisy-indigo);
  }
  .chrome.on-dark .brand .w { color: var(--wisy-white); }

  /* ============================================================
     SLIDE 1 — Title
     ============================================================ */
  .s-title {
    position: relative;
    height: 100%;
    background: var(--wisy-white);
    display: grid;
    grid-template-columns: 1fr 720px;
  }
  .s-title__left {
    padding: 96px var(--pad-x) 80px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    box-sizing: border-box;
    height: 100%;
  }
  .s-title__wordmark {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 200px;
    line-height: 0.85;
    letter-spacing: -0.04em;
    color: var(--wisy-indigo);
    text-transform: lowercase;
    margin: 24px 0 0;
  }
  .s-title__hook {
    max-width: 920px;
  }
  .s-title__hook .t {
    font-size: 76px;
    font-weight: 500;
    line-height: 0.98;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 0 0 28px;
    text-wrap: balance;
  }
  .s-title__hook .t em {
    font-style: normal;
    color: var(--wisy-indigo);
  }
  .s-title__hook .sub {
    font-size: 26px;
    color: var(--fg-2);
    line-height: 1.4;
    margin: 0;
    max-width: 760px;
  }
  .s-title__meta {
    display: flex;
    gap: 24px;
    align-items: center;
    color: var(--fg-3);
    font-family: var(--font-mono);
    font-size: 24px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }
  .s-title__meta span.bar { width: 32px; height: 1px; background: var(--fg-3); }

  .s-title__right {
    position: relative;
    background: var(--wisy-indigo);
    overflow: hidden;
  }
  .s-title__right::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      radial-gradient(ellipse at 70% 30%, rgba(221,244,91,0.18), transparent 60%),
      url("https://images.unsplash.com/photo-1604719312566-8912e9227c6a?w=1600&q=80&auto=format&fit=crop") center/cover;
    mix-blend-mode: luminosity;
    opacity: 0.55;
  }
  .s-title__right::after {
    content: "";
    position: absolute; inset: 0;
    background: linear-gradient(180deg, rgba(83,84,237,0.55) 0%, rgba(83,84,237,0.92) 100%);
  }
  .s-title__rightInner {
    position: relative;
    z-index: 2;
    height: 100%;
    box-sizing: border-box;
    padding: 72px 64px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: var(--wisy-white);
  }
  .s-title__mark {
    width: 84px; height: 84px;
    border-radius: 20px;
    background: var(--wisy-white);
    display: grid; place-items: center;
    font-family: var(--font-sans);
    color: var(--wisy-indigo);
    font-weight: 700;
    font-size: 56px;
    letter-spacing: -0.04em;
    line-height: 1;
  }
  .s-title__statBlock {
    display: flex;
    flex-direction: column;
    gap: 18px;
  }
  .s-title__stat {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 64px;
    line-height: 0.95;
    letter-spacing: -0.03em;
    color: var(--wisy-lime);
    margin: 0;
  }
  .s-title__statLbl {
    font-family: var(--font-sans);
    font-weight: 400;
    font-size: 24px;
    line-height: 1.35;
    color: rgba(255,255,255,0.9);
    max-width: 520px;
    margin: 0;
  }

  /* ============================================================
     SLIDE 2 — $1.7T
     ============================================================ */
  .s-stakes {
    height: 100%;
    box-sizing: border-box;
    background: var(--wisy-black);
    color: var(--wisy-white);
    position: relative;
    padding: 72px var(--pad-x) 80px;
    display: flex;
    flex-direction: column;
    gap: 40px;
  }
  .s-stakes .kicker { color: var(--wisy-indigo-200); }
  .s-stakes .kicker .dot { background: var(--wisy-lime); }

  .s-stakes__hero {
    display: grid;
    grid-template-columns: 1.05fr 1fr;
    gap: 64px;
    align-items: center;
    flex: 1;
    min-height: 0;
  }
  .s-stakes__number {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 300px;
    line-height: 0.85;
    letter-spacing: -0.05em;
    color: var(--wisy-lime);
    margin: 0;
  }
  .s-stakes__number .unit { font-size: 200px; color: var(--wisy-white); letter-spacing: -0.02em; margin-left: 12px; }
  .s-stakes__copy h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 56px;
    line-height: 1.02;
    letter-spacing: -0.02em;
    color: var(--wisy-white);
    margin: 0 0 24px;
    text-wrap: balance;
  }
  .s-stakes__copy p {
    font-size: 26px;
    line-height: 1.4;
    color: rgba(255,255,255,0.78);
    margin: 0;
    max-width: 580px;
  }
  .s-stakes__row {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 36px;
    padding-top: 28px;
    border-top: 1px solid rgba(255,255,255,0.12);
    align-items: start;
    flex-shrink: 0;
  }
  .s-stakes__cell .n {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 44px;
    line-height: 1;
    letter-spacing: -0.025em;
    color: var(--wisy-white);
    margin: 0 0 12px;
  }
  .s-stakes__cell .n .accent { color: var(--wisy-lime); }
  .s-stakes__cell .l {
    font-family: var(--font-sans);
    font-size: 24px;
    line-height: 1.3;
    color: rgba(255,255,255,0.78);
    margin: 0;
  }
  .s-stakes__cell.quote {
    padding: 4px 0 4px 22px;
    border-left: 2px solid var(--wisy-lime);
  }
  .s-stakes__cell.quote .q {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 26px;
    line-height: 1.25;
    color: var(--wisy-lime);
    margin: 0;
    text-wrap: balance;
  }

  /* ============================================================
     SLIDE 3 — Ground reality
     ============================================================ */
  .s-ground {
    height: 100%;
    display: grid;
    grid-template-columns: 1.05fr 1fr;
  }
  .s-ground__photo {
    position: relative;
    background:
      linear-gradient(180deg, rgba(0,0,0,0.05) 0%, rgba(0,0,0,0.45) 100%),
      url("https://images.unsplash.com/photo-1604719312566-8912e9227c6a?w=1600&q=80&auto=format&fit=crop") center/cover;
  }
  .s-ground__rep {
    position: absolute;
    inset: auto 56px 56px;
    display: flex;
    flex-direction: column-reverse;
    gap: 18px;
  }
  .s-ground__rep .nameRow {
    display: flex; align-items: center; gap: 16px;
  }
  .s-ground__rep .avatar {
    width: 64px; height: 64px;
    border-radius: 999px;
    background: var(--wisy-indigo);
    color: var(--wisy-white);
    display: grid; place-items: center;
    font-weight: 600;
    font-size: 24px;
    border: 3px solid var(--wisy-white);
  }
  .s-ground__rep .name {
    font-family: var(--font-sans);
    color: var(--wisy-white);
    font-weight: 600;
    font-size: 26px;
    line-height: 1.2;
  }
  .s-ground__rep .name span {
    display: block;
    font-size: 20px;
    font-weight: 400;
    color: rgba(255,255,255,0.85);
    font-family: var(--font-mono);
    letter-spacing: 0.08em;
    text-transform: uppercase;
    margin-top: 4px;
  }
  .s-ground__chips {
    display: flex; flex-wrap: wrap; gap: 10px;
    max-width: 640px;
  }
  .s-ground__chips .c {
    background: rgba(255,255,255,0.95);
    color: var(--wisy-black);
    border-radius: 999px;
    padding: 10px 18px;
    font-family: var(--font-mono);
    font-size: 18px;
    font-weight: 500;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    backdrop-filter: blur(8px);
  }
  .s-ground__chips .c.warn { background: var(--wisy-lime); color: var(--wisy-black); }

  .s-ground__right {
    padding: 80px 96px 96px 96px;
    display: flex;
    flex-direction: column;
    gap: 40px;
    background: var(--wisy-white);
    box-sizing: border-box;
    height: 100%;
  }
  .s-ground__title h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 68px;
    line-height: 0.98;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 24px 0 0;
    text-wrap: balance;
  }
  .s-ground__title h2 em { font-style: normal; color: var(--wisy-indigo); }

  .s-ground__chaos {
    display: flex;
    flex-direction: column;
    gap: 12px;
  }
  .s-ground__chaosRow {
    display: flex; align-items: center; gap: 16px;
    background: var(--wisy-gray-50);
    border-radius: 16px;
    padding: 14px 20px;
    border: 1px solid var(--border-1);
  }
  .s-ground__chaosRow .app {
    width: 44px; height: 44px; border-radius: 10px;
    display: grid; place-items: center;
    font-family: var(--font-mono); font-weight: 600;
    color: var(--wisy-white);
    font-size: 18px;
  }
  .s-ground__chaosRow .lbl {
    font-size: 24px;
    color: var(--fg-1);
    font-weight: 500;
  }
  .s-ground__chaosRow .tag {
    margin-left: auto;
    font-family: var(--font-mono);
    font-size: 16px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--wisy-danger);
  }

  .s-ground__quote {
    margin-top: auto;
    padding-top: 28px;
    border-top: 2px solid var(--wisy-black);
    font-size: 26px;
    line-height: 1.3;
    color: var(--fg-1);
    font-weight: 500;
  }
  .s-ground__quote em { font-style: normal; background: var(--wisy-lime); padding: 2px 10px 4px; border-radius: 8px; }

  /* ============================================================
     SLIDE 4 — AIR
     ============================================================ */
  .s-air {
    height: 100%;
    background: var(--wisy-white);
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  .s-air__left {
    padding: var(--pad-top) 80px var(--pad-bottom) var(--pad-x);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .s-air__brand {
    display: flex; align-items: baseline; gap: 28px;
    margin-top: 28px;
  }
  .s-air__brand .name {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 156px;
    line-height: 0.9;
    letter-spacing: -0.04em;
    color: var(--wisy-indigo);
  }
  .s-air__brand .expand {
    font-family: var(--font-mono);
    font-size: 18px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--fg-2);
    max-width: 220px;
    line-height: 1.45;
  }
  .s-air__pitch {
    font-size: 40px;
    line-height: 1.15;
    color: var(--fg-1);
    margin: 32px 0 0;
    max-width: 640px;
    font-weight: 500;
    text-wrap: balance;
  }
  .s-air__pitch em { font-style: normal; color: var(--wisy-indigo); }

  .s-air__bars {
    display: flex; flex-direction: column; gap: 22px;
    margin-top: 32px;
  }
  .s-air__bar { }
  .s-air__bar .row {
    display: flex; justify-content: space-between; align-items: baseline;
    margin-bottom: 10px;
  }
  .s-air__bar .row .l {
    font-family: var(--font-mono);
    font-size: 18px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--fg-2);
  }
  .s-air__bar .row .r {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 22px;
    color: var(--fg-1);
  }
  .s-air__bar .track {
    height: 18px;
    background: var(--wisy-gray-50);
    border-radius: 999px;
    overflow: hidden;
    position: relative;
  }
  .s-air__bar .fill {
    height: 100%;
    border-radius: 999px;
  }
  .s-air__bar.legacy .fill { width: 32%; background: var(--wisy-gray-500); }
  .s-air__bar.air .fill {
    width: 96%;
    background: linear-gradient(90deg, var(--wisy-indigo) 0%, var(--wisy-indigo) 70%, var(--wisy-lime) 100%);
  }
  .s-air__caps {
    display: flex; gap: 12px; margin-top: 8px;
    flex-wrap: wrap;
  }
  .s-air__cap {
    border: 1px solid var(--border-1);
    border-radius: 999px;
    padding: 10px 18px;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--fg-2);
  }

  .s-air__right {
    position: relative;
    background:
      linear-gradient(135deg, var(--wisy-indigo-100) 0%, var(--wisy-white) 100%);
    overflow: hidden;
  }
  .s-air__right::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      radial-gradient(circle at 50% 50%, rgba(83,84,237,0.10), transparent 55%);
  }
  /* Background grid */
  .s-air__right::after {
    content: "";
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(83,84,237,0.06) 1px, transparent 1px),
      linear-gradient(90deg, rgba(83,84,237,0.06) 1px, transparent 1px);
    background-size: 48px 48px;
    pointer-events: none;
    mask-image: radial-gradient(ellipse at center, black 35%, transparent 80%);
    -webkit-mask-image: radial-gradient(ellipse at center, black 35%, transparent 80%);
  }

  /* Device hub */
  .s-air__hub {
    position: absolute;
    inset: 0;
    z-index: 2;
  }
  .s-air__hubSvg {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 1;
  }

  /* Center AIR core */
  .s-air__core {
    position: absolute;
    left: 50%; top: 50%;
    transform: translate(-50%, -50%);
    width: 240px; height: 240px;
    border-radius: 999px;
    background: var(--wisy-black);
    color: var(--wisy-white);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 6px;
    box-shadow: 0 30px 80px rgba(83,84,237,0.30), 0 0 0 8px rgba(83,84,237,0.08);
    z-index: 3;
    overflow: hidden;
  }
  .s-air__core::before,
  .s-air__core::after {
    content: "";
    position: absolute;
    inset: 0;
    border-radius: 999px;
    border: 2px solid var(--wisy-indigo);
    opacity: 0;
  }
  [data-deck-active] .s-air__core::before { animation: airCoreRing 2600ms var(--ease-out) 200ms infinite; }
  [data-deck-active] .s-air__core::after  { animation: airCoreRing 2600ms var(--ease-out) 1500ms infinite; }
  @keyframes airCoreRing {
    0%   { opacity: 0.7; transform: scale(1); }
    100% { opacity: 0;   transform: scale(1.5); }
  }
  .s-air__coreLbl {
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--wisy-indigo-200);
  }
  .s-air__coreMark {
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 72px;
    line-height: 0.9;
    letter-spacing: -0.04em;
    color: var(--wisy-lime);
  }
  .s-air__coreStatus {
    display: inline-flex; align-items: center; gap: 6px;
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--wisy-lime);
    margin-top: 4px;
  }
  .s-air__coreStatus .d {
    width: 6px; height: 6px;
    border-radius: 999px;
    background: var(--wisy-lime);
  }
  [data-deck-active] .s-air__coreStatus .d {
    animation: airBlink 1100ms steps(2, end) infinite;
  }
  @keyframes airBlink {
    50% { opacity: 0.3; }
  }

  /* Device cards */
  .s-air__dev {
    position: absolute;
    transform: translate(-50%, -50%);
    width: 168px;
    background: var(--wisy-white);
    border: 1px solid var(--border-1);
    border-radius: 18px;
    padding: 14px 16px 12px;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 8px;
    box-shadow: var(--shadow-sm);
    z-index: 2;
  }
  [data-deck-active] .s-air__dev {
    animation: airDevIn 540ms var(--ease-out) both;
  }
  [data-deck-active] .s-air__dev.d1 { animation-delay: 80ms; }
  [data-deck-active] .s-air__dev.d2 { animation-delay: 200ms; }
  [data-deck-active] .s-air__dev.d3 { animation-delay: 320ms; }
  [data-deck-active] .s-air__dev.d4 { animation-delay: 440ms; }
  [data-deck-active] .s-air__dev.d5 { animation-delay: 560ms; }
  @keyframes airDevIn {
    from { opacity: 0; transform: translate(-50%, -50%) scale(0.86); }
    to   { opacity: 1; transform: translate(-50%, -50%) scale(1); }
  }
  .s-air__devIcon {
    width: 56px; height: 56px;
    border-radius: 14px;
    background: var(--wisy-indigo-100);
    color: var(--wisy-indigo);
    display: grid; place-items: center;
    margin-top: 2px;
  }
  .s-air__devIcon svg { width: 32px; height: 32px; stroke: currentColor; fill: none; stroke-width: 1.8; stroke-linecap: round; stroke-linejoin: round; }
  .s-air__devLbl {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 18px;
    color: var(--fg-1);
    line-height: 1.1;
  }
  .s-air__devMeta {
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--fg-3);
    line-height: 1.3;
  }
  .s-air__devOnline {
    display: inline-flex; align-items: center; gap: 5px;
    font-family: var(--font-mono);
    font-size: 10px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--wisy-success);
    font-weight: 600;
  }
  .s-air__devOnline .d {
    width: 5px; height: 5px;
    border-radius: 999px;
    background: var(--wisy-success);
  }
  [data-deck-active] .s-air__devOnline .d {
    animation: airDevDot 1600ms ease-out infinite;
  }
  [data-deck-active] .s-air__dev.d2 .s-air__devOnline .d { animation-delay: -200ms; }
  [data-deck-active] .s-air__dev.d3 .s-air__devOnline .d { animation-delay: -400ms; }
  [data-deck-active] .s-air__dev.d4 .s-air__devOnline .d { animation-delay: -600ms; }
  [data-deck-active] .s-air__dev.d5 .s-air__devOnline .d { animation-delay: -800ms; }
  @keyframes airDevDot {
    0%   { box-shadow: 0 0 0 0 rgba(31,138,91,0.5); }
    70%  { box-shadow: 0 0 0 8px rgba(31,138,91,0); }
    100% { box-shadow: 0 0 0 0 rgba(31,138,91,0); }
  }

  /* SVG connection lines + traveling pulses */
  .s-air__hubPath {
    fill: none;
    stroke: rgba(83,84,237,0.22);
    stroke-width: 1.5;
    vector-effect: non-scaling-stroke;
  }
  .s-air__hubPathLive {
    fill: none;
    stroke: var(--wisy-indigo);
    stroke-width: 2;
    stroke-linecap: round;
    stroke-dasharray: 4 10;
    vector-effect: non-scaling-stroke;
  }
  [data-deck-active] .s-air__hubPathLive {
    animation: airDash 1400ms linear infinite;
  }
  @keyframes airDash {
    to { stroke-dashoffset: -140; }
  }

  /* Caption strip at bottom of right panel */
  .s-air__caption {
    position: absolute;
    left: 56px; right: 56px; bottom: 48px;
    display: flex; justify-content: space-between; align-items: center;
    padding: 16px 20px;
    background: var(--wisy-white);
    border: 1px solid var(--border-1);
    border-radius: 16px;
    box-shadow: var(--shadow-md);
    z-index: 4;
    font-family: var(--font-mono);
    font-size: 13px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--fg-2);
  }
  .s-air__caption .lbl {
    color: var(--wisy-indigo);
    font-weight: 600;
  }
  .s-air__caption .v {
    color: var(--wisy-black);
    font-weight: 600;
  }
  .s-air__caption em {
    font-style: normal;
    color: var(--wisy-lime-700);
  }

  /* ============================================================
     SLIDE 5 — AI Agents
     ============================================================ */
  .s-agents {
    height: 100%;
    box-sizing: border-box;
    background: var(--wisy-indigo-100);
    padding: 72px var(--pad-x) 72px;
    display: flex;
    flex-direction: column;
    gap: 40px;
  }
  .s-agents__head {
    display: grid; grid-template-columns: 1fr 600px;
    gap: 80px;
    align-items: end;
  }
  .s-agents__head h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 64px;
    line-height: 0.98;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 20px 0 0;
    text-wrap: balance;
  }
  .s-agents__head h2 em { font-style: normal; color: var(--wisy-indigo); }
  .s-agents__head p {
    font-size: 24px;
    line-height: 1.4;
    color: var(--fg-2);
    margin: 0;
  }

  .s-agents__flow {
    display: grid;
    grid-template-columns: 340px 1fr 340px;
    gap: 48px;
    align-items: stretch;
    flex: 1;
    min-height: 0;
  }

  .s-agents__phone {
    position: relative;
    width: 340px; height: 560px;
    border-radius: 40px;
    background: #000;
    padding: 12px;
    box-shadow: 0 30px 60px rgba(16,24,64,0.18);
    margin: 0 auto;
    align-self: center;
    box-sizing: border-box;
  }
  .s-agents__phone::after {
    content: ""; position: absolute; top: 22px; left: 50%; transform: translateX(-50%);
    width: 110px; height: 26px; border-radius: 14px; background: #000; z-index: 2;
  }
  .s-agents__phoneScreen {
    width: 100%; height: 100%;
    border-radius: 32px;
    background: linear-gradient(180deg, #f7f7fb 0%, white 100%);
    position: relative; overflow: hidden;
    display: flex; flex-direction: column;
    padding: 64px 18px 18px;
    gap: 12px;
  }
  .s-agents__phoneHead {
    display: flex; align-items: center; gap: 10px;
    margin-bottom: 4px;
  }
  .s-agents__phoneHead .b {
    background: var(--wisy-black); color: var(--wisy-white);
    padding: 5px 10px; border-radius: 999px;
    font-family: var(--font-mono); font-size: 10px;
    letter-spacing: 0.12em; text-transform: uppercase;
    font-weight: 600;
  }
  .s-agents__phoneHead .t {
    font-family: var(--font-sans); font-weight: 600; font-size: 16px;
    color: var(--fg-1);
  }
  .s-agents__photoCap {
    height: 130px;
    border-radius: 16px;
    background: url("https://images.unsplash.com/photo-1542838132-92c53300491e?w=600&q=80&auto=format&fit=crop") center/cover;
    position: relative;
    overflow: hidden;
  }
  .s-agents__photoCap .check {
    position: absolute; right: 10px; bottom: 10px;
    background: var(--wisy-lime); color: var(--wisy-black);
    border-radius: 999px;
    padding: 4px 10px;
    font-family: var(--font-mono); font-size: 9px; font-weight: 600;
    letter-spacing: 0.12em; text-transform: uppercase;
  }
  .s-agents__phoneSub {
    font-family: var(--font-mono); font-size: 9px;
    letter-spacing: 0.14em; text-transform: uppercase;
    color: var(--fg-3);
    margin-top: 4px;
  }
  .s-agents__action {
    border: 1px solid var(--border-1);
    border-radius: 14px;
    padding: 10px 12px;
    background: white;
    display: flex; flex-direction: column; gap: 4px;
  }
  .s-agents__action.top {
    border: 1.5px solid var(--wisy-indigo);
    background: var(--wisy-indigo-100);
  }
  .s-agents__action .ahdr {
    display: flex; justify-content: space-between;
    font-family: var(--font-mono); font-size: 9px;
    letter-spacing: 0.12em; text-transform: uppercase;
    color: var(--fg-3);
  }
  .s-agents__action .ahdr .pri { color: var(--wisy-indigo); font-weight: 600; }
  .s-agents__action.top .ahdr .pri { color: var(--wisy-indigo); }
  .s-agents__action .ttl {
    font-family: var(--font-sans); font-weight: 600; font-size: 13px;
    color: var(--fg-1); line-height: 1.25;
  }
  .s-agents__action .rev {
    font-family: var(--font-mono); font-size: 11px; color: var(--wisy-success);
    font-weight: 600;
  }

  /* Middle: flow with arrows */
  .s-agents__pipe {
    display: flex; flex-direction: column;
    gap: 14px;
    justify-content: center;
  }
  .s-agents__step {
    background: var(--wisy-white);
    border-radius: 20px;
    border: 1px solid var(--border-1);
    padding: 20px 24px;
    display: grid;
    grid-template-columns: 48px 1fr auto;
    align-items: center;
    gap: 18px;
    box-shadow: var(--shadow-sm);
  }
  .s-agents__step .num {
    width: 48px; height: 48px;
    border-radius: 999px;
    background: var(--wisy-black);
    color: var(--wisy-white);
    display: grid; place-items: center;
    font-family: var(--font-mono);
    font-weight: 600;
    font-size: 20px;
  }
  .s-agents__step .num.lime { background: var(--wisy-lime); color: var(--wisy-black); }
  .s-agents__step .num.indigo { background: var(--wisy-indigo); color: var(--wisy-white); }
  .s-agents__step .body { min-width: 0; }
  .s-agents__step .body .lbl {
    font-family: var(--font-mono); font-size: 14px;
    letter-spacing: 0.12em; text-transform: uppercase;
    color: var(--fg-3); margin: 0 0 4px;
  }
  .s-agents__step .body .t {
    font-family: var(--font-sans); font-weight: 500;
    font-size: 24px; color: var(--fg-1); line-height: 1.2;
    margin: 0;
  }
  .s-agents__step .body .t em { font-style: normal; color: var(--wisy-indigo); font-weight: 600; }
  .s-agents__step .time {
    font-family: var(--font-mono);
    font-size: 20px; font-weight: 600;
    color: var(--wisy-success);
    white-space: nowrap;
  }
  .s-agents__pipeArrow {
    text-align: center;
    color: var(--wisy-indigo);
    font-size: 22px;
    margin: -6px 0;
    line-height: 1;
  }

  /* Right column: outcomes */
  .s-agents__out {
    display: flex; flex-direction: column;
    gap: 14px;
    justify-content: center;
  }
  .s-agents__out h3 {
    font-family: var(--font-mono);
    font-size: 16px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-2);
    margin: 0 0 4px;
    font-weight: 500;
  }
  .s-agents__outCard {
    background: var(--wisy-white);
    border: 1px solid var(--border-1);
    border-radius: 18px;
    padding: 20px 24px;
  }
  .s-agents__outCard .v {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 52px;
    line-height: 1;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 0 0 8px;
  }
  .s-agents__outCard .v .small { font-size: 28px; }
  .s-agents__outCard .l {
    font-family: var(--font-sans);
    font-size: 18px;
    color: var(--fg-2);
    line-height: 1.35;
    margin: 0;
  }
  .s-agents__outCard.dark {
    background: var(--wisy-black);
    color: var(--wisy-white);
    border: none;
  }
  .s-agents__outCard.dark .v { color: var(--wisy-lime); }
  .s-agents__outCard.dark .l { color: rgba(255,255,255,0.75); }

  /* ============================================================
     SLIDE 6 — HQI
     ============================================================ */
  .s-hqi {
    height: 100%;
    background: var(--wisy-white);
    padding: var(--pad-top) var(--pad-x) var(--pad-bottom);
    display: grid;
    grid-template-rows: auto 1fr;
    gap: 40px;
  }
  .s-hqi__head {
    display: grid;
    grid-template-columns: 1fr 600px;
    gap: 80px;
    align-items: end;
  }
  .s-hqi__head h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 96px;
    line-height: 0.95;
    letter-spacing: -0.03em;
    color: var(--wisy-black);
    margin: 24px 0 0;
    text-wrap: balance;
  }
  .s-hqi__head h2 em { font-style: normal; color: var(--wisy-indigo); }
  .s-hqi__head p {
    font-size: 26px;
    line-height: 1.4;
    color: var(--fg-2);
    margin: 0;
  }
  .s-hqi__head p strong { color: var(--fg-1); font-weight: 600; }

  /* Mac window */
  .s-hqi__mac {
    background: #eaeaef;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: var(--shadow-lg);
    border: 1px solid var(--border-1);
    display: flex;
    flex-direction: column;
  }
  .s-hqi__macBar {
    background: linear-gradient(180deg, #f6f6fa 0%, #ececf2 100%);
    height: 44px;
    display: flex;
    align-items: center;
    padding: 0 18px;
    gap: 8px;
    border-bottom: 1px solid #d8d8e0;
  }
  .s-hqi__macBar .dot {
    width: 13px; height: 13px; border-radius: 999px;
    background: #ddd;
  }
  .s-hqi__macBar .dot.r { background: #ff5f57; }
  .s-hqi__macBar .dot.y { background: #ffbd2e; }
  .s-hqi__macBar .dot.g { background: #28c941; }
  .s-hqi__macBar .url {
    margin-left: 20px;
    font-family: var(--font-mono);
    font-size: 14px;
    color: var(--fg-3);
    letter-spacing: 0.04em;
  }
  .s-hqi__macBar .url b { color: var(--wisy-indigo); font-weight: 600; }

  .s-hqi__app {
    flex: 1;
    background: var(--wisy-white);
    display: grid;
    grid-template-columns: 220px 1fr;
  }
  .s-hqi__sidebar {
    background: #fafafd;
    border-right: 1px solid var(--border-1);
    padding: 28px 20px;
    display: flex; flex-direction: column;
    gap: 6px;
  }
  .s-hqi__sidebar .logo {
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 24px;
    color: var(--wisy-indigo);
    letter-spacing: -0.02em;
    margin-bottom: 28px;
  }
  .s-hqi__sidebar .nav {
    display: flex; align-items: center; gap: 10px;
    padding: 10px 12px;
    border-radius: 10px;
    font-family: var(--font-sans);
    font-size: 14px;
    color: var(--fg-2);
    cursor: pointer;
  }
  .s-hqi__sidebar .nav.active {
    background: var(--wisy-indigo-100);
    color: var(--wisy-indigo);
    font-weight: 600;
  }
  .s-hqi__sidebar .nav .ic {
    width: 16px; height: 16px; border-radius: 4px;
    background: var(--fg-3);
    opacity: 0.4;
  }
  .s-hqi__sidebar .nav.active .ic { background: var(--wisy-indigo); opacity: 1; }

  .s-hqi__main {
    padding: 28px 32px;
    display: grid;
    grid-template-rows: auto auto 1fr;
    gap: 22px;
    overflow: hidden;
  }
  .s-hqi__topRow {
    display: flex; justify-content: space-between; align-items: center;
  }
  .s-hqi__topRow h3 {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 26px;
    color: var(--fg-1);
    margin: 0;
  }
  .s-hqi__topRow h3 span { color: var(--fg-3); font-weight: 400; font-size: 18px; }
  .s-hqi__topRow .live {
    display: flex; align-items: center; gap: 8px;
    background: var(--wisy-indigo-100);
    color: var(--wisy-indigo);
    padding: 6px 14px;
    border-radius: 999px;
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    font-weight: 600;
  }
  .s-hqi__topRow .live::before {
    content: ""; width: 8px; height: 8px; border-radius: 999px;
    background: var(--wisy-success);
    box-shadow: 0 0 0 4px rgba(31,138,91,0.18);
  }

  .s-hqi__kpis {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 16px;
  }
  .s-hqi__kpi {
    border: 1px solid var(--border-1);
    border-radius: 16px;
    padding: 18px 20px;
    background: var(--wisy-white);
  }
  .s-hqi__kpi .l {
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-3);
    margin: 0 0 8px;
  }
  .s-hqi__kpi .v {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 38px;
    line-height: 1;
    letter-spacing: -0.02em;
    color: var(--fg-1);
    margin: 0;
  }
  .s-hqi__kpi .d {
    font-family: var(--font-mono);
    font-size: 12px;
    margin-top: 6px;
    color: var(--wisy-success);
    font-weight: 600;
  }
  .s-hqi__kpi .d.bad { color: var(--wisy-danger); }

  .s-hqi__panels {
    display: grid;
    grid-template-columns: 1.3fr 1fr;
    gap: 18px;
    min-height: 0;
  }
  .s-hqi__panel {
    border: 1px solid var(--border-1);
    border-radius: 16px;
    padding: 20px;
    background: var(--wisy-white);
    display: flex; flex-direction: column;
    overflow: hidden;
  }
  .s-hqi__panel h4 {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 16px;
    margin: 0 0 16px;
    color: var(--fg-1);
    display: flex; align-items: center; justify-content: space-between;
  }
  .s-hqi__panel h4 .pill {
    font-family: var(--font-mono);
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    background: var(--wisy-gray-50);
    color: var(--fg-2);
    padding: 4px 10px;
    border-radius: 999px;
    height: auto;
    font-weight: 500;
  }
  /* Heatmap */
  .s-hqi__heat {
    display: grid;
    grid-template-columns: repeat(16, 1fr);
    grid-auto-rows: 1fr;
    gap: 4px;
    height: 100%;
  }
  .s-hqi__heat span {
    border-radius: 4px;
    background: var(--wisy-indigo-100);
  }
  /* Alerts list */
  .s-hqi__alerts {
    display: flex; flex-direction: column; gap: 10px;
  }
  .s-hqi__alert {
    display: grid;
    grid-template-columns: 8px 1fr auto;
    align-items: center;
    gap: 12px;
    padding: 10px 12px;
    border-radius: 10px;
    background: var(--wisy-gray-50);
  }
  .s-hqi__alert .bar { width: 4px; height: 100%; min-height: 34px; border-radius: 4px; background: var(--wisy-indigo); }
  .s-hqi__alert.warn .bar { background: var(--wisy-warning); }
  .s-hqi__alert.danger .bar { background: var(--wisy-danger); }
  .s-hqi__alert .body { font-family: var(--font-sans); font-size: 14px; color: var(--fg-1); font-weight: 500; line-height: 1.3; }
  .s-hqi__alert .body small { display: block; font-family: var(--font-mono); font-size: 10px; letter-spacing: 0.1em; text-transform: uppercase; color: var(--fg-3); margin-top: 2px; }
  .s-hqi__alert .rev { font-family: var(--font-mono); font-weight: 600; font-size: 14px; color: var(--wisy-success); white-space: nowrap; }

  /* Floating call-outs */
  .s-hqi__callout {
    position: absolute;
    background: var(--wisy-black);
    color: var(--wisy-white);
    border-radius: 14px;
    padding: 14px 18px;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    font-weight: 500;
    box-shadow: var(--shadow-lg);
    z-index: 5;
  }

  /* ============================================================
     SLIDE 7 — Convergence / Agentic flow
     ============================================================ */
  .s-conv {
    height: 100%;
    box-sizing: border-box;
    background:
      radial-gradient(circle at 50% 60%, rgba(83,84,237,0.06), transparent 60%),
      var(--wisy-gray-50);
    padding: 64px var(--pad-x) 64px;
    display: flex;
    flex-direction: column;
    gap: 24px;
    position: relative;
    overflow: hidden;
  }
  /* Background grid */
  .s-conv::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(83,84,237,0.05) 1px, transparent 1px),
      linear-gradient(90deg, rgba(83,84,237,0.05) 1px, transparent 1px);
    background-size: 48px 48px;
    pointer-events: none;
    mask-image: radial-gradient(ellipse at center, black 30%, transparent 75%);
    -webkit-mask-image: radial-gradient(ellipse at center, black 30%, transparent 75%);
  }
  .s-conv__head {
    position: relative;
    z-index: 2;
  }
  .s-conv__head h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 64px;
    line-height: 0.98;
    letter-spacing: -0.02em;
    color: var(--wisy-black);
    margin: 14px 0 12px;
    text-wrap: balance;
    max-width: 1500px;
  }
  .s-conv__head h2 em { font-style: normal; color: var(--wisy-indigo); }
  .s-conv__head p {
    font-size: 22px;
    color: var(--fg-2);
    line-height: 1.4;
    margin: 0;
    max-width: 1100px;
  }

  .s-conv__diagram {
    position: relative;
    flex: 1;
    min-height: 0;
    z-index: 2;
  }
  .s-conv__svg {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 1;
  }

  /* Streams column (left) */
  .s-conv__streams {
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
    width: 360px;
    display: flex;
    flex-direction: column;
    gap: 10px;
    z-index: 2;
  }
  .s-conv__stream {
    background: var(--wisy-white);
    border: 1px solid var(--border-1);
    border-radius: 14px;
    padding: 12px 18px;
    display: grid;
    grid-template-columns: 36px 1fr 14px;
    gap: 14px;
    align-items: center;
    box-shadow: var(--shadow-xs);
  }
  [data-deck-active] .s-conv__stream {
    animation: convStreamIn 480ms var(--ease-out) both;
  }
  [data-deck-active] .s-conv__stream:nth-child(1) { animation-delay: 0ms; }
  [data-deck-active] .s-conv__stream:nth-child(2) { animation-delay: 80ms; }
  [data-deck-active] .s-conv__stream:nth-child(3) { animation-delay: 160ms; }
  [data-deck-active] .s-conv__stream:nth-child(4) { animation-delay: 240ms; }
  [data-deck-active] .s-conv__stream:nth-child(5) { animation-delay: 320ms; }
  @keyframes convStreamIn {
    from { opacity: 0; transform: translateX(-24px); }
    to   { opacity: 1; transform: translateX(0); }
  }
  .s-conv__stream .icon {
    width: 36px; height: 36px;
    border-radius: 10px;
    display: grid; place-items: center;
    font-family: var(--font-mono);
    font-weight: 600;
    font-size: 14px;
    color: var(--wisy-white);
    letter-spacing: 0;
  }
  .s-conv__stream:nth-child(1) .icon { background: var(--wisy-indigo); }
  .s-conv__stream:nth-child(2) .icon { background: var(--wisy-lime); color: var(--wisy-black); }
  .s-conv__stream:nth-child(3) .icon { background: var(--wisy-indigo-200); color: var(--wisy-indigo-800); }
  .s-conv__stream:nth-child(4) .icon { background: var(--wisy-black); }
  .s-conv__stream:nth-child(5) .icon { background: var(--wisy-success); }
  .s-conv__stream .lbl {
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--fg-3);
    margin: 0 0 2px;
  }
  .s-conv__stream .ttl {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 18px;
    color: var(--fg-1);
    margin: 0;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .s-conv__stream .live {
    width: 8px; height: 8px;
    border-radius: 999px;
    background: var(--wisy-success);
    box-shadow: 0 0 0 0 rgba(31,138,91,0.5);
  }
  [data-deck-active] .s-conv__stream .live {
    animation: convDotPulse 1800ms ease-out infinite;
  }
  @keyframes convDotPulse {
    0%   { box-shadow: 0 0 0 0 rgba(31,138,91,0.6); }
    70%  { box-shadow: 0 0 0 10px rgba(31,138,91,0); }
    100% { box-shadow: 0 0 0 0 rgba(31,138,91,0); }
  }

  /* Central agent core */
  .s-conv__core {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    width: 360px;
    background: var(--wisy-black);
    color: var(--wisy-white);
    border-radius: 28px;
    padding: 26px 26px 22px;
    text-align: left;
    box-shadow: 0 30px 80px rgba(83,84,237,0.32), 0 0 0 6px rgba(83,84,237,0.06);
    z-index: 3;
    overflow: hidden;
  }
  [data-deck-active] .s-conv__core {
    animation: convCoreIn 720ms var(--ease-out) 220ms both;
  }
  @keyframes convCoreIn {
    from { opacity: 0; transform: translate(-50%, -50%) scale(0.92); }
    to   { opacity: 1; transform: translate(-50%, -50%) scale(1); }
  }
  /* Pulse ring behind core */
  .s-conv__core::before,
  .s-conv__core::after {
    content: "";
    position: absolute;
    top: 50%; left: 50%;
    width: 100%; height: 100%;
    border: 1.5px solid var(--wisy-indigo);
    border-radius: 28px;
    transform: translate(-50%, -50%) scale(1);
    opacity: 0;
    pointer-events: none;
  }
  [data-deck-active] .s-conv__core::before { animation: convRing 2400ms var(--ease-out) 800ms infinite; }
  [data-deck-active] .s-conv__core::after  { animation: convRing 2400ms var(--ease-out) 1600ms infinite; }
  @keyframes convRing {
    0%   { opacity: 0.7; transform: translate(-50%, -50%) scale(1); }
    100% { opacity: 0;   transform: translate(-50%, -50%) scale(1.45); }
  }

  .s-conv__coreHead {
    display: flex; align-items: center; gap: 10px;
    margin-bottom: 14px;
  }
  .s-conv__coreMark {
    width: 36px; height: 36px;
    border-radius: 10px;
    background: var(--wisy-indigo);
    color: var(--wisy-white);
    display: grid; place-items: center;
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 22px;
    letter-spacing: -0.04em;
    line-height: 1;
    text-transform: lowercase;
  }
  .s-conv__coreLbl {
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--wisy-indigo-200);
  }
  .s-conv__coreStatus {
    margin-left: auto;
    display: flex; align-items: center; gap: 6px;
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--wisy-lime);
  }
  .s-conv__coreStatus .d {
    width: 6px; height: 6px; border-radius: 999px;
    background: var(--wisy-lime);
  }
  [data-deck-active] .s-conv__coreStatus .d {
    animation: convBlink 1200ms steps(2, end) infinite;
  }
  @keyframes convBlink {
    50% { opacity: 0.25; }
  }

  .s-conv__coreV {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 32px;
    line-height: 1.05;
    letter-spacing: -0.025em;
    color: var(--wisy-white);
    margin: 0 0 12px;
  }
  .s-conv__coreV em { font-style: normal; color: var(--wisy-lime); }

  /* Throughput meter + sparkline */
  .s-conv__coreMeter {
    margin-bottom: 14px;
  }
  .s-conv__coreMeterTop {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 8px;
  }
  .s-conv__coreMeterTop .l {
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--wisy-indigo-200);
  }
  .s-conv__coreMeterTop .v {
    font-family: var(--font-sans);
    font-weight: 600;
    color: var(--wisy-white);
    display: inline-flex;
    align-items: baseline;
    gap: 8px;
  }
  .s-conv__coreMeterTop .v em {
    font-style: normal;
    color: var(--wisy-lime);
    font-size: 24px;
    letter-spacing: -0.025em;
    font-variant-numeric: tabular-nums;
  }
  .s-conv__coreMeterTop .v .u {
    font-family: var(--font-mono);
    font-size: 11px;
    color: rgba(255,255,255,0.55);
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }
  .s-conv__spark {
    display: grid;
    grid-template-columns: repeat(18, 1fr);
    gap: 3px;
    height: 26px;
    align-items: end;
  }
  .s-conv__spark span {
    display: block;
    background: var(--wisy-indigo-300);
    border-radius: 2px;
    height: var(--h, 30%);
    transform-origin: bottom;
  }
  [data-deck-active] .s-conv__spark span {
    animation: convSpark 1800ms var(--ease-out) infinite alternate;
  }
  [data-deck-active] .s-conv__spark span:nth-child(3n)   { animation-delay: 100ms; background: var(--wisy-lime); }
  [data-deck-active] .s-conv__spark span:nth-child(5n)   { animation-delay: 200ms; }
  [data-deck-active] .s-conv__spark span:nth-child(4n+1) { animation-delay: 300ms; }
  [data-deck-active] .s-conv__spark span:nth-child(7n)   { animation-delay: 50ms; background: var(--wisy-lime); }
  @keyframes convSpark {
    from { transform: scaleY(0.6); }
    to   { transform: scaleY(1.0); }
  }

  /* Sub-agents */
  .s-conv__agents {
    display: flex; flex-direction: column; gap: 8px;
    padding-top: 10px;
    border-top: 1px solid rgba(255,255,255,0.08);
  }
  .s-conv__agent {
    display: grid;
    grid-template-columns: 8px 1fr auto 70px;
    gap: 10px;
    align-items: center;
    font-family: var(--font-mono);
    font-size: 12px;
    color: rgba(255,255,255,0.92);
    letter-spacing: 0.02em;
  }
  .s-conv__agent .dot {
    width: 8px; height: 8px;
    border-radius: 999px;
    background: var(--wisy-lime);
    box-shadow: 0 0 0 0 rgba(221,244,91,0.5);
  }
  [data-deck-active] .s-conv__agent .dot {
    animation: convAgentPulse 1400ms var(--ease-out) infinite;
  }
  [data-deck-active] .s-conv__agent:nth-child(1) .dot { animation-duration: 1100ms; }
  [data-deck-active] .s-conv__agent:nth-child(2) .dot { animation-duration: 1500ms; }
  [data-deck-active] .s-conv__agent:nth-child(3) .dot { animation-duration: 1800ms; }
  [data-deck-active] .s-conv__agent.idle .dot { animation: none; background: rgba(255,255,255,0.25); }
  @keyframes convAgentPulse {
    0%   { box-shadow: 0 0 0 0 rgba(221,244,91,0.55); }
    70%  { box-shadow: 0 0 0 6px rgba(221,244,91,0); }
    100% { box-shadow: 0 0 0 0 rgba(221,244,91,0); }
  }
  .s-conv__agent .nm {
    color: rgba(255,255,255,0.95);
  }
  .s-conv__agent.idle .nm { color: rgba(255,255,255,0.55); }
  .s-conv__agent .rate {
    color: var(--wisy-lime);
    font-weight: 600;
    font-size: 11px;
  }
  .s-conv__agent.idle .rate {
    color: var(--wisy-indigo-200);
    font-weight: 400;
  }
  .s-conv__agent .rate em {
    font-style: normal;
    font-variant-numeric: tabular-nums;
  }
  .s-conv__agent .bar {
    width: 70px; height: 4px;
    background: rgba(255,255,255,0.10);
    border-radius: 999px;
    overflow: hidden;
    position: relative;
  }
  .s-conv__agent .bar i {
    display: block;
    height: 100%;
    width: var(--w, 50%);
    background: var(--wisy-lime);
    border-radius: 999px;
    transform-origin: left;
  }
  [data-deck-active] .s-conv__agent .bar i {
    animation: convAgentBar 2200ms var(--ease-in-out) infinite;
  }
  [data-deck-active] .s-conv__agent:nth-child(1) .bar i { animation-duration: 1900ms; }
  [data-deck-active] .s-conv__agent:nth-child(2) .bar i { animation-duration: 2600ms; animation-delay: -300ms; }
  [data-deck-active] .s-conv__agent:nth-child(3) .bar i { animation-duration: 2200ms; animation-delay: -500ms; }
  [data-deck-active] .s-conv__agent.idle .bar i { animation: none; opacity: 0.5; background: var(--wisy-indigo-300); }
  @keyframes convAgentBar {
    0%, 100% { transform: scaleX(0.65); }
    50%      { transform: scaleX(1.0); }
  }

  /* Activity log (ticker inside core) */
  .s-conv__log {
    margin-top: 12px;
    height: 72px;
    overflow: hidden;
    border-top: 1px solid rgba(255,255,255,0.08);
    padding-top: 8px;
    position: relative;
    -webkit-mask: linear-gradient(180deg, transparent 0%, #000 25%, #000 75%, transparent 100%);
            mask: linear-gradient(180deg, transparent 0%, #000 25%, #000 75%, transparent 100%);
  }
  .s-conv__logRow {
    display: grid;
    grid-template-columns: 88px 1fr auto;
    gap: 10px;
    align-items: center;
    font-family: var(--font-mono);
    font-size: 11px;
    color: rgba(255,255,255,0.78);
    line-height: 1.4;
    height: 22px;
    white-space: nowrap;
    overflow: hidden;
  }
  .s-conv__logRow .t {
    color: rgba(255,255,255,0.35);
    font-size: 10px;
    letter-spacing: 0.02em;
  }
  .s-conv__logRow .m {
    color: rgba(255,255,255,0.9);
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .s-conv__logRow .m em {
    font-style: normal;
    color: var(--wisy-indigo-200);
  }
  .s-conv__logRow .v {
    font-weight: 600;
    font-size: 11px;
  }
  .s-conv__logRow .v.ok { color: var(--wisy-success); }
  .s-conv__logRow .v.hi { color: var(--wisy-lime); }

  [data-deck-active] .s-conv__log .s-conv__logRow {
    animation: convLogScroll 6s linear infinite;
  }
  [data-deck-active] .s-conv__log .s-conv__logRow.r0 { animation-delay: 0s; }
  [data-deck-active] .s-conv__log .s-conv__logRow.r1 { animation-delay: -1s; }
  [data-deck-active] .s-conv__log .s-conv__logRow.r2 { animation-delay: -2s; }
  [data-deck-active] .s-conv__log .s-conv__logRow.r3 { animation-delay: -3s; }
  [data-deck-active] .s-conv__log .s-conv__logRow.r4 { animation-delay: -4s; }
  [data-deck-active] .s-conv__log .s-conv__logRow.r5 { animation-delay: -5s; }
  @keyframes convLogScroll {
    0%   { transform: translateY(72px); opacity: 0; }
    10%  { opacity: 1; }
    50%  { transform: translateY(0); opacity: 1; }
    90%  { transform: translateY(-72px); opacity: 1; }
    100% { transform: translateY(-72px); opacity: 0; }
  }
  .s-conv__log {
    /* let absolute children stack */
    position: relative;
  }
  .s-conv__log .s-conv__logRow {
    position: absolute;
    left: 0; right: 0;
    top: 8px;
  }

  /* Outcomes column (right) */
  .s-conv__outcomes {
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
    width: 400px;
    display: flex; flex-direction: column; gap: 10px;
    z-index: 2;
  }
  .s-conv__out {
    background: var(--wisy-white);
    border-radius: 14px;
    padding: 14px 20px;
    border: 1px solid var(--border-1);
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 16px;
    align-items: center;
  }
  [data-deck-active] .s-conv__out {
    animation: convOutIn 480ms var(--ease-out) both;
  }
  [data-deck-active] .s-conv__out:nth-child(1) { animation-delay: 900ms; }
  [data-deck-active] .s-conv__out:nth-child(2) { animation-delay: 1050ms; }
  [data-deck-active] .s-conv__out:nth-child(3) { animation-delay: 1200ms; }
  [data-deck-active] .s-conv__out:nth-child(4) { animation-delay: 1350ms; }
  @keyframes convOutIn {
    from { opacity: 0; transform: translateX(24px); }
    to   { opacity: 1; transform: translateX(0); }
  }
  .s-conv__out.hero {
    background: var(--wisy-lime);
    border: none;
  }
  .s-conv__out .v {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 36px;
    line-height: 1;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 0;
    white-space: nowrap;
  }
  .s-conv__out.hero .v { font-size: 44px; }
  .s-conv__out .l {
    font-family: var(--font-sans);
    font-size: 16px;
    color: var(--fg-2);
    line-height: 1.3;
    margin: 0;
  }
  .s-conv__out.hero .l { color: var(--wisy-black); font-weight: 500; }

  /* SVG paths */
  /* Outcome value flash + sparkle when a new decision arrives */
  .s-conv__out .v { transition: transform var(--dur-base) var(--ease-out); }
  [data-deck-active] .s-conv__out .v {
    animation: convOutFlash 4.4s var(--ease-out) infinite;
  }
  [data-deck-active] .s-conv__out:nth-child(1) .v { animation-delay: 0.0s; }
  [data-deck-active] .s-conv__out:nth-child(2) .v { animation-delay: 1.1s; }
  [data-deck-active] .s-conv__out:nth-child(3) .v { animation-delay: 2.2s; }
  [data-deck-active] .s-conv__out:nth-child(4) .v { animation-delay: 3.3s; }
  @keyframes convOutFlash {
    0%, 92%, 100% { transform: scale(1); }
    4%  { transform: scale(1.08); }
    10% { transform: scale(1); }
  }
  .s-conv__out {
    position: relative;
  }
  .s-conv__out::after {
    content: "";
    position: absolute; inset: 0;
    border-radius: inherit;
    box-shadow: 0 0 0 0 rgba(83,84,237,0);
    pointer-events: none;
  }
  [data-deck-active] .s-conv__out::after {
    animation: convOutGlow 4.4s var(--ease-out) infinite;
  }
  [data-deck-active] .s-conv__out:nth-child(1)::after { animation-delay: 0.0s; }
  [data-deck-active] .s-conv__out:nth-child(2)::after { animation-delay: 1.1s; }
  [data-deck-active] .s-conv__out:nth-child(3)::after { animation-delay: 2.2s; }
  [data-deck-active] .s-conv__out:nth-child(4)::after { animation-delay: 3.3s; }
  @keyframes convOutGlow {
    0%, 100% { box-shadow: 0 0 0 0 rgba(83,84,237,0); }
    3%       { box-shadow: 0 0 0 4px rgba(83,84,237,0.18); }
    12%      { box-shadow: 0 0 0 0 rgba(83,84,237,0); }
  }
  .s-conv__out.hero::after {
    /* lime hero gets a lime glow */
  }
  [data-deck-active] .s-conv__out.hero::after {
    animation-name: convOutGlowHero;
  }
  @keyframes convOutGlowHero {
    0%, 100% { box-shadow: 0 0 0 0 rgba(221,244,91,0); }
    3%       { box-shadow: 0 0 0 6px rgba(221,244,91,0.45); }
    12%      { box-shadow: 0 0 0 0 rgba(221,244,91,0); }
  }

  .s-conv__path {
    fill: none;
    stroke: rgba(83,84,237,0.22);
    stroke-width: 1.5;
    stroke-linecap: round;
    vector-effect: non-scaling-stroke;
  }
  .s-conv__path.out { stroke: rgba(0,0,0,0.18); }
  .s-conv__pathLive {
    fill: none;
    stroke: var(--wisy-indigo);
    stroke-width: 2;
    stroke-linecap: round;
    stroke-dasharray: 4 12;
    stroke-dashoffset: 0;
    vector-effect: non-scaling-stroke;
  }
  [data-deck-active] .s-conv__pathLive {
    animation: convDash 1600ms linear infinite;
  }
  @keyframes convDash {
    to { stroke-dashoffset: -160; }
  }
  .s-conv__pathLive.out { stroke: var(--wisy-lime); }

  .s-conv__legend {
    display: flex; justify-content: space-between; align-items: center;
    border-top: 1px solid var(--border-1);
    padding-top: 18px;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--fg-3);
    flex-shrink: 0;
    position: relative;
    z-index: 2;
  }
  .s-conv__legend strong { color: var(--wisy-black); font-weight: 600; }

  .s-conv__arrow {
    display: flex; flex-direction: column; align-items: center; gap: 16px;
  }
  .s-conv__arrow svg { width: 100%; height: 2px; }
  .s-conv__arrow .lbl {
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-2);
    text-align: center;
    line-height: 1.4;
  }

  /* ============================================================
     SLIDE 8 — Credibility
     ============================================================ */
  .s-cred {
    height: 100%;
    box-sizing: border-box;
    background: var(--wisy-black);
    color: var(--wisy-white);
    padding: 72px var(--pad-x) 72px;
    display: flex;
    flex-direction: column;
    gap: 40px;
    position: relative;
  }
  .s-cred__head h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 64px;
    line-height: 0.98;
    letter-spacing: -0.02em;
    color: var(--wisy-white);
    margin: 18px 0 0;
    text-wrap: balance;
    max-width: 1500px;
  }
  .s-cred__head h2 em { font-style: normal; color: var(--wisy-lime); }

  .s-cred__grid {
    display: grid;
    grid-template-columns: 1.25fr 1fr;
    gap: 40px;
    flex: 1;
    min-height: 0;
  }
  .s-cred__lead {
    background: var(--wisy-indigo);
    border-radius: 28px;
    padding: 40px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: var(--wisy-white);
    position: relative;
    overflow: hidden;
  }
  .s-cred__lead .kicker {
    color: var(--wisy-indigo-200);
  }
  .s-cred__lead .kicker .dot { background: var(--wisy-lime); }
  .s-cred__lead .lockup {
    margin: 24px 0;
    display: flex; align-items: center;
    gap: 20px;
  }
  .s-cred__lead .lockup .wisy {
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 96px;
    letter-spacing: -0.04em;
    line-height: 0.85;
    text-transform: lowercase;
    color: var(--wisy-white);
  }
  .s-cred__lead .lockup .x {
    font-size: 48px; color: var(--wisy-indigo-200);
    font-weight: 300;
  }
  .s-cred__lead .lockup .pal {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 60px;
    letter-spacing: -0.025em;
    color: var(--wisy-lime);
    line-height: 0.9;
  }
  .s-cred__lead p {
    font-size: 24px;
    line-height: 1.4;
    color: rgba(255,255,255,0.85);
    margin: 0;
    max-width: 580px;
  }
  .s-cred__lead p em { color: var(--wisy-lime); font-style: normal; font-weight: 600; }

  .s-cred__flexes {
    display: flex; flex-direction: column; gap: 16px;
  }
  .s-cred__flex {
    background: #0f0f10;
    border: 1px solid rgba(255,255,255,0.1);
    border-radius: 22px;
    padding: 22px 28px;
    flex: 1;
  }
  .s-cred__flex .l {
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--wisy-indigo-200);
    margin: 0 0 10px;
  }
  .s-cred__flex .v {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 28px;
    line-height: 1.15;
    letter-spacing: -0.015em;
    color: var(--wisy-white);
    margin: 0;
    text-wrap: balance;
  }
  .s-cred__flex .v em { color: var(--wisy-lime); font-style: normal; }

  .s-cred__logos {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 20px;
    padding: 20px 0 0;
    border-top: 1px solid rgba(255,255,255,0.12);
    flex-shrink: 0;
  }
  .s-cred__logo {
    display: flex; flex-direction: column; align-items: center; justify-content: center;
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 24px;
    color: rgba(255,255,255,0.6);
    letter-spacing: -0.01em;
    border-right: 1px solid rgba(255,255,255,0.08);
    padding: 8px 0;
  }
  .s-cred__logo:last-child { border-right: none; }
  .s-cred__logo small {
    display: block;
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.35);
    margin-top: 6px;
    font-weight: 400;
  }

  /* ============================================================
     SLIDE 9 — Social proof
     ============================================================ */
  .s-proof {
    height: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 100%;
    overflow: hidden;
  }
  .s-proof__photo {
    position: relative;
    background:
      linear-gradient(180deg, rgba(0,0,0,0.0) 30%, rgba(0,0,0,0.55) 100%),
      url("https://images.unsplash.com/photo-1601598851547-4302969d0614?w=1400&q=80&auto=format&fit=crop") center/cover;
  }
  .s-proof__photo .tag {
    position: absolute;
    top: 56px; left: 56px;
    background: var(--wisy-white);
    color: var(--wisy-black);
    border-radius: 999px;
    padding: 12px 20px;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    font-weight: 500;
    display: flex; align-items: center; gap: 10px;
  }
  .s-proof__photo .tag .dot {
    width: 8px; height: 8px; border-radius: 999px; background: var(--wisy-indigo);
  }
  .s-proof__photo .brandStamp {
    position: absolute;
    left: 56px; bottom: 56px;
    color: var(--wisy-white);
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 56px;
    letter-spacing: -0.02em;
    line-height: 1;
  }
  .s-proof__photo .brandStamp span {
    display: block;
    font-family: var(--font-mono);
    font-weight: 400;
    font-size: 16px;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.85);
    margin-top: 12px;
  }

  .s-proof__right {
    padding: 72px 80px 72px 80px;
    background: var(--wisy-white);
    display: flex;
    flex-direction: column;
    gap: 28px;
    box-sizing: border-box;
    overflow: hidden;
  }
  .s-proof__head h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 56px;
    line-height: 0.98;
    letter-spacing: -0.025em;
    color: var(--wisy-black);
    margin: 18px 0 0;
    text-wrap: balance;
  }

  .s-proof__quote {
    background: var(--wisy-indigo-100);
    border-radius: 22px;
    padding: 26px 32px;
    position: relative;
  }
  .s-proof__quote::before {
    content: "“";
    position: absolute;
    top: -8px; left: 20px;
    font-family: var(--font-sans);
    font-size: 96px;
    line-height: 1;
    color: var(--wisy-indigo);
    font-weight: 600;
  }
  .s-proof__quote p {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 24px;
    line-height: 1.35;
    color: var(--wisy-black);
    margin: 0 0 16px;
    padding-left: 8px;
    text-wrap: balance;
  }
  .s-proof__quote .meta {
    display: flex; align-items: center; gap: 14px;
    padding-left: 8px;
  }
  .s-proof__quote .meta .av {
    width: 44px; height: 44px; border-radius: 999px;
    background: var(--wisy-indigo);
    color: var(--wisy-white);
    display: grid; place-items: center;
    font-weight: 600; font-size: 16px;
  }
  .s-proof__quote .meta .who {
    font-family: var(--font-sans);
    font-size: 18px;
    color: var(--fg-1);
    font-weight: 600;
  }
  .s-proof__quote .meta .who span {
    display: block;
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-2);
    margin-top: 2px;
    font-weight: 400;
  }

  .s-proof__stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: auto;
    padding-top: 24px;
    border-top: 1px solid var(--border-1);
  }
  .s-proof__stat .v {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1;
    letter-spacing: -0.025em;
    color: var(--wisy-indigo);
    margin: 0 0 6px;
  }
  .s-proof__stat .l {
    font-family: var(--font-sans);
    font-size: 16px;
    color: var(--fg-2);
    line-height: 1.35;
    margin: 0;
  }

  /* ============================================================
     SLIDE 10 — Bottom line
     ============================================================ */
  .s-close {
    height: 100%;
    box-sizing: border-box;
    background: var(--wisy-white);
    padding: 72px var(--pad-x) 72px;
    position: relative;
    display: flex;
    flex-direction: column;
    gap: 40px;
  }
  .s-close__head {
    display: flex; justify-content: space-between; align-items: center;
  }
  .s-close__hero {
    display: grid;
    grid-template-columns: 1.05fr 1fr;
    gap: 64px;
    align-items: center;
    flex: 1;
    min-height: 0;
  }
  .s-close__num {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 360px;
    line-height: 0.85;
    letter-spacing: -0.05em;
    color: var(--wisy-indigo);
    margin: 0;
    position: relative;
  }
  .s-close__num .x {
    font-size: 200px;
    color: var(--wisy-black);
    margin-left: -8px;
  }
  .s-close__num .min {
    position: absolute;
    bottom: 24px; right: -8px;
    transform: rotate(-4deg);
    background: var(--wisy-lime);
    color: var(--wisy-black);
    padding: 8px 18px 12px;
    border-radius: 14px;
    font-family: var(--font-mono);
    font-weight: 600;
    font-size: 22px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    line-height: 1;
  }
  .s-close__right h2 {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 48px;
    line-height: 1.02;
    letter-spacing: -0.02em;
    color: var(--wisy-black);
    margin: 18px 0 0;
    text-wrap: balance;
  }
  .s-close__right h2 em { font-style: normal; color: var(--wisy-indigo); }
  .s-close__right .quote {
    font-family: var(--font-sans);
    font-weight: 500;
    font-size: 26px;
    line-height: 1.3;
    color: var(--wisy-white);
    margin: 28px 0 0;
    padding: 24px 28px;
    background: var(--wisy-black);
    border-radius: 20px;
    text-wrap: balance;
  }
  .s-close__right .quote em { font-style: normal; color: var(--wisy-lime); }

  .s-close__cta {
    display: flex; justify-content: space-between; align-items: center;
    border-top: 1px solid var(--border-1);
    padding-top: 28px;
    flex-shrink: 0;
  }
  .s-close__cta .who {
    font-family: var(--font-sans);
    font-weight: 600;
    font-size: 24px;
    color: var(--fg-1);
  }
  .s-close__cta .who span {
    display: block;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-3);
    margin-top: 4px;
    font-weight: 400;
  }
  .s-close__cta .next {
    display: flex; align-items: center; gap: 20px;
    font-family: var(--font-mono);
    font-size: 14px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--fg-2);
  }
  .s-close__cta .next .btn {
    background: var(--wisy-indigo);
    color: var(--wisy-white);
    padding: 16px 26px;
    border-radius: 999px;
    font-weight: 600;
    letter-spacing: 0.08em;
    font-size: 16px;
    box-shadow: var(--shadow-indigo);
  }
</style>
</head>
<body>

<deck-stage width="1920" height="1080">

  <!-- ====================================================
       SLIDE 1 — Title
       ==================================================== -->
  <section data-label="01 Title">
    <div class="s-title">
      <div class="s-title__left">
        <div>
          <p class="kicker"><span class="dot"></span><span>Wisy &middot; Field deck &middot; 2026</span></p>
          <h1 class="s-title__wordmark">wisy:</h1>
        </div>
        <div class="s-title__hook">
          <p class="t">From <em>shelf</em> to <em>HQ</em>.<br/>Real-time shelf intelligence.</p>
          <p class="sub">Photograph the shelf. Wisy ranks the fix list by revenue. Your team acts before they leave the store — your HQ sees it before lunch.</p>
        </div>
        <div class="s-title__meta">
          <span>For CPG &amp; Grocery</span>
          <span class="bar"></span>
          <span>5 min</span>
          <span class="bar"></span>
          <span>Confidential</span>
        </div>
      </div>
      <div class="s-title__right">
        <div class="s-title__rightInner">
          <div class="s-title__mark">w:</div>
          <div class="s-title__statBlock">
            <p class="s-title__stat">250 SKUs.<br/>One photo.</p>
            <p class="s-title__statLbl">The whole shelf, read and ranked — even offline.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 2 — $1.7 trillion
       ==================================================== -->
  <section data-label="02 Stakes">
    <div class="s-stakes">
      <p class="kicker"><span class="dot"></span><span>The stakes &middot; Global retail execution</span></p>

      <div class="s-stakes__hero">
        <p class="s-stakes__number">$1.7T<span class="unit"></span></p>
        <div class="s-stakes__copy">
          <h2>lost every year to bad retail execution.</h2>
          <p>For a $1B brand, that's <strong style="color: var(--wisy-lime)">$20M&nbsp;–&nbsp;$50M</strong> walking off the shelf annually. Out-of-stocks. Wrong planogram. Missed promotion. Quiet, daily revenue leak.</p>
        </div>
      </div>

      <div class="s-stakes__row">
        <div class="s-stakes__cell">
          <p class="n"><span class="accent">1 in 13</span></p>
          <p class="l">items a shopper looks for is out of stock — and most walk away.</p>
        </div>
        <div class="s-stakes__cell">
          <p class="n"><span class="accent">~70%</span></p>
          <p class="l">of trade promotions fail to execute at the shelf as planned.</p>
        </div>
        <div class="s-stakes__cell">
          <p class="n"><span class="accent">14&nbsp;days</span></p>
          <p class="l">average lag from shelf reality to HQ dashboard.</p>
        </div>
        <div class="s-stakes__cell quote">
          <p class="q">“This isn't a technology problem. It's a <strong>data</strong> problem.”</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 3 — Ground reality
       ==================================================== -->
  <section data-label="03 Ground reality">
    <div class="s-ground">
      <div class="s-ground__photo">
        <div class="s-ground__rep">
          <div class="nameRow">
            <div class="avatar">MR</div>
            <div class="name">
              Maria R.
              <span>Field rep &middot; Store 0412 &middot; 11:42</span>
            </div>
          </div>
          <div class="s-ground__chips">
            <span class="c">7 active apps</span>
            <span class="c warn">12 OOS suspected</span>
            <span class="c">3 promos to audit</span>
          </div>
        </div>
      </div>
      <div class="s-ground__right">
        <div class="s-ground__title">
          <p class="kicker"><span class="dot"></span><span>The ground reality</span></p>
          <h2>By the time HQ sees the data, the <em>shelf has already changed.</em></h2>
        </div>

        <div class="s-ground__chaos">
          <div class="s-ground__chaosRow">
            <div class="app" style="background: #2a72e0">A</div>
            <div class="lbl">Audit app — manual photo + tag, 90s per shelf</div>
            <span class="tag">no AI</span>
          </div>
          <div class="s-ground__chaosRow">
            <div class="app" style="background: #5e2cbf">B</div>
            <div class="lbl">Route planner — separate login, no shelf context</div>
            <span class="tag">disconnected</span>
          </div>
          <div class="s-ground__chaosRow">
            <div class="app" style="background: #c0392b">C</div>
            <div class="lbl">Promo form — paper PDF, signed at checkout</div>
            <span class="tag">offline only</span>
          </div>
        </div>

        <p class="s-ground__quote">Reps drown in tabs, guess what matters, and leave. The opportunity is <em>gone</em> before the photo reaches HQ.</p>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 4 — AIR
       ==================================================== -->
  <section data-label="04 AIR">
    <div class="s-air">
      <div class="s-air__left">
        <div>
          <p class="kicker"><span class="dot"></span><span>Product 01 &middot; The capture layer</span></p>
          <div class="s-air__brand">
            <div class="name">AIR<span style="color: var(--wisy-black); font-size: 60px; vertical-align: 18px;">.</span></div>
            <div class="expand">Agentic<br/>Image<br/>Recognition</div>
          </div>
          <p class="s-air__pitch">The <em>cheapest robot</em> on every shelf — it lives in the rep's pocket.</p>
        </div>

        <div>
          <div class="s-air__bars">
            <div class="s-air__bar legacy">
              <div class="row">
                <span class="l">Legacy image recognition</span>
                <span class="r">Stops at HQ</span>
              </div>
              <div class="track"><div class="fill"></div></div>
            </div>
            <div class="s-air__bar air">
              <div class="row">
                <span class="l">AIR — agentic, multimodal</span>
                <span class="r">Action at the shelf</span>
              </div>
              <div class="track"><div class="fill"></div></div>
            </div>
          </div>

          <div class="s-air__caps">
            <span class="s-air__cap">Phones &amp; tablets</span>
            <span class="s-air__cap">Cooler cameras</span>
            <span class="s-air__cap">IoT sensors</span>
            <span class="s-air__cap">Offline-first</span>
            <span class="s-air__cap">Built for 2026 AI</span>
          </div>
        </div>
      </div>

      <div class="s-air__right">
        <div class="s-air__hub">
          <svg class="s-air__hubSvg" viewBox="0 0 1000 1000" preserveAspectRatio="none" aria-hidden="true">
            <defs>
              <path id="airL1" d="M500,500 L500,170"/>
              <path id="airL2" d="M500,500 L814,398"/>
              <path id="airL3" d="M500,500 L694,766"/>
              <path id="airL4" d="M500,500 L306,766"/>
              <path id="airL5" d="M500,500 L186,398"/>
            </defs>

            <use href="#airL1" class="s-air__hubPath"/>
            <use href="#airL2" class="s-air__hubPath"/>
            <use href="#airL3" class="s-air__hubPath"/>
            <use href="#airL4" class="s-air__hubPath"/>
            <use href="#airL5" class="s-air__hubPath"/>
            <use href="#airL1" class="s-air__hubPathLive"/>
            <use href="#airL2" class="s-air__hubPathLive" style="animation-delay:-150ms"/>
            <use href="#airL3" class="s-air__hubPathLive" style="animation-delay:-300ms"/>
            <use href="#airL4" class="s-air__hubPathLive" style="animation-delay:-450ms"/>
            <use href="#airL5" class="s-air__hubPathLive" style="animation-delay:-600ms"/>

            <!-- Pulses traveling from device → core (reversed direction via keyPoints 1→0) -->
            <circle r="6" fill="#5354ED"><animateMotion dur="1.8s" begin="0s"   repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL1"/></animateMotion></circle>
            <circle r="6" fill="#5354ED"><animateMotion dur="1.8s" begin="0.4s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL2"/></animateMotion></circle>
            <circle r="6" fill="#5354ED"><animateMotion dur="1.8s" begin="0.8s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL3"/></animateMotion></circle>
            <circle r="6" fill="#5354ED"><animateMotion dur="1.8s" begin="1.2s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL4"/></animateMotion></circle>
            <circle r="6" fill="#5354ED"><animateMotion dur="1.8s" begin="1.6s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL5"/></animateMotion></circle>

            <circle r="6" fill="#DDF45B" stroke="#000" stroke-width="1"><animateMotion dur="1.8s" begin="0.2s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL1"/></animateMotion></circle>
            <circle r="6" fill="#DDF45B" stroke="#000" stroke-width="1"><animateMotion dur="1.8s" begin="0.6s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL3"/></animateMotion></circle>
            <circle r="6" fill="#DDF45B" stroke="#000" stroke-width="1"><animateMotion dur="1.8s" begin="1.0s" repeatCount="indefinite" keyTimes="0;1" keyPoints="1;0"><mpath href="#airL5"/></animateMotion></circle>
          </svg>

          <!-- Center AIR core -->
          <div class="s-air__core">
            <span class="s-air__coreLbl">Capture layer</span>
            <span class="s-air__coreMark">AIR</span>
            <span class="s-air__coreStatus"><span class="d"></span>Multimodal</span>
          </div>

          <!-- Device 1: Phone (top) -->
          <div class="s-air__dev d1" style="left:50%; top:17%;">
            <div class="s-air__devIcon">
              <svg viewBox="0 0 24 24"><rect x="7" y="2.5" width="10" height="19" rx="2.2"/><line x1="10.5" y1="18.5" x2="13.5" y2="18.5"/><line x1="10" y1="4.5" x2="14" y2="4.5"/></svg>
            </div>
            <div class="s-air__devLbl">Phone</div>
            <div class="s-air__devMeta">iOS / Android</div>
            <div class="s-air__devOnline"><span class="d"></span>Live</div>
          </div>

          <!-- Device 2: Tablet (right) -->
          <div class="s-air__dev d2" style="left:81.4%; top:39.8%;">
            <div class="s-air__devIcon">
              <svg viewBox="0 0 24 24"><rect x="3" y="4.5" width="18" height="15" rx="2.2"/><line x1="11" y1="17" x2="13" y2="17"/></svg>
            </div>
            <div class="s-air__devLbl">Tablet</div>
            <div class="s-air__devMeta">In-store kiosk</div>
            <div class="s-air__devOnline"><span class="d"></span>Live</div>
          </div>

          <!-- Device 3: IoT (bottom-right) -->
          <div class="s-air__dev d3" style="left:69.4%; top:76.6%;">
            <div class="s-air__devIcon">
              <svg viewBox="0 0 24 24"><rect x="4" y="7" width="16" height="11" rx="2"/><path d="M9 7 V4.5"/><path d="M15 7 V4.5"/><circle cx="9" cy="12.5" r="1"/><circle cx="15" cy="12.5" r="1"/><line x1="8" y1="21" x2="16" y2="21"/></svg>
            </div>
            <div class="s-air__devLbl">IoT sensor</div>
            <div class="s-air__devMeta">Shelf + weight</div>
            <div class="s-air__devOnline"><span class="d"></span>Live</div>
          </div>

          <!-- Device 4: Cooler camera (bottom-left) -->
          <div class="s-air__dev d4" style="left:30.6%; top:76.6%;">
            <div class="s-air__devIcon">
              <svg viewBox="0 0 24 24"><rect x="3" y="7" width="18" height="13" rx="2"/><path d="M8 7 L9.5 4.5 H14.5 L16 7"/><circle cx="12" cy="13.5" r="3.2"/><circle cx="12" cy="13.5" r="1.2" fill="currentColor" stroke="none"/></svg>
            </div>
            <div class="s-air__devLbl">Cooler camera</div>
            <div class="s-air__devMeta">Always-on shelf</div>
            <div class="s-air__devOnline"><span class="d"></span>Live</div>
          </div>

          <!-- Device 5: Meta glasses (left) -->
          <div class="s-air__dev d5" style="left:18.6%; top:39.8%;">
            <div class="s-air__devIcon">
              <svg viewBox="0 0 24 24"><circle cx="6.5" cy="14.5" r="3.8"/><circle cx="17.5" cy="14.5" r="3.8"/><path d="M10.3 14 L13.7 14"/><path d="M2.5 12 L4 11"/><path d="M21.5 12 L20 11"/></svg>
            </div>
            <div class="s-air__devLbl">Meta Glasses</div>
            <div class="s-air__devMeta">Hands-free capture</div>
            <div class="s-air__devOnline"><span class="d"></span>Live</div>
          </div>
        </div>

        <div class="s-air__caption">
          <span class="lbl">· AIR network</span>
          <span>5 device classes · <em>one</em> capture layer · <span class="v">offline-first</span></span>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 5 — Agents
       ==================================================== -->
  <section data-label="05 Agents">
    <div class="s-agents">
      <div class="s-agents__head">
        <div>
          <p class="kicker"><span class="dot"></span><span>Product 02 &middot; The action layer</span></p>
          <h2>An <em>AI teammate</em> in every rep's pocket — three ranked actions, every visit.</h2>
        </div>
        <p>Raw data is noise. Wisy's Agents apply your business rules to every photo and surface the three highest-revenue actions before the rep leaves the aisle.</p>
      </div>

      <div class="s-agents__flow">
        <!-- Left: phone -->
        <div class="s-agents__phone">
          <div class="s-agents__phoneScreen">
            <div class="s-agents__phoneHead">
              <span class="b">wisy:</span>
              <span class="t">Store 0412 &middot; Aisle 4</span>
            </div>
            <div class="s-agents__photoCap"><span class="check">Captured</span></div>
            <p class="s-agents__phoneSub">Next best actions &middot; ranked by revenue</p>
            <div class="s-agents__action top">
              <div class="ahdr"><span>01 &middot; Refill</span><span class="pri">Priority</span></div>
              <div class="ttl">Restock Coca-Cola 600ml — 4 facings missing</div>
              <div class="rev">+$840 / visit</div>
            </div>
            <div class="s-agents__action">
              <div class="ahdr"><span>02 &middot; Compliance</span><span>Promo</span></div>
              <div class="ttl">Rebuild promo end-cap — Nestlé summer block</div>
              <div class="rev">+$520 / visit</div>
            </div>
            <div class="s-agents__action">
              <div class="ahdr"><span>03 &middot; Planogram</span><span>Fix</span></div>
              <div class="ttl">Swap shelf 3 — competitor in your slot</div>
              <div class="rev">+$310 / visit</div>
            </div>
          </div>
        </div>

        <!-- Middle: pipeline -->
        <div class="s-agents__pipe">
          <div class="s-agents__step">
            <div class="num">1</div>
            <div class="body">
              <p class="lbl">Capture</p>
              <p class="t">One photo of the shelf</p>
            </div>
            <span class="time">0:00</span>
          </div>
          <div class="s-agents__pipeArrow">↓</div>
          <div class="s-agents__step">
            <div class="num indigo">2</div>
            <div class="body">
              <p class="lbl">Apply rules</p>
              <p class="t">Brand &times; planogram &times; promo &times; price</p>
            </div>
            <span class="time">0:01</span>
          </div>
          <div class="s-agents__pipeArrow">↓</div>
          <div class="s-agents__step">
            <div class="num lime">3</div>
            <div class="body">
              <p class="lbl">Rank &amp; act</p>
              <p class="t"><em>Three</em> revenue-ranked next actions</p>
            </div>
            <span class="time">0:02</span>
          </div>
        </div>

        <!-- Right: outcomes -->
        <div class="s-agents__out">
          <h3>What it changes for the rep</h3>
          <div class="s-agents__outCard">
            <p class="v">30min<span class="small"> → 0</span></p>
            <p class="l">Time spent guessing what matters at this store today</p>
          </div>
          <div class="s-agents__outCard">
            <p class="v">+25%</p>
            <p class="l">Field-team efficiency, measured by actions closed per visit</p>
          </div>
          <div class="s-agents__outCard dark">
            <p class="v">3 / visit</p>
            <p class="l">High-confidence fixes, ranked by recovered revenue</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 6 — HQI
       ==================================================== -->
  <section data-label="06 HQI">
    <div class="s-hqi">
      <div class="s-hqi__head">
        <div>
          <p class="kicker"><span class="dot"></span><span>Product 03 &middot; The intelligence layer</span></p>
          <h2><em>HQI</em> — the shelf, wired straight to HQ.</h2>
        </div>
        <p>Not a dashboard. Not BI. <strong>HQI</strong> is the intelligence layer that pulls every shelf in every store into one live operating picture — and pushes actions back down.</p>
      </div>

      <div class="s-hqi__mac" style="position: relative;">
        <div class="s-hqi__macBar">
          <span class="dot r"></span><span class="dot y"></span><span class="dot g"></span>
          <span class="url">hq.wisy.ai &nbsp;/&nbsp; <b>execution / live</b></span>
        </div>
        <div class="s-hqi__app">
          <div class="s-hqi__sidebar">
            <div class="logo">wisy:</div>
            <div class="nav active"><span class="ic"></span>Live execution</div>
            <div class="nav"><span class="ic"></span>Share of shelf</div>
            <div class="nav"><span class="ic"></span>Out of stock</div>
            <div class="nav"><span class="ic"></span>Planogram</div>
            <div class="nav"><span class="ic"></span>Promotions</div>
            <div class="nav"><span class="ic"></span>Field team</div>
            <div class="nav"><span class="ic"></span>Routes</div>
            <div class="nav"><span class="ic"></span>Reports</div>
          </div>
          <div class="s-hqi__main">
            <div class="s-hqi__topRow">
              <h3>Live execution <span>&middot; Latin America &middot; 4,212 stores</span></h3>
              <span class="live">Live &middot; 2s lag</span>
            </div>
            <div class="s-hqi__kpis">
              <div class="s-hqi__kpi">
                <p class="l">On-shelf availability</p>
                <p class="v">94.1<small style="font-size: 22px">%</small></p>
                <p class="d">▲ 2.4 vs. last week</p>
              </div>
              <div class="s-hqi__kpi">
                <p class="l">Share of shelf</p>
                <p class="v">38.6<small style="font-size: 22px">%</small></p>
                <p class="d">▲ 1.1</p>
              </div>
              <div class="s-hqi__kpi">
                <p class="l">Promo compliance</p>
                <p class="v">81<small style="font-size: 22px">%</small></p>
                <p class="d bad">▼ 3.2 — Region 04</p>
              </div>
              <div class="s-hqi__kpi">
                <p class="l">Revenue at risk</p>
                <p class="v">$184<small style="font-size: 22px">K</small></p>
                <p class="d">recoverable this week</p>
              </div>
            </div>

            <div class="s-hqi__panels">
              <div class="s-hqi__panel">
                <h4>Compliance heatmap — by store cluster<span class="pill">last 24h</span></h4>
                <div class="s-hqi__heat" id="heat"></div>
              </div>
              <div class="s-hqi__panel">
                <h4>Ranked alerts — push to field<span class="pill">12 open</span></h4>
                <div class="s-hqi__alerts">
                  <div class="s-hqi__alert danger">
                    <span class="bar"></span>
                    <div class="body">OOS cluster — Coca-Cola 2L, 38 stores São Paulo<small>Region 02 &middot; opened 4m ago</small></div>
                    <span class="rev">+$42K</span>
                  </div>
                  <div class="s-hqi__alert warn">
                    <span class="bar"></span>
                    <div class="body">Promo block missing — Nestlé summer end-cap<small>Region 04 &middot; 21 stores</small></div>
                    <span class="rev">+$28K</span>
                  </div>
                  <div class="s-hqi__alert">
                    <span class="bar"></span>
                    <div class="body">Competitor encroachment — shelf 3, Carrefour SP<small>14 stores &middot; planogram drift</small></div>
                    <span class="rev">+$19K</span>
                  </div>
                  <div class="s-hqi__alert warn">
                    <span class="bar"></span>
                    <div class="body">Price mismatch vs. PoS — Ferrero Rocher T16<small>Chile &middot; 9 stores</small></div>
                    <span class="rev">+$12K</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 7 — Agentic flow / Convergence
       ==================================================== -->
  <section data-label="07 Convergence">
    <div class="s-conv">
      <div class="s-conv__head">
        <p class="kicker"><span class="dot"></span><span>The agentic layer &middot; Data convergence</span></p>
        <h2>A fleet of agents, joining your stack into <em>one continuous decision.</em></h2>
        <p>Most retail tools own one workflow. Wisy runs a swarm of specialised agents across sell-in, sell-out, shelf, route and promo — joining them in real time, ranking what matters, and pushing the action to the rep.</p>
      </div>

      <div class="s-conv__diagram">
        <!-- SVG layer: connection paths + traveling pulses -->
        <svg class="s-conv__svg" viewBox="0 0 1000 600" preserveAspectRatio="none" aria-hidden="true">
          <defs>
            <path id="cp-in-1" d="M214,171 C320,171 320,300 393,300"/>
            <path id="cp-in-2" d="M214,235 C320,235 340,300 393,300"/>
            <path id="cp-in-3" d="M214,300 L393,300"/>
            <path id="cp-in-4" d="M214,365 C320,365 340,300 393,300"/>
            <path id="cp-in-5" d="M214,429 C320,429 320,300 393,300"/>
            <path id="cp-out-1" d="M607,300 C680,300 680,192 762,192"/>
            <path id="cp-out-2" d="M607,300 C680,300 680,270 762,270"/>
            <path id="cp-out-3" d="M607,300 C680,300 680,348 762,348"/>
            <path id="cp-out-4" d="M607,300 C680,300 680,426 762,426"/>
          </defs>

          <!-- Static path lines -->
          <use href="#cp-in-1" class="s-conv__path"/>
          <use href="#cp-in-2" class="s-conv__path"/>
          <use href="#cp-in-3" class="s-conv__path"/>
          <use href="#cp-in-4" class="s-conv__path"/>
          <use href="#cp-in-5" class="s-conv__path"/>
          <use href="#cp-out-1" class="s-conv__path out"/>
          <use href="#cp-out-2" class="s-conv__path out"/>
          <use href="#cp-out-3" class="s-conv__path out"/>
          <use href="#cp-out-4" class="s-conv__path out"/>

          <!-- Animated dashed flow on top -->
          <use href="#cp-in-1" class="s-conv__pathLive"/>
          <use href="#cp-in-2" class="s-conv__pathLive" style="animation-delay:-200ms"/>
          <use href="#cp-in-3" class="s-conv__pathLive" style="animation-delay:-400ms"/>
          <use href="#cp-in-4" class="s-conv__pathLive" style="animation-delay:-600ms"/>
          <use href="#cp-in-5" class="s-conv__pathLive" style="animation-delay:-800ms"/>
          <use href="#cp-out-1" class="s-conv__pathLive out" style="animation-delay:-200ms"/>
          <use href="#cp-out-2" class="s-conv__pathLive out" style="animation-delay:-500ms"/>
          <use href="#cp-out-3" class="s-conv__pathLive out" style="animation-delay:-800ms"/>
          <use href="#cp-out-4" class="s-conv__pathLive out" style="animation-delay:-1100ms"/>

          <!-- Traveling token pulses: 3 per inbound path, staggered -->
          <circle r="5" fill="#5354ED"><animateMotion dur="2.4s" begin="0s"    repeatCount="indefinite"><mpath href="#cp-in-1"/></animateMotion></circle>
          <circle r="5" fill="#5354ED"><animateMotion dur="2.4s" begin="0.8s"  repeatCount="indefinite"><mpath href="#cp-in-1"/></animateMotion></circle>
          <circle r="5" fill="#5354ED"><animateMotion dur="2.4s" begin="1.6s"  repeatCount="indefinite"><mpath href="#cp-in-1"/></animateMotion></circle>

          <circle r="5" fill="#DDF45B"><animateMotion dur="2.4s" begin="0.3s"  repeatCount="indefinite"><mpath href="#cp-in-2"/></animateMotion></circle>
          <circle r="5" fill="#DDF45B"><animateMotion dur="2.4s" begin="1.1s"  repeatCount="indefinite"><mpath href="#cp-in-2"/></animateMotion></circle>
          <circle r="5" fill="#DDF45B"><animateMotion dur="2.4s" begin="1.9s"  repeatCount="indefinite"><mpath href="#cp-in-2"/></animateMotion></circle>

          <circle r="5" fill="#A8AFFF"><animateMotion dur="2.4s" begin="0.15s" repeatCount="indefinite"><mpath href="#cp-in-3"/></animateMotion></circle>
          <circle r="5" fill="#A8AFFF"><animateMotion dur="2.4s" begin="0.95s" repeatCount="indefinite"><mpath href="#cp-in-3"/></animateMotion></circle>
          <circle r="5" fill="#A8AFFF"><animateMotion dur="2.4s" begin="1.75s" repeatCount="indefinite"><mpath href="#cp-in-3"/></animateMotion></circle>

          <circle r="5" fill="#000000"><animateMotion dur="2.4s" begin="0.45s" repeatCount="indefinite"><mpath href="#cp-in-4"/></animateMotion></circle>
          <circle r="5" fill="#000000"><animateMotion dur="2.4s" begin="1.25s" repeatCount="indefinite"><mpath href="#cp-in-4"/></animateMotion></circle>
          <circle r="5" fill="#000000"><animateMotion dur="2.4s" begin="2.05s" repeatCount="indefinite"><mpath href="#cp-in-4"/></animateMotion></circle>

          <circle r="5" fill="#1F8A5B"><animateMotion dur="2.4s" begin="0.6s"  repeatCount="indefinite"><mpath href="#cp-in-5"/></animateMotion></circle>
          <circle r="5" fill="#1F8A5B"><animateMotion dur="2.4s" begin="1.4s"  repeatCount="indefinite"><mpath href="#cp-in-5"/></animateMotion></circle>
          <circle r="5" fill="#1F8A5B"><animateMotion dur="2.4s" begin="2.2s"  repeatCount="indefinite"><mpath href="#cp-in-5"/></animateMotion></circle>

          <!-- Outbound: lime pulses going to outcomes -->
          <circle r="6" fill="#DDF45B" stroke="#000" stroke-width="1"><animateMotion dur="2.2s" begin="0.7s" repeatCount="indefinite"><mpath href="#cp-out-1"/></animateMotion></circle>
          <circle r="6" fill="#DDF45B" stroke="#000" stroke-width="1"><animateMotion dur="2.2s" begin="1.8s" repeatCount="indefinite"><mpath href="#cp-out-1"/></animateMotion></circle>

          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="1.1s" repeatCount="indefinite"><mpath href="#cp-out-2"/></animateMotion></circle>
          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="2.2s" repeatCount="indefinite"><mpath href="#cp-out-2"/></animateMotion></circle>

          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="1.5s" repeatCount="indefinite"><mpath href="#cp-out-3"/></animateMotion></circle>
          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="2.6s" repeatCount="indefinite"><mpath href="#cp-out-3"/></animateMotion></circle>

          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="1.9s" repeatCount="indefinite"><mpath href="#cp-out-4"/></animateMotion></circle>
          <circle r="5" fill="#5354ED"><animateMotion dur="2.2s" begin="3.0s" repeatCount="indefinite"><mpath href="#cp-out-4"/></animateMotion></circle>

          <!-- Labeled data packets (less frequent, narrative) -->
          <g class="s-conv__packet">
            <rect x="-30" y="-9" width="60" height="18" rx="9" fill="#5354ED" stroke="#0c0c1e" stroke-width="1"/>
            <text x="0" y="3.5" text-anchor="middle" fill="#fff" font-size="10" font-family="Roboto Mono, monospace" font-weight="500" letter-spacing="0.5">SKU-184</text>
            <animateMotion dur="3.6s" begin="0.3s" repeatCount="indefinite" rotate="0"><mpath href="#cp-in-3"/></animateMotion>
          </g>
          <g class="s-conv__packet">
            <rect x="-26" y="-9" width="52" height="18" rx="9" fill="#DDF45B" stroke="#0c0c1e" stroke-width="1"/>
            <text x="0" y="3.5" text-anchor="middle" fill="#000" font-size="10" font-family="Roboto Mono, monospace" font-weight="600" letter-spacing="0.5">$840</text>
            <animateMotion dur="3.6s" begin="1.8s" repeatCount="indefinite"><mpath href="#cp-in-2"/></animateMotion>
          </g>
          <g class="s-conv__packet">
            <rect x="-22" y="-9" width="44" height="18" rx="9" fill="#fff" stroke="#0c0c1e" stroke-width="1"/>
            <text x="0" y="3.5" text-anchor="middle" fill="#000" font-size="10" font-family="Roboto Mono, monospace" font-weight="600" letter-spacing="0.5">OOS</text>
            <animateMotion dur="3.6s" begin="2.7s" repeatCount="indefinite"><mpath href="#cp-in-1"/></animateMotion>
          </g>

          <!-- Outbound packets: ranked decisions -->
          <g class="s-conv__packet">
            <rect x="-44" y="-10" width="88" height="20" rx="10" fill="#DDF45B" stroke="#0c0c1e" stroke-width="1"/>
            <text x="0" y="4" text-anchor="middle" fill="#000" font-size="10" font-family="Roboto Mono, monospace" font-weight="700" letter-spacing="0.5">+$840 ↑ RANK 1</text>
            <animateMotion dur="3.2s" begin="0.8s" repeatCount="indefinite"><mpath href="#cp-out-1"/></animateMotion>
          </g>
          <g class="s-conv__packet">
            <rect x="-36" y="-10" width="72" height="20" rx="10" fill="#0c0c1e" stroke="#5354ED" stroke-width="1"/>
            <text x="0" y="4" text-anchor="middle" fill="#fff" font-size="10" font-family="Roboto Mono, monospace" font-weight="600" letter-spacing="0.5">FIX OOS ×5</text>
            <animateMotion dur="3.2s" begin="1.9s" repeatCount="indefinite"><mpath href="#cp-out-2"/></animateMotion>
          </g>
          <g class="s-conv__packet">
            <rect x="-40" y="-10" width="80" height="20" rx="10" fill="#0c0c1e" stroke="#5354ED" stroke-width="1"/>
            <text x="0" y="4" text-anchor="middle" fill="#fff" font-size="10" font-family="Roboto Mono, monospace" font-weight="600" letter-spacing="0.5">PROMO ✓ NS-12</text>
            <animateMotion dur="3.2s" begin="2.6s" repeatCount="indefinite"><mpath href="#cp-out-3"/></animateMotion>
          </g>
          <g class="s-conv__packet">
            <rect x="-36" y="-10" width="72" height="20" rx="10" fill="#0c0c1e" stroke="#5354ED" stroke-width="1"/>
            <text x="0" y="4" text-anchor="middle" fill="#fff" font-size="10" font-family="Roboto Mono, monospace" font-weight="600" letter-spacing="0.5">REP → 1471</text>
            <animateMotion dur="3.2s" begin="3.3s" repeatCount="indefinite"><mpath href="#cp-out-4"/></animateMotion>
          </g>
        </svg>

        <!-- Streams (left) -->
        <div class="s-conv__streams">
          <div class="s-conv__stream">
            <div class="icon">SI</div>
            <div><p class="lbl">Stream 01 &middot; ERP</p><p class="ttl">Sell-in</p></div>
            <span class="live"></span>
          </div>
          <div class="s-conv__stream">
            <div class="icon">SO</div>
            <div><p class="lbl">Stream 02 &middot; PoS</p><p class="ttl">Sell-out</p></div>
            <span class="live"></span>
          </div>
          <div class="s-conv__stream">
            <div class="icon">SH</div>
            <div><p class="lbl">Stream 03 &middot; AIR photos</p><p class="ttl">Shelf truth</p></div>
            <span class="live"></span>
          </div>
          <div class="s-conv__stream">
            <div class="icon">RT</div>
            <div><p class="lbl">Stream 04 &middot; Field GPS</p><p class="ttl">Route &amp; visit</p></div>
            <span class="live"></span>
          </div>
          <div class="s-conv__stream">
            <div class="icon">PR</div>
            <div><p class="lbl">Stream 05 &middot; Calendar</p><p class="ttl">Promo &amp; price</p></div>
            <span class="live"></span>
          </div>
        </div>

        <!-- Core agent orchestrator (center) -->
        <div class="s-conv__core">
          <div class="s-conv__coreHead">
            <div class="s-conv__coreMark">w:</div>
            <span class="s-conv__coreLbl">Agent orchestrator</span>
            <span class="s-conv__coreStatus"><span class="d"></span>Live</span>
          </div>

          <div class="s-conv__coreMeter">
            <div class="s-conv__coreMeterTop">
              <span class="l">Throughput</span>
              <span class="v"><em id="convActions">2,481</em><span class="u">actions / sec</span></span>
            </div>
            <div class="s-conv__spark" aria-hidden="true">
              <span style="--h:42%"></span><span style="--h:58%"></span><span style="--h:36%"></span>
              <span style="--h:64%"></span><span style="--h:48%"></span><span style="--h:72%"></span>
              <span style="--h:54%"></span><span style="--h:88%"></span><span style="--h:62%"></span>
              <span style="--h:76%"></span><span style="--h:44%"></span><span style="--h:82%"></span>
              <span style="--h:58%"></span><span style="--h:94%"></span><span style="--h:68%"></span>
              <span style="--h:78%"></span><span style="--h:52%"></span><span style="--h:86%"></span>
            </div>
          </div>

          <div class="s-conv__agents">
            <div class="s-conv__agent">
              <span class="dot"></span>
              <span class="nm">oos-detector</span>
              <span class="rate"><em>3.2k</em>/s</span>
              <span class="bar"><i style="--w:78%"></i></span>
            </div>
            <div class="s-conv__agent">
              <span class="dot"></span>
              <span class="nm">planogram-fix</span>
              <span class="rate"><em>1.8k</em>/s</span>
              <span class="bar"><i style="--w:54%"></i></span>
            </div>
            <div class="s-conv__agent">
              <span class="dot"></span>
              <span class="nm">promo-audit</span>
              <span class="rate"><em>0.9k</em>/s</span>
              <span class="bar"><i style="--w:32%"></i></span>
            </div>
            <div class="s-conv__agent idle">
              <span class="dot"></span>
              <span class="nm">route-optimizer</span>
              <span class="rate">queued</span>
              <span class="bar"><i style="--w:8%"></i></span>
            </div>
          </div>

          <!-- Activity log -->
          <div class="s-conv__log" aria-hidden="true">
            <div class="s-conv__logRow r0"><span class="t">12:42:18.901</span><span class="m">photo → <em>store 0412</em></span><span class="v ok">+187 SKUs</span></div>
            <div class="s-conv__logRow r1"><span class="t">12:42:18.902</span><span class="m">join: sell-out × shelf</span><span class="v ok">+$840</span></div>
            <div class="s-conv__logRow r2"><span class="t">12:42:18.903</span><span class="m">oos-detector ✓ 5 fixes</span><span class="v hi">ranked</span></div>
            <div class="s-conv__logRow r3"><span class="t">12:42:18.904</span><span class="m">action → <em>rep 1471</em></span><span class="v hi">pushed</span></div>
            <div class="s-conv__logRow r4"><span class="t">12:42:18.905</span><span class="m">planogram-fix ✓</span><span class="v ok">+$310</span></div>
            <div class="s-conv__logRow r5"><span class="t">12:42:18.906</span><span class="m">promo-audit → Nestlé</span><span class="v ok">+$520</span></div>
          </div>
        </div>

        <!-- Outcomes (right) -->
        <div class="s-conv__outcomes">
          <div class="s-conv__out hero">
            <p class="v">10×</p>
            <p class="l">Minimum ROI<br/>in year one</p>
          </div>
          <div class="s-conv__out">
            <p class="v">−42%</p>
            <p class="l">Out-of-stocks in 60 days</p>
          </div>
          <div class="s-conv__out">
            <p class="v">+18 pts</p>
            <p class="l">Promo compliance, measured by photo</p>
          </div>
          <div class="s-conv__out">
            <p class="v">−30 min</p>
            <p class="l">Per store visit, returned to the rep</p>
          </div>
        </div>
      </div>

      <div class="s-conv__legend">
        <span>Each join becomes a new question your stack can't ask today.</span>
        <span><strong>Wisy:</strong> the layer above your stack — not another tab inside it.</span>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 8 — Credibility
       ==================================================== -->
  <section data-label="08 Credibility">
    <div class="s-cred">
      <div class="s-cred__head">
        <p class="kicker on-dark"><span class="dot"></span><span>Why this team &middot; Why now</span></p>
        <h2>Silicon Valley horsepower. <em>Backed by Palantir.</em></h2>
      </div>

      <div class="s-cred__grid">
        <div class="s-cred__lead">
          <p class="kicker"><span class="dot"></span><span>Foundational partner</span></p>
          <div class="lockup">
            <div class="wisy">wisy:</div>
            <div class="x">×</div>
            <div class="pal">Palantir</div>
          </div>
          <p>Built on the same data infrastructure that runs the world's hardest operational problems. Wisy is the <em>first AI-native</em> retail execution platform on top of it.</p>
        </div>

        <div class="s-cred__flexes">
          <div class="s-cred__flex">
            <p class="l">Disruption speed</p>
            <p class="v">Models that ship <em>week-over-week</em> — not quarter-over-quarter.</p>
          </div>
          <div class="s-cred__flex">
            <p class="l">Free of legacy drag</p>
            <p class="v">No private-equity stagnation. No 18-month roadmaps.</p>
          </div>
          <div class="s-cred__flex">
            <p class="l">Built for 2026 AI</p>
            <p class="v">Multimodal, agentic, on-device — designed for what models can do <em>now.</em></p>
          </div>
        </div>
      </div>

      <div class="s-cred__logos">
        <div class="s-cred__logo">Palantir<small>Data infrastructure</small></div>
        <div class="s-cred__logo">SV Capital<small>Lead investor</small></div>
        <div class="s-cred__logo">Foundry<small>Platform partner</small></div>
        <div class="s-cred__logo">AWS<small>Compute</small></div>
        <div class="s-cred__logo">NVIDIA<small>Inference</small></div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 9 — Social proof
       ==================================================== -->
  <section data-label="09 Social proof">
    <div class="s-proof">
      <div class="s-proof__photo">
        <div class="tag"><span class="dot"></span>Deployed &middot; Chile</div>
        <div class="brandStamp">CCU<span>Largest brewer &middot; Latin America</span></div>
      </div>
      <div class="s-proof__right">
        <div class="s-proof__head">
          <p class="kicker"><span class="dot"></span><span>Validated in the wild</span></p>
          <h2>Proven where execution is hardest.</h2>
        </div>

        <div class="s-proof__quote">
          <p>Wisy collapsed a 30-minute store audit into <strong>seconds</strong> — and gave our reps the same shelf picture our HQ team sees. We stopped arguing about the data and started fixing the shelf.</p>
          <div class="meta">
            <div class="av">JR</div>
            <div class="who">J. Ramírez<span>VP Field Execution &middot; CCU</span></div>
          </div>
        </div>

        <div class="s-proof__quote" style="background: var(--wisy-gray-50);">
          <p>The first IR vendor where the rep gets value <em>at the shelf</em>, not three weeks later in a PDF.</p>
          <div class="meta">
            <div class="av" style="background: var(--wisy-black)">F</div>
            <div class="who">Director, Trade Marketing<span>Ferrero &middot; LATAM</span></div>
          </div>
        </div>

        <div class="s-proof__stats">
          <div class="s-proof__stat">
            <p class="v">4,200+</p>
            <p class="l">Stores scanned monthly across deployed brands</p>
          </div>
          <div class="s-proof__stat">
            <p class="v">1.8M</p>
            <p class="l">Shelf photos processed by AIR last quarter</p>
          </div>
          <div class="s-proof__stat">
            <p class="v">11</p>
            <p class="l">Countries live in Latin America &amp; EMEA</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ====================================================
       SLIDE 10 — Bottom line
       ==================================================== -->
  <section data-label="10 Close">
    <div class="s-close">
      <div class="s-close__head">
        <p class="kicker"><span class="dot"></span><span>The bottom line</span></p>
        <p class="kicker" style="color: var(--fg-3)"><span>wisy:</span></p>
      </div>

      <div class="s-close__hero">
        <p class="s-close__num">10<span class="x">×</span><span class="min">Minimum</span></p>
        <div class="s-close__right">
          <h2>Projected return on Wisy <em>in year one.</em></h2>
          <p class="quote">Let our competitors chase next-best-actions. <em>We'll build your scaling intelligence layer.</em></p>
        </div>
      </div>

      <div class="s-close__cta">
        <div class="who">Wisy &middot; AI-native retail execution<span>wisy.ai &nbsp;·&nbsp; hello@wisy.ai</span></div>
        <div class="next">
          <span>Next step</span>
          <span class="btn">Pilot in 30 days &nbsp;→</span>
        </div>
      </div>
    </div>
  </section>

</deck-stage>

<script>
/**
 * <deck-stage> — reusable web component for HTML decks.
 *
 * Handles:
 *  (a) speaker notes — reads <script type="application/json" id="speaker-notes">
 *      and posts {slideIndexChanged: N} to the parent window on nav.
 *  (b) keyboard navigation — ←/→, PgUp/PgDn, Space, Home/End, number keys.
 *      On touch devices, tapping the left/right half of the stage goes
 *      prev/next — taps on links, buttons and other interactive slide
 *      content are left alone.
 *  (c) press R to reset to slide 0 (with a tasteful keyboard hint).
 *  (d) bottom-center overlay showing slide count + hints, fades out on idle.
 *  (e) auto-scaling — inner canvas is a fixed design size (default 1920×1080)
 *      scaled with `transform: scale()` to fit the viewport, letterboxed.
 *      Set the `noscale` attribute to render at authored size (1:1) — the
 *      PPTX exporter sets this so its DOM capture sees unscaled geometry.
 *  (f) print — `@media print` lays every slide out as its own page at the
 *      design size, so the browser's Print → Save as PDF produces a clean
 *      one-page-per-slide PDF with no extra setup.
 *  (g) thumbnail rail — resizable left-hand column of per-slide thumbnails
 *      (static clones). Click to navigate; ↑/↓ with a thumbnail focused to
 *      step between slides; drag to reorder; right-click for
 *      Skip / Move up / Move down / Delete (opens a Cancel/Delete confirm
 *      dialog). Drag the rail's right edge to resize; width persists to
 *      localStorage. Skipped slides carry `data-deck-skip`, are dimmed in
 *      the rail, omitted from prev/next navigation, and hidden at print.
 *      The rail is suppressed in presenting mode, in the host's Preview
 *      mode (ViewerMode='none'), on `noscale`, on narrow viewports
 *      (≤640px), and via the `no-rail` attribute. Rail mutations dispatch
 *      a `deckchange`
 *      CustomEvent on the element: detail = {action, from, to, slide}.
 *
 * Slides are HIDDEN, not unmounted. Non-active slides stay in the DOM with
 * `visibility: hidden` + `opacity: 0`, so their state (videos, iframes,
 * form inputs, React trees) is preserved across navigation.
 *
 * Lifecycle event — the component dispatches a `slidechange` CustomEvent on
 * itself whenever the active slide changes (including the initial mount).
 * The event bubbles and composes out of shadow DOM, so you can listen on
 * the <deck-stage> element or on document:
 *
 *   document.querySelector('deck-stage').addEventListener('slidechange', (e) => {
 *     e.detail.index         // new 0-based index
 *     e.detail.previousIndex // previous index, or -1 on init
 *     e.detail.total         // total slide count
 *     e.detail.slide         // the new active slide element
 *     e.detail.previousSlide // the prior slide element, or null on init
 *     e.detail.reason        // 'init' | 'keyboard' | 'click' | 'tap' | 'api'
 *   });
 *
 * Persistence: none at the deck level. The host app keeps the current slide
 * in its own URL (?slide=) and re-delivers it via location.hash on load, so a
 * bare load with no hash always starts at slide 1.
 *
 * Usage:
 *   <style>deck-stage:not(:defined){visibility:hidden}</style>
 *   <deck-stage width="1920" height="1080">
 *     <section data-label="Title">...</section>
 *     <section data-label="Agenda">...</section>
 *   </deck-stage>
 *   <script src="deck-stage.js"></script>
 *
 * The :not(:defined) rule prevents a flash of the first slide at its
 * authored styles before this script runs and attaches the shadow root.
 *
 * Slides are the direct element children of <deck-stage>. Each slide is
 * automatically tagged with:
 *   - data-screen-label="NN Label"   (1-indexed, for comment flow)
 *   - data-om-validate="no_overflowing_text,no_overlapping_text,slide_sized_text"
 */

(() => {
  const DESIGN_W_DEFAULT = 1920;
  const DESIGN_H_DEFAULT = 1080;
  const OVERLAY_HIDE_MS = 1800;
  const VALIDATE_ATTR = 'no_overflowing_text,no_overlapping_text,slide_sized_text';
  const FINE_POINTER_MQ = matchMedia('(hover: hover) and (pointer: fine)');
  const NARROW_MQ = matchMedia('(max-width: 640px)');
  // Slide-authored controls that should keep a tap instead of it navigating.
  const INTERACTIVE_SEL = 'a[href], button, input, select, textarea, summary, label, video[controls], audio[controls], [role="button"], [onclick], [tabindex]:not([tabindex^="-"]), [contenteditable]:not([contenteditable="false" i])';

  const pad2 = (n) => String(n).padStart(2, '0');

  // Label precedence: data-label → data-screen-label (number stripped) → first heading → "Slide".
  const getSlideLabel = (el) => {
    const explicit = el.getAttribute('data-label');
    if (explicit) return explicit;

    const existing = el.getAttribute('data-screen-label');
    if (existing) return existing.replace(/^\s*\d+\s*/, '').trim() || existing;

    const h = el.querySelector('h1, h2, h3, [data-title]');
    const t = h && (h.textContent || '').trim().slice(0, 40);
    if (t) return t;

    return 'Slide';
  };

  const stylesheet = `
    :host {
      position: fixed;
      inset: 0;
      display: block;
      background: #000;
      color: #fff;
      font-family: -apple-system, BlinkMacSystemFont, "Helvetica Neue", Helvetica, Arial, sans-serif;
      overflow: hidden;
      -webkit-tap-highlight-color: transparent;
    }
    /* connectedCallback holds this until document.fonts.ready (capped 2s) so
     * the first visible paint has the deck's real typography + final rail
     * layout. opacity (not visibility) so the active slide can't un-hide
     * itself via the ::slotted([data-deck-active]) visibility:visible rule.
     * Only the stage/rail hide — the black :host background stays, so the
     * iframe doesn't flash the page's default white. */
    :host([data-fonts-pending]) .stage,
    :host([data-fonts-pending]) .rail { opacity: 0; pointer-events: none; }

    .stage {
      position: absolute;
      inset: 0;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .canvas {
      position: relative;
      transform-origin: center center;
      flex-shrink: 0;
      background: #fff;
      will-change: transform;
    }

    /* Slides live in light DOM (via <slot>) so authored CSS still applies.
       We absolutely position each slotted child to stack them. */
    ::slotted(*) {
      position: absolute !important;
      inset: 0 !important;
      width: 100% !important;
      height: 100% !important;
      box-sizing: border-box !important;
      overflow: hidden;
      opacity: 0;
      pointer-events: none;
      visibility: hidden;
    }
    ::slotted([data-deck-active]) {
      opacity: 1;
      pointer-events: auto;
      visibility: visible;
    }

    .overlay {
      position: fixed;
      left: 50%;
      bottom: 22px;
      transform: translate(-50%, 6px) scale(0.92);
      filter: blur(6px);
      display: flex;
      align-items: center;
      gap: 4px;
      padding: 4px;
      background: #000;
      color: #fff;
      border-radius: 999px;
      font-size: 12px;
      font-feature-settings: "tnum" 1;
      letter-spacing: 0.01em;
      opacity: 0;
      pointer-events: none;
      transition: opacity 260ms ease, transform 260ms cubic-bezier(.2,.8,.2,1), filter 260ms ease;
      transform-origin: center bottom;
      z-index: 2147483000;
      user-select: none;
    }
    .overlay[data-visible] {
      opacity: 1;
      pointer-events: auto;
      transform: translate(-50%, 0) scale(1);
      filter: blur(0);
    }

    .btn {
      appearance: none;
      -webkit-appearance: none;
      background: transparent;
      border: 0;
      margin: 0;
      padding: 0;
      color: inherit;
      font: inherit;
      cursor: default;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      height: 28px;
      min-width: 28px;
      border-radius: 999px;
      color: rgba(255,255,255,0.72);
      transition: background 140ms ease, color 140ms ease;
      -webkit-tap-highlight-color: transparent;
    }
    .btn:hover { background: rgba(255,255,255,0.12); color: #fff; }
    .btn:active { background: rgba(255,255,255,0.18); }
    .btn:focus { outline: none; }
    .btn:focus-visible { outline: none; }
    .btn::-moz-focus-inner { border: 0; }
    .btn svg { width: 14px; height: 14px; display: block; }
    .btn.reset {
      font-size: 11px;
      font-weight: 500;
      letter-spacing: 0.02em;
      padding: 0 10px 0 12px;
      gap: 6px;
      color: rgba(255,255,255,0.72);
    }
    .btn.reset .kbd {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-width: 16px;
      height: 16px;
      padding: 0 4px;
      font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
      font-size: 10px;
      line-height: 1;
      color: rgba(255,255,255,0.88);
      background: rgba(255,255,255,0.12);
      border-radius: 4px;
    }

    .count {
      font-variant-numeric: tabular-nums;
      color: #fff;
      font-weight: 500;
      padding: 0 8px;
      min-width: 42px;
      text-align: center;
      font-size: 12px;
    }
    .count .sep { color: rgba(255,255,255,0.45); margin: 0 3px; font-weight: 400; }
    .count .total { color: rgba(255,255,255,0.55); }

    .divider {
      width: 1px;
      height: 14px;
      background: rgba(255,255,255,0.18);
      margin: 0 2px;
    }

    /* ── Thumbnail rail ──────────────────────────────────────────────────
       Fixed column on the left; each thumbnail is a static deep-clone of
       the light-DOM slide scaled into a 16:9 (or design-aspect) frame. The
       stage re-fits around it (see _fit); hidden during present / noscale
       / print so capture geometry and fullscreen output are unchanged. */
    .rail {
      position: fixed;
      left: 0;
      top: 0;
      bottom: 0;
      width: var(--deck-rail-w, 188px);
      background: #141414;
      border-right: 1px solid rgba(255,255,255,0.08);
      overflow-y: auto;
      overflow-x: hidden;
      padding: 12px 10px;
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      gap: 12px;
      z-index: 2147482500;
      scrollbar-width: thin;
      scrollbar-color: rgba(255,255,255,0.18) transparent;
    }
    .rail::-webkit-scrollbar { width: 8px; }
    .rail::-webkit-scrollbar-track { background: transparent; margin: 2px; }
    .rail::-webkit-scrollbar-thumb {
      background: rgba(255,255,255,0.18);
      border-radius: 4px;
      border: 2px solid transparent;
      background-clip: content-box;
    }
    .rail::-webkit-scrollbar-thumb:hover {
      background: rgba(255,255,255,0.28);
      border: 2px solid transparent;
      background-clip: content-box;
    }
    :host([no-rail]) .rail,
    :host([noscale]) .rail { display: none; }
    .rail[data-presenting] { display: none; }
    @media (max-width: 640px) {
      .rail, .rail-resize { display: none; }
    }
    /* User-driven show/hide (the TweaksPanel toggle) slides instead of
       popping. Transitions are gated on :host([data-rail-anim]) — set only
       for the 200ms around the toggle — so window-resize and rail-width
       drag (which also call _fit) don't lag behind the cursor. */
    .rail[data-user-hidden] { transform: translateX(-100%); }
    :host([data-rail-anim]) .rail { transition: transform 200ms cubic-bezier(.3,.7,.4,1); }
    :host([data-rail-anim]) .stage { transition: left 200ms cubic-bezier(.3,.7,.4,1); }
    :host([data-rail-anim]) .canvas { transition: transform 200ms cubic-bezier(.3,.7,.4,1); }
    /* transition shorthand replaces rather than merges — repeat the base
       .overlay opacity/transform/filter transitions so visibility changes
       during the 200ms toggle window still fade instead of popping. */
    :host([data-rail-anim]) .overlay {
      transition: margin-left 200ms cubic-bezier(.3,.7,.4,1),
                  opacity 260ms ease,
                  transform 260ms cubic-bezier(.2,.8,.2,1),
                  filter 260ms ease;
    }

    .thumb {
      position: relative;
      display: flex;
      align-items: flex-start;
      gap: 8px;
      cursor: pointer;
      user-select: none;
    }
    .thumb .num {
      width: 16px;
      flex-shrink: 0;
      font-size: 11px;
      font-weight: 500;
      text-align: right;
      color: rgba(255,255,255,0.55);
      padding-top: 2px;
      font-variant-numeric: tabular-nums;
    }
    .thumb .frame {
      position: relative;
      flex: 1;
      min-width: 0;
      aspect-ratio: var(--deck-aspect);
      background: #fff;
      border-radius: 4px;
      outline: 2px solid transparent;
      outline-offset: 0;
      overflow: hidden;
      transition: outline-color 120ms ease;
    }
    .thumb:hover .frame { outline-color: rgba(255,255,255,0.25); }
    .thumb { outline: none; }
    .thumb:focus-visible .frame { outline-color: rgba(255,255,255,0.5); }
    .thumb[data-current] .num { color: #fff; }
    .thumb[data-current] .frame { outline-color: #D97757; }
    .thumb[data-dragging] { opacity: 0.35; }
    .thumb::before {
      content: '';
      position: absolute;
      left: 24px;
      right: 0;
      height: 3px;
      border-radius: 2px;
      background: #D97757;
      opacity: 0;
      pointer-events: none;
    }
    .thumb[data-drop="before"]::before { top: -8px; opacity: 1; }
    .thumb[data-drop="after"]::before { bottom: -8px; opacity: 1; }
    .thumb[data-skip] .frame { opacity: 0.35; }
    .thumb[data-skip] .frame::after {
      content: 'Skipped';
      position: absolute;
      inset: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      background: rgba(0,0,0,0.45);
      color: #fff;
      font-size: 10px;
      font-weight: 500;
      letter-spacing: 0.04em;
    }

    .ctxmenu {
      position: fixed;
      min-width: 150px;
      padding: 4px;
      background: #242424;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 7px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.45);
      z-index: 2147483100;
      display: none;
      font-size: 12px;
    }
    .ctxmenu[data-open] { display: block; }
    .ctxmenu button {
      display: block;
      width: 100%;
      appearance: none;
      border: 0;
      background: transparent;
      color: #e8e8e8;
      font: inherit;
      text-align: left;
      padding: 6px 10px;
      border-radius: 4px;
      cursor: pointer;
    }
    .ctxmenu button:hover:not(:disabled) { background: rgba(255,255,255,0.08); }
    .ctxmenu button:disabled { opacity: 0.35; cursor: default; }
    .ctxmenu hr {
      border: 0;
      border-top: 1px solid rgba(255,255,255,0.1);
      margin: 4px 2px;
    }

    .rail-resize {
      position: fixed;
      left: calc(var(--deck-rail-w, 188px) - 3px);
      top: 0;
      bottom: 0;
      width: 6px;
      cursor: col-resize;
      z-index: 2147482600;
      touch-action: none;
    }
    .rail-resize:hover,
    .rail-resize[data-dragging] { background: rgba(255,255,255,0.12); }
    :host([no-rail]) .rail-resize,
    :host([noscale]) .rail-resize,
    .rail[data-presenting] + .rail-resize,
    .rail[data-user-hidden] + .rail-resize { display: none; }

    /* Delete-confirm popup — matches the SPA's ConfirmDialog layout
       (title + message body, depressed footer with Cancel / Delete). */
    .confirm-backdrop {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.45);
      z-index: 2147483200;
      display: none;
      align-items: center;
      justify-content: center;
    }
    .confirm-backdrop[data-open] { display: flex; }
    .confirm {
      width: 320px;
      max-width: calc(100vw - 32px);
      background: #2a2a2a;
      color: #e8e8e8;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 12px;
      box-shadow: 0 12px 32px rgba(0,0,0,0.5);
      overflow: hidden;
      font-family: inherit;
      animation: deck-confirm-in 0.18s ease;
    }
    @keyframes deck-confirm-in {
      from { opacity: 0; transform: scale(0.96); }
      to { opacity: 1; transform: scale(1); }
    }
    .confirm .body { padding: 20px 20px 16px; }
    .confirm .title { font-size: 14px; font-weight: 600; margin-bottom: 4px; }
    .confirm .msg { font-size: 13px; line-height: 1.5; color: rgba(255,255,255,0.65); }
    .confirm .footer {
      padding: 14px 20px;
      background: #1f1f1f;
      border-top: 1px solid rgba(255,255,255,0.08);
      display: flex;
      justify-content: flex-end;
      gap: 8px;
    }
    .confirm button {
      appearance: none;
      font: inherit;
      font-size: 13px;
      font-weight: 500;
      padding: 8px 16px;
      border-radius: 8px;
      cursor: pointer;
    }
    .confirm .cancel {
      background: transparent;
      border: 0;
      color: rgba(255,255,255,0.8);
    }
    .confirm .cancel:hover { background: rgba(255,255,255,0.08); }
    .confirm .danger {
      background: #c96442;
      border: 1px solid rgba(0,0,0,0.15);
      color: #fff;
      box-shadow: 0 1px 3px rgba(166,50,68,0.3), 0 2px 6px rgba(166,50,68,0.18);
    }
    .confirm .danger:hover { background: #b5563a; }

    /* ── Print: one page per slide, no chrome ────────────────────────────
       The screen layout stacks every slide at inset:0 inside a scaled
       canvas; for print we want them in document flow at the authored
       design size so the browser paginates one slide per sheet. The
       @page size is set from the width/height attributes via the inline
       <style id="deck-stage-print-page"> that connectedCallback injects
       into <head> (the @page at-rule has no effect inside shadow DOM). */
    @media print {
      :host {
        position: static;
        inset: auto;
        background: none;
        overflow: visible;
        color: inherit;
      }
      .stage { position: static; display: block; }
      .canvas {
        transform: none !important;
        width: auto !important;
        height: auto !important;
        background: none;
        will-change: auto;
      }
      ::slotted(*) {
        position: relative !important;
        inset: auto !important;
        width: var(--deck-design-w) !important;
        height: var(--deck-design-h) !important;
        box-sizing: border-box !important;
        opacity: 1 !important;
        visibility: visible !important;
        pointer-events: auto;
        break-after: page;
        page-break-after: always;
        break-inside: avoid;
        overflow: hidden;
      }
      /* :last-child alone isn't enough once data-deck-skip hides the
         trailing slide(s) — the last *visible* slide still carries
         break-after:page and prints a blank sheet. _markLastVisible()
         maintains data-deck-last-visible on the last non-skipped slide. */
      ::slotted(*:last-child),
      ::slotted([data-deck-last-visible]) {
        break-after: auto;
        page-break-after: auto;
      }
      ::slotted([data-deck-skip]) { display: none !important; }
      .overlay, .rail, .rail-resize, .ctxmenu, .confirm-backdrop { display: none !important; }
    }
  `;

  class DeckStage extends HTMLElement {
    static get observedAttributes() { return ['width', 'height', 'noscale', 'no-rail']; }

    constructor() {
      super();
      this._root = this.attachShadow({ mode: 'open' });
      this._index = 0;
      this._slides = [];
      this._notes = [];
      this._hideTimer = null;
      this._mouseIdleTimer = null;
      this._menuIndex = -1;

      this._onKey = this._onKey.bind(this);
      this._onResize = this._onResize.bind(this);
      this._onSlotChange = this._onSlotChange.bind(this);
      this._onMouseMove = this._onMouseMove.bind(this);
      this._onTap = this._onTap.bind(this);
      this._onMessage = this._onMessage.bind(this);
      // Capture-phase close so a click anywhere dismisses the menu, but
      // ignore clicks that land inside the menu itself — otherwise the
      // capture handler runs before the menu's own (bubble) handler and
      // clears _menuIndex out from under it.
      this._onDocClick = (e) => {
        if (this._menu && e.composedPath && e.composedPath().includes(this._menu)) return;
        this._closeMenu();
      };
    }

    get designWidth() {
      return parseInt(this.getAttribute('width'), 10) || DESIGN_W_DEFAULT;
    }
    get designHeight() {
      return parseInt(this.getAttribute('height'), 10) || DESIGN_H_DEFAULT;
    }

    connectedCallback() {
      // Presenter-view popup loads deckUrl?_snthumb=...#N for its prev/cur/
      // next thumbnails — the rail has no business rendering inside those
      // (wrong scale, and it offsets the stage so the thumb shows a gutter).
      if (/[?&]_snthumb=/.test(location.search)) this.setAttribute('no-rail', '');
      this._render();
      this._loadNotes();
      this._syncPrintPageRule();
      window.addEventListener('keydown', this._onKey);
      window.addEventListener('resize', this._onResize);
      window.addEventListener('mousemove', this._onMouseMove, { passive: true });
      window.addEventListener('message', this._onMessage);
      window.addEventListener('click', this._onDocClick, true);
      this.addEventListener('click', this._onTap);
      // Initial collection + layout happens via slotchange, which fires on mount.
      this._enableRail();
      // Hold the stage hidden until webfonts are ready so the first visible
      // paint has the deck's real typography — the :not(:defined) guard in
      // the page HTML only covers custom-element upgrade, not font load.
      // Capped so a 404'd font URL can't blank the deck indefinitely.
      this.setAttribute('data-fonts-pending', '');
      const reveal = () => this.removeAttribute('data-fonts-pending');
      // rAF first: fonts.ready is a pre-resolved promise until layout has
      // resolved the slotted text's font-family and pushed a FontFace into
      // 'loading'. Reading it here in connectedCallback (parse-time) would
      // settle the race in a microtask before any font fetch starts.
      requestAnimationFrame(() => {
        Promise.race([
          document.fonts ? document.fonts.ready : Promise.resolve(),
          new Promise((r) => setTimeout(r, 2000)),
        ]).then(reveal, reveal);
      });
    }

    _enableRail() {
      // Idempotent — older host builds still post __omelette_rail_enabled.
      // no-rail guard keeps the observers/stylesheet walk off the cheap path
      // for presenter-popup thumbnail iframes (up to 9 per view).
      if (this._railEnabled || this.hasAttribute('no-rail')) return;
      this._railEnabled = true;
      // Per-viewer preference — restored alongside rail width. Default on;
      // only a stored '0' (from the TweaksPanel toggle) hides it.
      this._railVisible = true;
      try {
        if (localStorage.getItem('deck-stage.railVisible') === '0') this._railVisible = false;
      } catch (e) {}
      // Live thumbnail updates: watch the light-DOM slides for content
      // edits and re-clone just the affected thumb(s), debounced. Ignore
      // the data-deck-* / data-screen-label / data-om-validate attributes
      // this component itself writes so nav and skip don't trigger
      // spurious refreshes.
      const OWN_ATTRS = /^data-(deck-|screen-label$|om-validate$)/;
      this._liveDirty = new Set();
      this._liveObserver = new MutationObserver((records) => {
        for (const r of records) {
          if (r.type === 'attributes' && OWN_ATTRS.test(r.attributeName || '')) continue;
          let n = r.target;
          while (n && n.parentElement !== this) n = n.parentElement;
          if (n && this._slideSet && this._slideSet.has(n)) this._liveDirty.add(n);
        }
        if (this._liveDirty.size && !this._liveTimer) {
          this._liveTimer = setTimeout(() => {
            this._liveTimer = null;
            this._liveDirty.forEach((s) => this._refreshThumb(s));
            this._liveDirty.clear();
          }, 200);
        }
      });
      this._liveObserver.observe(this, {
        subtree: true, childList: true, characterData: true, attributes: true,
      });
      // Lazy thumbnail materialization — clone the slide only when its
      // frame scrolls into (or near) the rail viewport. rootMargin gives
      // ~4 thumbs of pre-load so fast scrolling doesn't flash blanks.
      this._railObserver = new IntersectionObserver((entries) => {
        entries.forEach((e) => {
          if (e.isIntersecting && e.target.__deckThumb) {
            this._materialize(e.target.__deckThumb);
          }
        });
      }, { root: this._rail, rootMargin: '400px 0px' });
      // Tweaks typically change CSS vars / attrs OUTSIDE <deck-stage>
      // (on <html>, <body>, a wrapper div, or a <style> tag), which
      // _liveObserver can't see. Re-snapshot author CSS (constructable
      // sheet is shared by reference, so one replaceSync updates every
      // thumb shadow root) and re-sync each thumb host's attrs + custom
      // properties. In-slide DOM mutations are _liveObserver's job.
      // Debounced so slider drags don't thrash.
      this._onTweakChange = () => {
        clearTimeout(this._tweakTimer);
        this._tweakTimer = setTimeout(() => {
          this._snapshotAuthorCss();
          // One getComputedStyle for the whole batch — each
          // getPropertyValue read below reuses the same computed style
          // as long as nothing invalidates layout between thumbs.
          const cs = getComputedStyle(this);
          (this._thumbs || []).forEach((t) => {
            if (t.host) this._syncThumbHostAttrs(t.host, cs);
          });
        }, 120);
      };
      window.addEventListener('tweakchange', this._onTweakChange);
      this._snapshotAuthorCss();
      // Build the rail now that it's enabled — slotchange already fired,
      // so _renderRail's early-return skipped the initial build.
      this._syncRailHidden();
      this._renderRail();
      this._fit();
    }

    /** Snapshot document stylesheets into a constructable sheet that each
     *  thumbnail's nested shadow root adopts — so author CSS styles the
     *  cloned slide content without touching this component's chrome.
     *  Cross-origin sheets throw on .cssRules — skip them. Re-callable:
     *  the existing constructable sheet is reused via replaceSync so every
     *  already-adopted shadow root picks up the fresh CSS without re-adopt. */
    _snapshotAuthorCss() {
      // :root in an adopted sheet inside a shadow root matches nothing
      // (only the document root qualifies), so author rules like
      // `:root[data-voice="modern"] .serif` never reach the clones.
      // Rewrite :root → :host and mirror <html>'s data-*/class/lang onto
      // each thumb host (see _syncThumbHostAttrs) so the same selectors
      // match inside the thumbnail's shadow tree.
      const authorCss = Array.from(document.styleSheets).map((sh) => {
        try {
          return Array.from(sh.cssRules).map((r) => r.cssText).join('\n');
        } catch (e) { return ''; }
      }).join('\n')
        // The shadow host is featureless outside the functional :host(...)
        // form, so any compound on :root — [attr], .class, #id, :pseudo —
        // must become :host(<compound>) not :host<compound>. Same for the
        // html type selector (Tailwind class-strategy dark mode emits
        // html.dark; Pico uses html[data-theme]), which has nothing to
        // match inside the thumb's shadow tree.
        .replace(/:root((?:\[[^\]]*\]|[.#][-\w]+|:[-\w]+(?:\([^)]*\))?)+)/g, ':host($1)')
        .replace(/:root\b/g, ':host')
        .replace(/(^|[\s,>~+(}])html((?:\[[^\]]*\]|[.#][-\w]+|:[-\w]+(?:\([^)]*\))?)+)(?![-\w])/g, '$1:host($2)')
        .replace(/(^|[\s,>~+(}])html(?![-\w])/g, '$1:host');
      // Every custom property the author references. _syncThumbHostAttrs
      // mirrors each one's *computed* value at <deck-stage> onto the
      // thumb host so the live value wins over the :host default above
      // regardless of which ancestor the tweak wrote to (<html>, <body>,
      // a wrapper div, or the deck-stage element itself all inherit
      // down to getComputedStyle(this)).
      this._authorVars = new Set(authorCss.match(/--[\w-]+/g) || []);
      try {
        if (!this._adoptedSheet) this._adoptedSheet = new CSSStyleSheet();
        this._adoptedSheet.replaceSync(authorCss);
      } catch (e) {
        this._adoptedSheet = null;
        this._authorCss = authorCss;
      }
    }

    _syncThumbHostAttrs(host, cs) {
      const de = document.documentElement;
      // setAttribute overwrites but can't delete — an attr removed from
      // <html> (toggleAttribute off, classList emptied) would linger on
      // the host and :host([data-*]) / :host(.foo) rules would keep
      // matching. Remove stale mirrored attrs first; iterate backward
      // because removeAttribute mutates the live NamedNodeMap.
      for (let i = host.attributes.length - 1; i >= 0; i--) {
        const n = host.attributes[i].name;
        if ((n.startsWith('data-') || n === 'class' || n === 'lang')
            && !de.hasAttribute(n)) {
          host.removeAttribute(n);
        }
      }
      for (const a of de.attributes) {
        if (a.name.startsWith('data-') || a.name === 'class' || a.name === 'lang') {
          host.setAttribute(a.name, a.value);
        }
      }
      // The :root→:host rewrite in _snapshotAuthorCss pins each custom
      // property to its stylesheet default on the thumb host, shadowing
      // the live value that would otherwise inherit. Tweaks can write the
      // live value on any ancestor — <html>, <body>, a wrapper div, the
      // deck-stage element — so read it as the *computed* value at
      // <deck-stage> (which sees the whole inheritance chain) rather than
      // trying to guess which element the author wrote to. Inline on the
      // host beats the :host{} rule. remove-stale covers vars dropped
      // from the stylesheet between snapshots.
      const vars = this._authorVars || new Set();
      for (let i = host.style.length - 1; i >= 0; i--) {
        const p = host.style[i];
        if (p.startsWith('--') && !vars.has(p)) host.style.removeProperty(p);
      }
      const live = cs || getComputedStyle(this);
      vars.forEach((p) => {
        const v = live.getPropertyValue(p);
        if (v) host.style.setProperty(p, v.trim());
        else host.style.removeProperty(p);
      });
    }

    disconnectedCallback() {
      window.removeEventListener('keydown', this._onKey);
      window.removeEventListener('resize', this._onResize);
      window.removeEventListener('mousemove', this._onMouseMove);
      window.removeEventListener('message', this._onMessage);
      window.removeEventListener('click', this._onDocClick, true);
      this.removeEventListener('click', this._onTap);
      if (this._hideTimer) clearTimeout(this._hideTimer);
      if (this._mouseIdleTimer) clearTimeout(this._mouseIdleTimer);
      if (this._liveTimer) clearTimeout(this._liveTimer);
      if (this._tweakTimer) clearTimeout(this._tweakTimer);
      if (this._railAnimTimer) clearTimeout(this._railAnimTimer);
      if (this._scaleRaf) cancelAnimationFrame(this._scaleRaf);
      if (this._liveObserver) this._liveObserver.disconnect();
      if (this._railObserver) this._railObserver.disconnect();
      if (this._onTweakChange) window.removeEventListener('tweakchange', this._onTweakChange);
    }

    attributeChangedCallback() {
      if (this._canvas) {
        this._canvas.style.width = this.designWidth + 'px';
        this._canvas.style.height = this.designHeight + 'px';
        this._canvas.style.setProperty('--deck-design-w', this.designWidth + 'px');
        this._canvas.style.setProperty('--deck-design-h', this.designHeight + 'px');
        if (this._rail) {
          this._rail.style.setProperty('--deck-aspect', this.designWidth + '/' + this.designHeight);
        }
        this._fit();
        this._scaleThumbs();
        this._syncPrintPageRule();
      }
    }

    _render() {
      const style = document.createElement('style');
      style.textContent = stylesheet;

      const stage = document.createElement('div');
      stage.className = 'stage';

      const canvas = document.createElement('div');
      canvas.className = 'canvas';
      canvas.style.width = this.designWidth + 'px';
      canvas.style.height = this.designHeight + 'px';
      canvas.style.setProperty('--deck-design-w', this.designWidth + 'px');
      canvas.style.setProperty('--deck-design-h', this.designHeight + 'px');

      const slot = document.createElement('slot');
      slot.addEventListener('slotchange', this._onSlotChange);
      canvas.appendChild(slot);
      stage.appendChild(canvas);

      // Overlay: compact, solid black, with clickable controls.
      const overlay = document.createElement('div');
      overlay.className = 'overlay export-hidden';
      overlay.setAttribute('role', 'toolbar');
      overlay.setAttribute('aria-label', 'Deck controls');
      overlay.setAttribute('data-omelette-chrome', '');
      overlay.innerHTML = `
        <button class="btn prev" type="button" aria-label="Previous slide" title="Previous (←)">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M10 3L5 8l5 5"/></svg>
        </button>
        <span class="count" aria-live="polite"><span class="current">1</span><span class="sep">/</span><span class="total">1</span></span>
        <button class="btn next" type="button" aria-label="Next slide" title="Next (→)">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M6 3l5 5-5 5"/></svg>
        </button>
        <span class="divider"></span>
        <button class="btn reset" type="button" aria-label="Reset to first slide" title="Reset (R)">Reset<span class="kbd">R</span></button>
      `;

      overlay.querySelector('.prev').addEventListener('click', () => this._advance(-1, 'click'));
      overlay.querySelector('.next').addEventListener('click', () => this._advance(1, 'click'));
      overlay.querySelector('.reset').addEventListener('click', () => this._go(0, 'click'));

      // Thumbnail rail + context menu. Thumbnails are populated in
      // _renderRail() after _collectSlides().
      const rail = document.createElement('div');
      rail.className = 'rail export-hidden';
      rail.setAttribute('data-omelette-chrome', '');
      rail.style.setProperty('--deck-aspect', this.designWidth + '/' + this.designHeight);
      // Edge auto-scroll while dragging a thumb near the rail's top/bottom
      // so off-screen drop targets are reachable. Native dragover fires
      // continuously while the pointer is stationary, so a per-event nudge
      // (ramped by edge proximity) is enough — no rAF loop needed.
      rail.addEventListener('dragover', (e) => {
        if (this._dragFrom == null) return;
        const r = rail.getBoundingClientRect();
        const EDGE = 40;
        const dt = e.clientY - r.top;
        const db = r.bottom - e.clientY;
        if (dt < EDGE) rail.scrollTop -= Math.ceil((EDGE - dt) / 3);
        else if (db < EDGE) rail.scrollTop += Math.ceil((EDGE - db) / 3);
      });

      const menu = document.createElement('div');
      menu.className = 'ctxmenu export-hidden';
      menu.setAttribute('data-omelette-chrome', '');
      menu.innerHTML = `
        <button type="button" data-act="skip">Skip slide</button>
        <button type="button" data-act="up">Move up</button>
        <button type="button" data-act="down">Move down</button>
        <hr>
        <button type="button" data-act="delete">Delete slide</button>
      `;
      menu.addEventListener('click', (e) => {
        const act = e.target && e.target.getAttribute && e.target.getAttribute('data-act');
        if (!act) return;
        const i = this._menuIndex;
        this._closeMenu();
        if (act === 'skip') this._toggleSkip(i);
        else if (act === 'up') this._moveSlide(i, i - 1);
        else if (act === 'down') this._moveSlide(i, i + 1);
        else if (act === 'delete') this._openConfirm(i);
      });
      menu.addEventListener('contextmenu', (e) => e.preventDefault());

      // Rail resize handle — drag to set --deck-rail-w, persisted to
      // localStorage so the width survives reloads.
      const resize = document.createElement('div');
      resize.className = 'rail-resize export-hidden';
      resize.setAttribute('data-omelette-chrome', '');
      resize.addEventListener('pointerdown', (e) => {
        e.preventDefault();
        resize.setPointerCapture(e.pointerId);
        resize.setAttribute('data-dragging', '');
        const move = (ev) => this._setRailWidth(ev.clientX);
        const up = () => {
          resize.removeEventListener('pointermove', move);
          resize.removeEventListener('pointerup', up);
          resize.removeEventListener('pointercancel', up);
          resize.removeAttribute('data-dragging');
          try { localStorage.setItem('deck-stage.railWidth', String(this._railPx)); } catch (err) {}
        };
        resize.addEventListener('pointermove', move);
        resize.addEventListener('pointerup', up);
        resize.addEventListener('pointercancel', up);
      });

      // Delete-confirm dialog — mirrors the SPA's ConfirmDialog layout.
      const confirm = document.createElement('div');
      confirm.className = 'confirm-backdrop export-hidden';
      confirm.setAttribute('data-omelette-chrome', '');
      confirm.innerHTML = `
        <div class="confirm" role="dialog" aria-modal="true">
          <div class="body">
            <div class="title">Delete slide?</div>
            <div class="msg">This slide will be removed from the deck.</div>
          </div>
          <div class="footer">
            <button type="button" class="cancel">Cancel</button>
            <button type="button" class="danger">Delete</button>
          </div>
        </div>
      `;
      confirm.addEventListener('click', (e) => {
        if (e.target === confirm) this._closeConfirm();
      });
      confirm.querySelector('.cancel').addEventListener('click', () => this._closeConfirm());
      confirm.querySelector('.danger').addEventListener('click', () => {
        const i = this._confirmIndex;
        this._closeConfirm();
        this._deleteSlide(i);
      });

      this._root.append(style, rail, resize, stage, overlay, menu, confirm);
      this._canvas = canvas;
      this._stage = stage;
      this._slot = slot;
      this._overlay = overlay;
      this._rail = rail;
      this._resize = resize;
      this._menu = menu;
      this._confirm = confirm;
      this._countEl = overlay.querySelector('.current');
      this._totalEl = overlay.querySelector('.total');

      // Restore persisted rail width.
      let rw = 188;
      try {
        const s = localStorage.getItem('deck-stage.railWidth');
        if (s) rw = parseInt(s, 10) || rw;
      } catch (err) {}
      this._setRailWidth(rw);
      this._syncRailHidden();
    }

    _setRailWidth(px) {
      const w = Math.max(120, Math.min(360, Math.round(px)));
      this._railPx = w;
      this.style.setProperty('--deck-rail-w', w + 'px');
      this._fit();
      // _scaleThumbs forces a sync layout (frame.offsetWidth) then writes
      // N transforms. During a resize drag this runs per-pointermove;
      // coalesce to one per frame.
      if (!this._scaleRaf) {
        this._scaleRaf = requestAnimationFrame(() => {
          this._scaleRaf = null;
          this._scaleThumbs();
        });
      }
    }

    /** @page must live in the document stylesheet — it's a no-op inside
     *  shadow DOM. Inject/update a single <head> style tag so the print
     *  sheet matches the design size and Save-as-PDF yields one slide per
     *  page with no margins. */
    _syncPrintPageRule() {
      const id = 'deck-stage-print-page';
      let tag = document.getElementById(id);
      if (!tag) {
        tag = document.createElement('style');
        tag.id = id;
        document.head.appendChild(tag);
      }
      tag.textContent =
        '@page { size: ' + this.designWidth + 'px ' + this.designHeight + 'px; margin: 0; } ' +
        '@media print { html, body { margin: 0 !important; padding: 0 !important; background: none !important; overflow: visible !important; height: auto !important; } ' +
        '* { -webkit-print-color-adjust: exact; print-color-adjust: exact; } }';
    }

    _onSlotChange() {
      // Rail mutations (delete/move) already reconcile synchronously and
      // emit slidechange with reason 'api'; skip the async slotchange that
      // would otherwise re-broadcast with reason 'init'.
      if (this._squelchSlotChange) { this._squelchSlotChange = false; return; }
      this._collectSlides();
      this._restoreIndex();
      this._applyIndex({ showOverlay: false, broadcast: true, reason: 'init' });
      this._fit();
    }

    _collectSlides() {
      const assigned = this._slot.assignedElements({ flatten: true });
      this._slides = assigned.filter((el) => {
        // Skip template/style/script nodes even if someone slots them.
        const tag = el.tagName;
        return tag !== 'TEMPLATE' && tag !== 'SCRIPT' && tag !== 'STYLE';
      });
      this._slideSet = new Set(this._slides);

      this._slides.forEach((slide, i) => {
        const n = i + 1;
        slide.setAttribute('data-screen-label', `${pad2(n)} ${getSlideLabel(slide)}`);

        // Validation attribute for comment flow / auto-checks.
        if (!slide.hasAttribute('data-om-validate')) {
          slide.setAttribute('data-om-validate', VALIDATE_ATTR);
        }

        slide.setAttribute('data-deck-slide', String(i));
      });

      if (this._totalEl) this._totalEl.textContent = String(this._slides.length || 1);
      if (this._index >= this._slides.length) this._index = Math.max(0, this._slides.length - 1);
      this._markLastVisible();
      this._renderRail();
    }

    /** Tag the last non-skipped slide so print CSS can drop its
     *  break-after (see the @media print comment above — :last-child
     *  alone matches a hidden skipped slide). */
    _markLastVisible() {
      let last = null;
      this._slides.forEach((s) => {
        s.removeAttribute('data-deck-last-visible');
        if (!s.hasAttribute('data-deck-skip')) last = s;
      });
      if (last) last.setAttribute('data-deck-last-visible', '');
    }

    _loadNotes() {
      const tag = document.getElementById('speaker-notes');
      if (!tag) { this._notes = []; return; }
      try {
        const parsed = JSON.parse(tag.textContent || '[]');
        if (Array.isArray(parsed)) this._notes = parsed;
      } catch (e) {
        console.warn('[deck-stage] Failed to parse #speaker-notes JSON:', e);
        this._notes = [];
      }
    }

    _restoreIndex() {
      // The host's ?slide= param is delivered as a #<int> hash (1-indexed) on
      // the iframe src. No hash → slide 1; the deck itself keeps no position
      // state across loads.
      const h = (location.hash || '').match(/^#(\d+)$/);
      if (h) {
        const n = parseInt(h[1], 10) - 1;
        if (n >= 0 && n < this._slides.length) this._index = n;
      }
    }

    _applyIndex({ showOverlay = true, broadcast = true, reason = 'init' } = {}) {
      if (!this._slides.length) return;
      const prev = this._prevIndex == null ? -1 : this._prevIndex;
      const curr = this._index;
      // Keep the iframe's own hash in sync so an in-iframe location.reload()
      // (reload banner path in viewer-handle.ts) lands on the current slide,
      // not the stale deep-link hash from initial load.
      try { history.replaceState(null, '', '#' + (curr + 1)); } catch (e) {}
      this._slides.forEach((s, i) => {
        if (i === curr) s.setAttribute('data-deck-active', '');
        else s.removeAttribute('data-deck-active');
      });
      if (this._countEl) this._countEl.textContent = String(curr + 1);
      // Follow-scroll on every navigation (init deep-link, keyboard, click,
      // tap, external goTo) — the only time we *don't* want the rail to
      // track current is after a rail-internal mutation, where _renderRail
      // has already restored the user's scroll position and yanking back to
      // current would undo it.
      this._syncRail(reason !== 'mutation');

      if (broadcast) {
        // (1) Legacy: host-window postMessage for speaker-notes renderers.
        try { window.postMessage({ slideIndexChanged: curr, deckTotal: this._slides.length, deckSkipped: this._skippedIndices() }, '*'); } catch (e) {}

        // (2) In-page CustomEvent on the <deck-stage> element itself.
        //     Bubbles and composes out of shadow DOM so slide code can listen:
        //       document.querySelector('deck-stage').addEventListener('slidechange', e => {
        //         e.detail.index, e.detail.previousIndex, e.detail.total, e.detail.slide, e.detail.reason
        //       });
        const detail = {
          index: curr,
          previousIndex: prev,
          total: this._slides.length,
          slide: this._slides[curr] || null,
          previousSlide: prev >= 0 ? (this._slides[prev] || null) : null,
          reason: reason, // 'init' | 'keyboard' | 'click' | 'tap' | 'api'
        };
        this.dispatchEvent(new CustomEvent('slidechange', {
          detail,
          bubbles: true,
          composed: true,
        }));
      }

      this._prevIndex = curr;
      if (showOverlay) this._flashOverlay();
    }

    _flashOverlay() {
      // Host posts __omelette_presenting while in fullscreen/tab presentation
      // mode — suppress the nav footer entirely (both hover and slide-change
      // flash) so the audience sees clean slides.
      if (!this._overlay || this._presenting) return;
      this._overlay.setAttribute('data-visible', '');
      if (this._hideTimer) clearTimeout(this._hideTimer);
      this._hideTimer = setTimeout(() => {
        this._overlay.removeAttribute('data-visible');
      }, OVERLAY_HIDE_MS);
    }

    _railWidth() {
      // State-based, no offsetWidth: the first _fit() can run before the
      // rail has had layout on some load paths, and a 0 there paints the
      // slide full-width for one frame before the post-slotchange _fit()
      // corrects it.
      if (!this._railEnabled || !this._railVisible || this.hasAttribute('no-rail')
          || this.hasAttribute('noscale') || this._presenting || this._previewMode
          || NARROW_MQ.matches) return 0;
      return this._railPx || 0;
    }

    _fit() {
      if (!this._canvas) return;
      const stage = this._canvas.parentElement;
      // PPTX export sets noscale so the DOM capture sees authored-size
      // geometry — the scaled canvas is in shadow DOM, so the exporter's
      // resetTransformSelector can't reach .canvas.style.transform directly.
      if (this.hasAttribute('noscale')) {
        this._canvas.style.transform = 'none';
        if (stage) stage.style.left = '0';
        if (this._overlay) this._overlay.style.marginLeft = '0';
        return;
      }
      const rw = this._railWidth();
      if (stage) stage.style.left = rw + 'px';
      // Overlay is centred on the viewport via left:50% + translate(-50%);
      // marginLeft shifts the centre by rw/2 so it lands in the middle of
      // the [rw, innerWidth] stage region.
      if (this._overlay) this._overlay.style.marginLeft = (rw / 2) + 'px';
      const vw = window.innerWidth - rw;
      const vh = window.innerHeight;
      const s = Math.min(vw / this.designWidth, vh / this.designHeight);
      this._canvas.style.transform = `scale(${s})`;
    }

    _onResize() {
      this._fit();
      // Crossing the narrow-viewport breakpoint reveals the rail — rerun the
      // thumbnail scale the same way _setRailWidth does.
      if (!this._scaleRaf) {
        this._scaleRaf = requestAnimationFrame(() => {
          this._scaleRaf = null;
          this._scaleThumbs();
        });
      }
    }

    _onMouseMove() {
      // Keep overlay visible while mouse moves; hide after idle.
      this._flashOverlay();
    }

    _onMessage(e) {
      const d = e.data;
      if (d && typeof d.__omelette_presenting === 'boolean') {
        this._presenting = d.__omelette_presenting;
        if (this._presenting && this._overlay) {
          this._overlay.removeAttribute('data-visible');
          if (this._hideTimer) clearTimeout(this._hideTimer);
        }
        this._syncRailHidden();
        this._closeMenu();
        this._closeConfirm();
        this._fit();
        this._scaleThumbs();
      }
      // Host's Preview segment (ViewerMode='none'): the rail's drag-reorder /
      // right-click skip-delete affordances are editing chrome, so hide it
      // while the user is just looking at the deck. Same hard-hide path as
      // presenting; independent of the user's _railVisible preference so
      // returning to Edit restores whatever they had.
      if (d && typeof d.__omelette_preview_mode === 'boolean') {
        if (d.__omelette_preview_mode === this._previewMode) return;
        this._previewMode = d.__omelette_preview_mode;
        this._syncRailHidden();
        this._closeMenu();
        this._closeConfirm();
        this._fit();
        this._scaleThumbs();
      }
      // Per-viewer show/hide, driven by the TweaksPanel's auto-injected
      // "Thumbnail rail" toggle (or any author script). Independent of
      // whether the Tweaks panel itself is open — closing the panel
      // doesn't change rail visibility. Persists alongside rail width.
      if (d && d.type === '__deck_rail_visible' && typeof d.on === 'boolean') {
        if (d.on === this._railVisible) return;
        this._railVisible = d.on;
        try { localStorage.setItem('deck-stage.railVisible', d.on ? '1' : '0'); } catch (e) {}
        // Arm the transition, commit it, then flip state — otherwise the
        // browser coalesces both writes and nothing animates on show.
        this.setAttribute('data-rail-anim', '');
        void (this._rail && this._rail.offsetHeight);
        this._syncRailHidden();
        this._fit();
        this._scaleThumbs();
        clearTimeout(this._railAnimTimer);
        this._railAnimTimer = setTimeout(() => this.removeAttribute('data-rail-anim'), 220);
      }
      if (d && d.type === '__omelette_rail_enabled') this._enableRail();
    }

    _syncRailHidden() {
      if (!this._rail) return;
      // data-presenting is the hard hide (display:none) for flag-off,
      // presentation mode, and the host's Preview segment — instant, no
      // transition. data-user-hidden is the soft hide (translateX(-100%))
      // for the viewer's rail toggle, so show/hide slides under
      // :host([data-rail-anim]).
      const hard = !this._railEnabled || this._presenting || this._previewMode;
      if (hard) this._rail.setAttribute('data-presenting', '');
      else this._rail.removeAttribute('data-presenting');
      if (!this._railVisible) this._rail.setAttribute('data-user-hidden', '');
      else this._rail.removeAttribute('data-user-hidden');
      // translateX hide leaves thumbs (tabIndex=0) in the tab order —
      // inert keeps them unfocusable while the rail is off-screen.
      this._rail.inert = hard || !this._railVisible;
    }

    _onTap(e) {
      // Touch-only — keyboard + the overlay toolbar cover nav on desktop.
      if (FINE_POINTER_MQ.matches) return;
      // Only taps that land on the stage (slide content or letterbox); the
      // overlay / rail / menus are siblings with their own click handlers.
      const path = e.composedPath();
      if (!this._stage || !path.includes(this._stage)) return;
      // Let interactive slide content keep the tap. composedPath (not
      // e.target.closest) so we see through open shadow roots — a <button>
      // inside a slide-authored custom element retargets e.target to the
      // host but still appears in the composed path.
      if (e.defaultPrevented) return;
      for (const n of path) {
        if (n === this._stage) break;
        if (n.matches && n.matches(INTERACTIVE_SEL)) return;
      }
      e.preventDefault();
      const rw = this._railWidth();
      const mid = rw + (window.innerWidth - rw) / 2;
      this._advance(e.clientX < mid ? -1 : 1, 'tap');
    }

    _onKey(e) {
      // Ignore when the user is typing.
      const t = e.target;
      if (t && (t.isContentEditable || /^(INPUT|TEXTAREA|SELECT)$/.test(t.tagName))) return;
      // Confirm dialog swallows nav keys while open; Escape cancels. Enter
      // is left to the focused button's native activation so Tab→Cancel
      // →Enter activates Cancel, not the window-level confirm path.
      if (this._confirm && this._confirm.hasAttribute('data-open')) {
        if (e.key === 'Escape') { this._closeConfirm(); e.preventDefault(); }
        return;
      }
      if (e.key === 'Escape' && this._menu && this._menu.hasAttribute('data-open')) {
        this._closeMenu();
        e.preventDefault();
        return;
      }
      if (e.metaKey || e.ctrlKey || e.altKey) return;

      const key = e.key;
      let handled = true;

      if (key === 'ArrowRight' || key === 'PageDown' || key === ' ' || key === 'Spacebar') {
        this._advance(1, 'keyboard');
      } else if (key === 'ArrowLeft' || key === 'PageUp') {
        this._advance(-1, 'keyboard');
      } else if (key === 'Home') {
        this._go(0, 'keyboard');
      } else if (key === 'End') {
        this._go(this._slides.length - 1, 'keyboard');
      } else if (key === 'r' || key === 'R') {
        this._go(0, 'keyboard');
      } else if (/^[0-9]$/.test(key)) {
        // 1..9 jump to that slide; 0 jumps to 10.
        const n = key === '0' ? 9 : parseInt(key, 10) - 1;
        if (n < this._slides.length) this._go(n, 'keyboard');
      } else {
        handled = false;
      }

      if (handled) {
        e.preventDefault();
        this._flashOverlay();
      }
    }

    _go(i, reason = 'api') {
      if (!this._slides.length) return;
      const clamped = Math.max(0, Math.min(this._slides.length - 1, i));
      if (clamped === this._index) {
        this._flashOverlay();
        return;
      }
      this._index = clamped;
      this._applyIndex({ showOverlay: true, broadcast: true, reason });
    }

    /** Step forward/back skipping any slide marked data-deck-skip. Falls
     *  back to _go's clamp-at-ends behaviour (flash overlay) when there's
     *  nothing further in that direction. */
    _advance(dir, reason) {
      if (!this._slides.length) return;
      let i = this._index + dir;
      while (i >= 0 && i < this._slides.length && this._slides[i].hasAttribute('data-deck-skip')) {
        i += dir;
      }
      if (i < 0 || i >= this._slides.length) { this._flashOverlay(); return; }
      this._go(i, reason);
    }

    // ── Thumbnail rail ────────────────────────────────────────────────────
    //
    // Thumbs are keyed by slide element and reused across _renderRail()
    // calls, so a reorder/delete is an O(changed) DOM shuffle instead of an
    // O(N) teardown-and-re-clone. Each thumb starts as a lightweight shell
    // (num + empty frame); the clone is materialized lazily by an
    // IntersectionObserver when the frame scrolls into (or near) view, so
    // only visible-ish slides pay the clone + image-decode cost.

    _renderRail() {
      if (!this._rail || !this._railEnabled) { this._thumbs = []; return; }
      // FLIP: record each *materialized* thumb's top before the reconcile.
      // Off-screen (non-materialized) thumbs don't need the animation and
      // skipping their getBoundingClientRect saves a forced layout per
      // off-screen thumb on large decks.
      const prevTops = new Map();
      (this._thumbs || []).forEach(({ thumb, slide, host }) => {
        if (host) prevTops.set(slide, thumb.getBoundingClientRect().top);
      });
      const st = this._rail.scrollTop;

      // Reconcile: reuse thumbs that already exist for a slide, create
      // shells for new slides, drop thumbs for removed slides.
      const bySlide = new Map();
      (this._thumbs || []).forEach((t) => bySlide.set(t.slide, t));
      const next = [];
      this._slides.forEach((slide) => {
        let t = bySlide.get(slide);
        if (t) bySlide.delete(slide);
        else t = this._makeThumb(slide);
        next.push(t);
      });
      // Orphans — slides removed since last render.
      bySlide.forEach((t) => {
        if (this._railObserver) this._railObserver.unobserve(t.frame);
        t.thumb.remove();
      });
      // Put thumbs into document order to match _slides. insertBefore on
      // an already-correctly-placed node is a no-op, so this is cheap
      // when nothing moved.
      next.forEach((t, i) => {
        const want = t.thumb;
        const at = this._rail.children[i];
        if (at !== want) this._rail.insertBefore(want, at || null);
        t.i = i;
        t.num.textContent = String(i + 1);
        if (t.slide.hasAttribute('data-deck-skip')) t.thumb.setAttribute('data-skip', '');
        else t.thumb.removeAttribute('data-skip');
      });
      this._thumbs = next;

      this._rail.scrollTop = st;
      if (prevTops.size) {
        const moved = [];
        this._thumbs.forEach(({ thumb, slide }) => {
          const old = prevTops.get(slide);
          if (old == null) return;
          const dy = old - thumb.getBoundingClientRect().top;
          if (Math.abs(dy) < 1) return;
          thumb.style.transition = 'none';
          thumb.style.transform = `translateY(${dy}px)`;
          moved.push(thumb);
        });
        if (moved.length) {
          // Commit the inverted positions before flipping the transition
          // on — otherwise the browser coalesces both style writes and
          // nothing animates.
          void this._rail.offsetHeight;
          moved.forEach((t) => {
            t.style.transition = 'transform 180ms cubic-bezier(.2,.7,.3,1)';
            t.style.transform = '';
          });
          setTimeout(() => moved.forEach((t) => { t.style.transition = ''; }), 220);
        }
      }
      requestAnimationFrame(() => this._scaleThumbs());
      this._syncRail(false);
    }

    /** Create a lightweight thumb shell for one slide. The clone is
     *  materialized later by the IntersectionObserver. Event handlers
     *  look up the thumb's *current* index (via _thumbs.indexOf) so the
     *  same element can be reused across reorders. */
    _makeThumb(slide) {
      const thumb = document.createElement('div');
      thumb.className = 'thumb';
      thumb.tabIndex = 0;
      const num = document.createElement('div');
      num.className = 'num';
      const frame = document.createElement('div');
      frame.className = 'frame';
      thumb.append(num, frame);

      const entry = { thumb, num, frame, slide, clone: null, host: null, i: -1 };
      // entry.i is refreshed on every _renderRail reconcile pass, so
      // handlers read the thumb's current position without an O(N) scan.
      const idx = () => entry.i;

      thumb.addEventListener('click', () => this._go(idx(), 'click'));
      // ↑/↓ step through the rail when a thumb has focus. _go clamps at the
      // ends and _applyIndex→_syncRail scrolls the new current thumb into
      // view; we move focus to it (preventScroll — _syncRail already
      // scrolled) so a held key walks the whole list. stopPropagation keeps
      // this out of the window-level _onKey nav handler.
      thumb.addEventListener('keydown', (e) => {
        if (e.key !== 'ArrowUp' && e.key !== 'ArrowDown') return;
        if (e.metaKey || e.ctrlKey || e.altKey) return;
        e.preventDefault();
        e.stopPropagation();
        this._go(idx() + (e.key === 'ArrowDown' ? 1 : -1), 'keyboard');
        const cur = this._thumbs && this._thumbs[this._index];
        if (cur) cur.thumb.focus({ preventScroll: true });
      });
      thumb.addEventListener('contextmenu', (e) => {
        e.preventDefault();
        this._openMenu(idx(), e.clientX, e.clientY);
      });
      thumb.draggable = true;
      thumb.addEventListener('dragstart', (e) => {
        this._dragFrom = idx();
        thumb.setAttribute('data-dragging', '');
        e.dataTransfer.effectAllowed = 'move';
        try { e.dataTransfer.setData('text/plain', String(this._dragFrom)); } catch (err) {}
      });
      thumb.addEventListener('dragend', () => {
        thumb.removeAttribute('data-dragging');
        this._clearDrop();
        this._dragFrom = null;
      });
      thumb.addEventListener('dragover', (e) => {
        if (this._dragFrom == null) return;
        e.preventDefault();
        e.dataTransfer.dropEffect = 'move';
        const r = thumb.getBoundingClientRect();
        this._setDrop(idx(), e.clientY < r.top + r.height / 2 ? 'before' : 'after');
      });
      thumb.addEventListener('drop', (e) => {
        if (this._dragFrom == null) return;
        e.preventDefault();
        const i = idx();
        const r = thumb.getBoundingClientRect();
        let to = e.clientY >= r.top + r.height / 2 ? i + 1 : i;
        if (this._dragFrom < to) to--;
        const from = this._dragFrom;
        this._clearDrop();
        this._dragFrom = null;
        if (to !== from) this._moveSlide(from, to);
      });

      if (this._railObserver) this._railObserver.observe(frame);
      frame.__deckThumb = entry;
      return entry;
    }

    /** Lazily build the clone for a thumb that has scrolled into view. */
    _materialize(entry) {
      if (entry.host) return;
      const dw = this.designWidth, dh = this.designHeight;
      let clone = entry.slide.cloneNode(true);
      clone.removeAttribute('id');
      clone.removeAttribute('data-deck-active');
      clone.querySelectorAll('[id]').forEach((el) => el.removeAttribute('id'));
      // Neuter heavy media; replace <video> with its poster so the box
      // keeps a visual. <iframe>/<audio> become empty placeholders.
      clone.querySelectorAll('iframe, audio, object, embed').forEach((el) => {
        el.removeAttribute('src');
        el.removeAttribute('srcdoc');
        el.removeAttribute('data');
        el.innerHTML = '';
      });
      clone.querySelectorAll('video').forEach((el) => {
        if (!el.poster) { el.removeAttribute('src'); el.innerHTML = ''; return; }
        const img = document.createElement('img');
        img.src = el.poster;
        img.alt = '';
        img.style.cssText = el.style.cssText + ';object-fit:cover;width:100%;height:100%;';
        img.className = el.className;
        el.replaceWith(img);
      });
      // Images: defer decode and let the browser pick the smallest
      // srcset candidate for the ~140px thumb. Same-URL clones reuse the
      // slide's decoded bitmap (URL-keyed cache), so the remaining cost
      // is paint/composite — lazy+async keeps that off the main thread.
      clone.querySelectorAll('img').forEach((el) => {
        el.loading = 'lazy';
        el.decoding = 'async';
        if (el.srcset) el.sizes = (this._railPx || 188) + 'px';
      });
      // Custom elements inside the slide would have their
      // connectedCallback fire when the clone is appended. Replace them
      // with inert boxes so a component-heavy deck doesn't run N copies
      // of each component's mount logic in the rail. Children are
      // preserved so layout-wrapper elements (<my-column><h2>…</h2>)
      // still show their authored content; the querySelectorAll NodeList
      // is static, so nested custom elements in the moved subtree are
      // still visited on later iterations.
      const neuter = (el) => {
        const box = document.createElement('div');
        box.style.cssText = (el.getAttribute('style') || '') +
          ';background:rgba(0,0,0,0.06);border:1px dashed rgba(0,0,0,0.15);';
        box.className = el.className;
        // Preserve theming/i18n hooks so [data-*] / :lang() / [dir]
        // descendant selectors still match the neutered root.
        for (const a of el.attributes) {
          const n = a.name;
          if (n.startsWith('data-') || n.startsWith('aria-') ||
              n === 'lang' || n === 'dir' || n === 'role' || n === 'title') {
            box.setAttribute(n, a.value);
          }
        }
        while (el.firstChild) box.appendChild(el.firstChild);
        return box;
      };
      // querySelectorAll('*') returns descendants only — a custom-element
      // slide root (<my-slide>…</my-slide>) would slip through and upgrade
      // on append. Swap the root first.
      if (clone.tagName.includes('-')) clone = neuter(clone);
      clone.querySelectorAll('*').forEach((el) => {
        if (el.tagName.includes('-')) el.replaceWith(neuter(el));
      });
      clone.style.cssText += ';position:absolute;top:0;left:0;transform-origin:0 0;' +
        'pointer-events:none;width:' + dw + 'px;height:' + dh + 'px;' +
        'box-sizing:border-box;overflow:hidden;visibility:visible;opacity:1;';
      const host = document.createElement('div');
      host.style.cssText = 'position:absolute;inset:0;';
      this._syncThumbHostAttrs(host);
      const sr = host.attachShadow({ mode: 'open' });
      if (this._adoptedSheet) sr.adoptedStyleSheets = [this._adoptedSheet];
      else {
        const st = document.createElement('style');
        st.textContent = this._authorCss || '';
        sr.appendChild(st);
      }
      sr.appendChild(clone);
      entry.frame.appendChild(host);
      entry.host = host;
      entry.clone = clone;
      if (this._thumbScale) clone.style.transform = 'scale(' + this._thumbScale + ')';
      // Once materialized the IO callback is a no-op early-return —
      // unobserve so scroll doesn't keep firing it.
      if (this._railObserver) this._railObserver.unobserve(entry.frame);
    }

    /** Re-clone a single thumb (live-update path). No-op if the thumb
     *  hasn't been materialized yet — it'll pick up current content when
     *  it scrolls into view. */
    _refreshThumb(slide) {
      const entry = (this._thumbs || []).find((t) => t.slide === slide);
      if (!entry || !entry.host) return;
      entry.host.remove();
      entry.host = entry.clone = null;
      this._materialize(entry);
    }

    _scaleThumbs() {
      if (!this._thumbs || !this._thumbs.length) return;
      // Every frame is the same width; if it reads 0 the rail is
      // display:none (noscale / no-rail / presenting / print) — leave the
      // clones as-is and re-run when the rail is revealed.
      const fw = this._thumbs[0].frame.offsetWidth;
      if (!fw) return;
      this._thumbScale = fw / this.designWidth;
      this._thumbs.forEach(({ clone }) => {
        if (clone) clone.style.transform = 'scale(' + this._thumbScale + ')';
      });
    }

    _setDrop(i, where) {
      // dragover fires at pointer-event rate; touch only the previous
      // and new target rather than sweeping all N thumbs.
      const t = this._thumbs && this._thumbs[i];
      if (this._dropOn && this._dropOn !== t) {
        this._dropOn.thumb.removeAttribute('data-drop');
      }
      if (t) t.thumb.setAttribute('data-drop', where);
      this._dropOn = t || null;
    }

    _clearDrop() {
      if (this._dropOn) this._dropOn.thumb.removeAttribute('data-drop');
      this._dropOn = null;
    }

    _syncRail(follow) {
      if (!this._thumbs) return;
      this._thumbs.forEach(({ thumb }, i) => {
        if (i === this._index) {
          thumb.setAttribute('data-current', '');
          if (follow && typeof thumb.scrollIntoView === 'function') {
            thumb.scrollIntoView({ block: 'nearest' });
          }
        } else {
          thumb.removeAttribute('data-current');
        }
      });
    }

    _openMenu(i, x, y) {
      if (!this._menu) return;
      this._menuIndex = i;
      const slide = this._slides[i];
      const skip = slide && slide.hasAttribute('data-deck-skip');
      this._menu.querySelector('[data-act="skip"]').textContent = skip ? 'Unskip slide' : 'Skip slide';
      this._menu.querySelector('[data-act="up"]').disabled = i <= 0;
      this._menu.querySelector('[data-act="down"]').disabled = i >= this._slides.length - 1;
      this._menu.querySelector('[data-act="delete"]').disabled = this._slides.length <= 1;
      // Place, then clamp to viewport after it's measurable.
      this._menu.style.left = x + 'px';
      this._menu.style.top = y + 'px';
      this._menu.setAttribute('data-open', '');
      const r = this._menu.getBoundingClientRect();
      const nx = Math.min(x, window.innerWidth - r.width - 4);
      const ny = Math.min(y, window.innerHeight - r.height - 4);
      this._menu.style.left = Math.max(4, nx) + 'px';
      this._menu.style.top = Math.max(4, ny) + 'px';
    }

    _closeMenu() {
      if (this._menu) this._menu.removeAttribute('data-open');
      this._menuIndex = -1;
    }

    _openConfirm(i) {
      if (!this._confirm) return;
      this._confirmIndex = i;
      this._confirm.querySelector('.title').textContent = 'Delete slide ' + (i + 1) + '?';
      this._confirm.setAttribute('data-open', '');
      const btn = this._confirm.querySelector('.danger');
      if (btn && btn.focus) btn.focus();
    }

    _closeConfirm() {
      if (this._confirm) this._confirm.removeAttribute('data-open');
      this._confirmIndex = -1;
    }

    _emitDeckChange(detail) {
      this.dispatchEvent(new CustomEvent('deckchange', {
        detail, bubbles: true, composed: true,
      }));
    }

    _deleteSlide(i) {
      const slide = this._slides[i];
      if (!slide || this._slides.length <= 1) return;
      const wasCurrent = i === this._index;
      if (i < this._index || (wasCurrent && i === this._slides.length - 1)) this._index--;
      this._squelchSlotChange = true;
      slide.remove();
      this._emitDeckChange({ action: 'delete', from: i, slide });
      this._collectSlides();
      this._applyIndex({ showOverlay: true, broadcast: true, reason: 'mutation' });
    }

    _toggleSkip(i) {
      const slide = this._slides[i];
      if (!slide) return;
      const on = !slide.hasAttribute('data-deck-skip');
      if (on) slide.setAttribute('data-deck-skip', '');
      else slide.removeAttribute('data-deck-skip');
      if (this._thumbs && this._thumbs[i]) {
        if (on) this._thumbs[i].thumb.setAttribute('data-skip', '');
        else this._thumbs[i].thumb.removeAttribute('data-skip');
      }
      this._markLastVisible();
      this._emitDeckChange({ action: on ? 'skip' : 'unskip', from: i, slide });
      // Re-broadcast so the presenter popup's prev/next thumbnails re-pick
      // the nearest non-skipped slide without waiting for a nav event.
      try { window.postMessage({ slideIndexChanged: this._index, deckTotal: this._slides.length, deckSkipped: this._skippedIndices() }, '*'); } catch (e) {}
    }

    _skippedIndices() {
      const out = [];
      for (let i = 0; i < this._slides.length; i++) {
        if (this._slides[i].hasAttribute('data-deck-skip')) out.push(i);
      }
      return out;
    }

    _moveSlide(i, j) {
      if (j < 0 || j >= this._slides.length || j === i) return;
      const slide = this._slides[i];
      const ref = j < i ? this._slides[j] : this._slides[j].nextSibling;
      // Track the active slide across the reorder so the same content
      // stays on screen.
      const cur = this._index;
      if (cur === i) this._index = j;
      else if (i < cur && j >= cur) this._index = cur - 1;
      else if (i > cur && j <= cur) this._index = cur + 1;
      this._squelchSlotChange = true;
      this.insertBefore(slide, ref);
      this._emitDeckChange({ action: 'move', from: i, to: j, slide });
      this._collectSlides();
      this._applyIndex({ showOverlay: false, broadcast: true, reason: 'mutation' });
    }

    // Public API ------------------------------------------------------------

    /** Current slide index (0-based). */
    get index() { return this._index; }
    /** Total slide count. */
    get length() { return this._slides.length; }
    /** Programmatically navigate. */
    goTo(i) { this._go(i, 'api'); }
    next() { this._advance(1, 'api'); }
    prev() { this._advance(-1, 'api'); }
    reset() { this._go(0, 'api'); }
  }

  if (!customElements.get('deck-stage')) {
    customElements.define('deck-stage', DeckStage);
  }
})();

</script>
<script>
  // Live ticking counter inside the Agent Orchestrator (slide 7)
  (function tickActions(){
    const el = document.getElementById('convActions');
    if (!el) return;
    let v = 2481;
    setInterval(() => {
      // small random walk, biased upward, never below 2000
      const delta = Math.floor(Math.random() * 80) - 30;
      v = Math.max(2000, Math.min(3200, v + delta));
      el.textContent = v.toLocaleString();
    }, 700);
  })();

  // Cycle per-agent throughput numbers
  (function tickAgentRates(){
    const els = document.querySelectorAll('.s-conv__agent .rate em');
    if (!els.length) return;
    const bases = [3.2, 1.8, 0.9];
    setInterval(() => {
      els.forEach((el, i) => {
        if (i >= bases.length) return;
        const wobble = (Math.random() * 0.6 - 0.3);
        const v = Math.max(0.2, bases[i] + wobble);
        el.textContent = v.toFixed(1) + 'k';
      });
    }, 900);
  })();
</script>
<script>
  // Populate the HQI heatmap
  (function buildHeat(){
    const heat = document.getElementById('heat');
    if (!heat) return;
    const COLS = 16, ROWS = 8;
    const palette = [
      'var(--wisy-indigo-100)',  // very light
      'var(--wisy-indigo-200)',
      '#A8AFFF',
      'var(--wisy-indigo)',
      'var(--wisy-indigo-800)'
    ];
    // Seeded pseudo-random distribution so it looks intentional
    let seed = 7;
    const rng = () => (seed = (seed * 1103515245 + 12345) & 0x7fffffff) / 0x7fffffff;
    for (let i = 0; i < COLS * ROWS; i++) {
      const r = rng();
      let idx;
      if (r < 0.40) idx = 0;
      else if (r < 0.65) idx = 1;
      else if (r < 0.85) idx = 2;
      else if (r < 0.96) idx = 3;
      else idx = 4;
      // sprinkle a few lime "danger" cells
      const lime = (rng() < 0.04);
      const span = document.createElement('span');
      span.style.background = lime ? 'var(--wisy-lime)' : palette[idx];
      heat.appendChild(span);
    }
  })();
</script>

</body>
</html>
