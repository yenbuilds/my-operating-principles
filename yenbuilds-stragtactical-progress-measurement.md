# Measuring Progress in the YenBuilds MSFS Platform

YenBuilds is not a feature-driven product.  
It is a **compounding platform**.

That means traditional metrics (features shipped, users, polish) are not just unhelpful early — they are actively misleading.

This document defines **how progress is measured** so momentum stays real, sustainable, and irreversible.

---

## Core Rule

> **Measure irreversible progress, not activity.**

Anything that can be deleted, rewritten, or abandoned without cost is motion — not progress.

---

## 1. Architectural Progress (Hard, Irreversible)

These are the highest-signal indicators.  
If these are increasing, the platform is advancing even if nothing visible ships.

**Weekly yes / no checks:**

- A new **named invariant** was added and documented  
  (e.g. *Telemetry Source Agnostic*, *Anonymous-First Identity*, *Append-Only Landing Rows*)

- An interface or seam was **frozen**  
  (schema, contract, event shape, file boundary)

- A dependency direction was made **one-way only**  
  (HUD depends on core, never the reverse)

- A module became **swappable without refactor**  
  (FSUIPC → SimConnect remains possible)

**Metric:**  
Count of invariants + frozen seams  
If this number rises, the platform is maturing.

---

## 2. Cognitive Load Reduction (The Silent Multiplier)

Progress is also measured by how much *thinking* the system requires.

**Weekly questions:**

- Can I return after 7 days and know exactly where to continue?
- Did I delete more concepts than I added?
- Did something become obvious that used to require thought?

**Hard proxy signals:**

- Number of files that feel dangerous to open → should decrease
- Number of comments explaining “why” → should decrease
- Number of things re-explained to Copilot → should decrease

Lower cognitive load = higher future velocity.

---

## 3. Optionality Created (Future Power)

The platform wins by **making future work optional**, not by doing it early.

Track **options unlocked**, not features completed.

Examples of real progress:

- “Cloud logging could be added now, but isn’t needed yet”
- “Community landing comparisons are possible later”
- “The HUD renderer could be swapped without touching telemetry”

**Weekly check:**  
Did I unlock at least **one future path** without committing to it?

If yes, that week counts.

---

## 4. External Verisimilitude (Weak but Useful Signals)

These prevent total solipsism. They are not the core metric.

Lightweight examples:

- A diagram
- A README
- A short clip or screenshot
- A written explanation

Rule:  
If it can be explained in **one sentence**, it counts.

---

## 5. Energy Sustainability (Non-Negotiable)

This is a hard constraint.

**Binary test:**

- Working on YenBuilds preserves or increases energy
- Stopping happens by choice, not exhaustion

If energy collapses, progress is fake — regardless of elegance.

---

## 6. Explicit Anti-Metrics (What Is Not Measured)

These are banned as primary signals:

- Lines of code
- Features shipped
- UI completeness
- Early user counts
- How impressive it looks

If any of these dominate decision-making, drift has begun.

---

## Weekly Scorecard

Once per week, answer only these:

1. Was something fundamental named or frozen?
2. Did the system become simpler or more legible?
3. Was future work unlocked without being done?
4. Was energy preserved?

If **3 out of 4** are yes, the week was a success.

---

## Philosophy Fit

This system exists to:

- Prevent fake progress
- Avoid over-engineering
- Reduce rabbit holes
- Enable quiet, compounding velocity

YenBuilds is measured by **what becomes impossible to lose**, not by what gets built quickly.
