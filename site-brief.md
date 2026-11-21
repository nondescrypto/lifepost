# Personal Website — Conceptual Brief

## What this is
Not a portfolio *about* me. A **roadmap/guide** for how to live in the new world
and make changes locally. Credibility comes from having actually walked the path —
4 years of travel + parallel lessons lived on the ground (vineyard in Italy,
permaculture in Auroville, community in Medellín, farms/projects worldwide).

## The core reframe
- Work CV = credentials. Travel history = **lived evidence**, and it's the biggest asset.
- Travel is the proof-of-concept (embodied, first-person); research is the
  proof-of-generality (the data that it holds beyond my own story).
- Thesis the whole site stands on: these ways of living are measurably more
  fulfilling, healthier, and more sustainable — and here's the evidence.

## Governing frame: INSIDE → OUT
Everything begins with **pure awareness**, then drips outward in widening spheres of
influence: awareness → self → home/family → world. "Be the change," given actual
architecture. This is the spine of the whole site AND the meaning of the hero
animation. The three domains are not a flat list — they are concentric rings of
effect. You tend the self, which lets you shape your immediate place, which ripples
into the wider world.

## Structure (concentric — awareness → self → home → world)
- **Center (the sun):** **Pure awareness / meditation / concentration** — the
  source everything radiates from. The contemplative stance *is* the research
  stance (clear seeing, honest inquiry). Oriented outward toward care for one's
  neighbor and the health of life itself. ("Everything starts internally" points
  literally at this.)
- **3 spheres of influence (inside → out):**
  1. **Self — Health & Wellness** (inner work): body and its rhythms — astrology,
     Ayurveda, Chinese herbs, movement + dancing (dance folded in here, not standalone).
  2. **Home — Home & Land development** (immediate surroundings): building,
     permaculture, conscious tech use, conscious resource use.
  3. **World — Trading, Markets & wider topics** (external sphere): how markets,
     tech, and resources are reshaping the world.
- Ordering (01/02/03) is now meaningful — a journey outward, not an arbitrary list.
  Sub-pages can be sequenced that way.
- **Connective tissue (Research):** NOT a 4th pillar — the evidence layer running
  through all three. Cuts across each domain via three lenses:
  - *Science* (mechanisms) · *Medicine* (health outcomes) · *Applied physics/tech*
    (implementation).
  - Any entry locates by **pillar × lens** (e.g. Health×medicine: meditation RCTs
    & inflammatory markers; Land×physics: earthen vs conventional thermal perf;
    Markets×science: energy accounting of PoW vs real-resource backing).
  - **Grade the evidence honestly:** well-established / promising-but-early /
    still-contested. Intellectual honesty is the persuasion. Avoid the
    wellness-influencer-cherry-picking failure mode. (Physics-brain instinct:
    evidence, not advocacy dressed as evidence.)
- **Harvest (Writing):** the arguments/guide built from the evidence. Mark
  "coming soon" for now; crystallizes out of the research over time.

## Front door — the unresolved decision
Audience is really *both* (skeptics + the already-sympathetic), but a page can only
*open* one way. Two routes:

- **Route A — Why first** (for the not-yet-convinced): problem → evidence → lived
  proof → roadmap. Center of gravity = Research + travel story. Wins with a smart,
  skeptical audience (physics/markets crowd). Risk: ready-to-act readers wade
  through convincing they didn't need.
- **Route B — How first** (for the sympathetic): the roadmap up front → domains →
  evidence underneath if you want it → my story as a companion who's walked it.
  Wins with people starved for credible, non-fluffy *how*. Risk: skeptic bounces
  before being convinced.

**The "both" move:** only the front door has to choose. Pick one as the hero's
opening gesture, build the other as the immediately-adjacent track — same spheres,
same research, two entry points, reader self-selects. A landing fork:
"New to this? Start with why." / "Ready to move? Start with the map."

**My leaning:** thin layer of Why (one sharp evidence+experience-backed line that
this is real, not fluff), then hand off fast to How. Travel story threads through
both as proof.

**What the inside-out frame suggests on its own:** the site could open at the
center (self) and invite the reader to move outward with you — a how-leaning,
journey-based entry. The reader starts where they already are (themselves) and
expands. This leans Route B, with a thin Why layer at the very top.

## Open questions to resolve
1. Which door opens first (A or B) — settles most of the shape.
2. Does Trading sit comfortably beside the contemplative pillars, or need a
   bridging frame? (The "resources / how the world is changing" angle does that work.)
3. How explicit to make the service / "health of life itself" mission — stated
   line, or implicit tone?
4. Research: my-own-inquiry-made-public vs curated-evidence-library vs both
   (investigation *through* the existing literature).

## Build status (existing code)
Single self-contained `index.html` (no deps) + `practices/` (5 sub-pages from a
shared template) + this brief. Dark, line-art aesthetic on black.

**Hero visuals (built):**
- A "sun" (filled gold orb + wavy corona) rising as a half-circle cut at the
  hero's bottom edge, stable across viewport ratios.
- 3 concentric rings = the spheres of influence, now color-coded:
  **gold = self (inner), sage = home (mid), indigo = world (outer)**, each with
  a node sitting on it.
- One enclosing dashed teal arc (the world's edge).
- A large partial elliptical orbit wrapping around the headline + the sun's lower
  edge; never crosses the words at any screen ratio (tested ultrawide→phone).

**Hero animation — NOW enacts inside→out (DONE this session):**
- Sun *breathes* at center (pure awareness, the source).
- *Pulses ripple outward* from the sun continuously, staggered so the drip never
  stops (CSS `emanate` keyframe; 3 pulses, 6s cycle, 2s offsets).
- Each ring + node *lights up in sequence* as the wave reaches it: self → home →
  world (`receive`/`arrive` keyframes, ~1.1s stagger).
- Replaced the old idle orbit-spin. Reduced-motion stills it all cleanly.

**STALE — predates the reframe, needs rework:**
- Hero copy: eyebrow still "Markets · Shelter · Breath · Motion · Notes",
  headline "Baba / works in cycles", old lede. Undersells the self→home→world
  story — rewrite to match the frame.
- 5 sub-pages (self-development, home-community, systems-notes, trading, dancing)
  are the OLD "five parallel practices" model. New model is 3 spheres + awareness
  center + research (connective) + writing (coming soon). Restructure.
- About/contact: placeholder copy; contact links are dummies
  (you@example.com, Instagram/Notes → #). GitHub → nondescrypto.
- Ring colors (gold/sage/indigo) are a first pass — retune if a self/home/world
  palette is chosen.

**Key files:**
- `index.html` — home (hero animation current; copy + grid stale)
- `practices/*.html` — 5 old-model pages, shared template
- `site-brief.md` — this doc
