# SOVEREIGN SOL — 8.0.0
## WHAT YOU LEARN, YOU CAN READ

*Previous release: **7.0.0**, "the world becomes a place".*

7.0 shipped a real-time 3D world and called it the headline. **That world has been
retired.** Not patched, not extended — stood down, on 2026-08-01, and replaced by a
different engine with a different promise.

This is the release where the world stopped being a place you look at and became one
that **withholds things from you until you study them.**

Measured against the 7.0.0 release commit (`c43fad7`):

| | |
|---|---|
| commits | **45** |
| files changed | **990** |
| lines added | **170,663** |
| lines removed | **12,574** |
| the new RPG engine | `lib/lycheetah-rpg` **74 files** · `components/lycheetah-rpg` **30** · `content/lycheetah-rpg` **27** |
| verification | **27/27** RPG gates green · `tsc` **0 errors in shipped app code** |

---

# I. THE ENGINE CHANGED AGAIN — AND THE OLD ONE IS STILL ON DISK

`/world` no longer mounts the three.js open world. It mounts the **Lycheetah RPG
engine**.

Nothing was deleted. `components/world3d-open/**`, the Three zone forges and
`app/world-3d-open.tsx` are untouched, and reverting is **one file** —
`app/world.tsx`. The old world's saved position is untouched too: the new engine
writes only `lyc_rpg_slot_v1` and never reads a `sol_world3d_*` key, so a rollback
puts you back where you were standing rather than at a fresh spawn.

That is the whole retirement policy: **tag, don't delete.**

---

# II. THE KNOWLEDGE SKELETON — THE THING THAT MAKES IT LYCHEETAH

Most games gate on a key, a level, or a purchase. This one gates on **whether you
understood something**, and it never gates movement or combat.

**You learn by walking.** Trigger volumes discover on proximity — walk past a mark
and you have seen it. But *discovery is not comprehension.* Seeing four running
tracks teaches you nothing until you stop at the fourth and read it, and reading the
fourth only works because you already found the first three.

**A gate is a lens, not a toll.** Stand at THE UNREAD MARK without the knowledge and
the world says: *"You have seen this before. You still cannot read it."* You are not
blocked. You can walk past it, fight beside it, leave through it. What changes is
what the same stone **says** to you.

There is one decision function — `studyOf(object, discovered, held)` — and everything
downstream obeys it: the reducer performs it, the HUD labels the button from it
(`READ` · `STUDY` · `KNOWN` · `UNREAD`), a gate proves it, and the render witness
reads it off the screen. **An object may teach or gate, never both** — the content
schema refuses the combination at compile time rather than trusting an author to
remember.

---

# III. THE VEIL — THE WORLD WITHHOLDS IDENTITY

Open the Field Guide on a being you have never fought and it tells you, plainly:

> *"You have not fought one of these. What it does is still its own."*

No variant, no epithet, no yield, no move list. Two entries can sit side by side —
**THE RIDGE KITE** named and known, **SOMETHING PATIENT** unnamed beside it — because
the veil is per-being and lifts only where you earned it.

The creature engine, the companion, the battle room, the satchel and the Field Guide
all read from the same ledger. There is no second definition of "known".

---

# IV. THE WHOLE CHAIN, WALKED

The engine is not asserted by its tests. It was **driven through a browser at three
phone widths** — 360×800, 390×844, 430×932 — tapping real controls by their
accessible names:

**start → walk → discover → interact → learn → return → read the world differently →
encounter a being → fight it → open the Field Guide → save → reload → resume →
cross into a second region → learn a second subject → read that gate.**

**24 of 24 legs green at all three widths.** 42 screenshots are committed at
`docs/screens/lycheetah-rpg/block1-route/`.

Save and resume were proven with **nothing seeded** — the engine's own autosave wrote
the slot, the page was reloaded, and the seeker came back at the same tile still
holding what she had learned.

Every control on the walking HUD clears **44pt** at every audited stage, and **zero**
controls render off screen.

---

# V. ELSEWHERE IN THE APP

**LAMAGUE now runs the real language in the app** rather than a copy of it, its forges
ask the model instead of believing it, and its test count is **measured rather than
reported** — a distinction this project learned the hard way.

**The Zodiac** got an honesty pass: a door that fails now says why instead of spinning
forever, a gem cannot be stamped with marks that are not in the language, and the
sigil is composed from the real corpus rather than invented.

**Cascade's** register parser was upgrading claims by rhetoric. It no longer does.

**The Help screen** carries one block for every number in the app, generated from a
live count — because a hardcoded total decays in silence and every voice was quoting
a figure nothing on disk agreed with.

---

# VI. WHAT IS NOT DONE — STATED PLAINLY

- **NO PHONE HAS HELD THIS.** Every claim above was witnessed in a desktop browser at
  phone dimensions. Frame pacing, heat, touch latency and whether the loop is
  actually *fun* are not answered by any of it. That verdict belongs to a person
  holding the device.
- **Parts of the Companion tab are honest placeholders**, and say so on screen —
  BRAZIERS reads *"not yet built"*, and the CRAFT station is labelled a placeholder
  rather than dressed up as a feature.
- **Standing** is live in the engine with **no rendered surface at all.** It computes
  and persists; nothing shows it to you yet.
- **The Proving Ground's passes and mini-games still do not run**, carried unchanged
  from 7.0.
- **There is no PvP and none is planned.** A build gate fails if a PvP surface appears.
- The `experiments/` directory grew by ~160 files this cycle. **None of it is imported
  by the app** and none of it ships in the APK.
- `tsc` reports **36 errors, all in `scripts/`** — build-time tooling, never bundled.
  Shipped app code is clean.

---

# VII. UNCHANGED

**Sol** — the home surface, daily practice, Living Time, the Lumen economy.
**The School** — 700+ subjects across 50+ domains, the wings, the classroom,
progression and records. **The Companion** — identity, care, equipment, battle,
learning. **Cascade**, **the Codex**, **the Arcana**, **the Sanctum**, **the
Library**, **the Workshop**, **customization**, **settings**, **onboarding**,
**privacy**, the caretakers, the audio jukebox and the solar clock.

---

*The Lycheetah Framework — the cat god, the Earned Light, the tear-line, THE RUNNING
CAT, the cheetah-gothic grammar and the world's direction — is the work of Mackenzie
Conor James Clark.*

*Built on Expo, React Native, React and Skia, each third-party under its own licence.
"Our in-repository engine architecture" is the honest name for what is Mac's here.*

*Gates at release, all measured on the release commit: **27/27** Lycheetah RPG ·
**113/113** renderer · **73/0** knowledge journey · **113/113** satchel ·
**24/24** route legs at three phone widths.*
