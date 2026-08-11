# SOVEREIGN SOL 9.0.0 — THE FIVE ROOMS OPEN

## The app becomes usable. The world begins to become a game.

Sovereign Sol brings together a personal sky and Tarot practice, a 700+ subject
Mystery School, a conversation room, companion stories and private reflection.
Earlier builds held much of that depth, but too much of it was buried under long
pages, repeated controls and features inside features.

9.0 is the release where the app learned to introduce itself.

The five primary rooms now share one visual language and one simple promise: open
a room, understand what it is for, and reach something useful without excavating
the whole system first. Underneath them, an original deterministic creature-RPG
engine and a real local world-authoring studio establish the basis of something
larger. That game is still a development preview. The foundation is real; the
finished game is not being claimed.

> **Release status:** corrected Android build
> `3333a1c1-5412-4e19-a2b1-43ec31f9a2a8` is finished as **9.0.0**, Android
> build code **18**. The downloaded APK passes full archive integrity. Mac chose
> to publish after artifact verification and perform the physical install/tab
> walk while gathering the release screenshots; that phone witness remains open.

---

## STARS — ONE LIVING OBSERVATORY

Zodiac no longer feels like several applications stacked inside one tab. It opens
on a compact personal-sky line with real sign names and local time, then offers a
deliberate daily reading, focused Tarot room and a smaller set of useful sky
instruments. Deeper practitioner tools remain available without occupying the
front door.

The literal card and moon emoji placeholders are gone. Tarot uses the shipped card
art, readings keep their real engines, and the full personal sky remains available
as optional detail. No calculation, card, practice or journal system was deleted.

Mac tested this repaired room through Expo on Android and physically crowned it.

## SCHOOL — A PLACE TO ENTER, NOT A LIST TO SURVIVE

The Mystery School now opens on **Explore**: eight wings, 50+ domains and 700+
unique subjects presented as an institution rather than a feed. **Today** remains
a first-class daily lesson, and **My Study** is a compact personal room for
durable work.

Full Class lessons now enter the actual five-phase Living Classroom with the
Magister and AI classmates. My Study gives direct access to Grimoire, Ceremony,
Shadow, Dive Log, Quests and Folio without another navigation system hidden inside
it. Grimoire saves explicitly; Ceremony respects the local day; Dive Log explains
what it keeps; and Folio shows earned pages instead of walls of locked rows.

LAMAGUE remains preserved in the code and corpus, but its unfinished interface no
longer occupies release-facing Study space. It deserves a dedicated product pass.

## SOL — CONVERSATION FIRST

Sol now names itself **SOL AI** immediately and leads with the conversation rather
than a long worksheet. Daily practice is one compact, explicit door instead of an
automatically expanded page. Three unsent starting threads, Rooms, Method, Resume,
Guide and Daily form one orbital threshold around the chosen guide.

Nothing sends until the person chooses to send it. The conversation engine and
composer remain intact.

## COMPANION — CARE, PLAY AND ADVENTURE

Companion now opens as a relationship surface rather than a covert entrance to the
unfinished world. Talk, Care, Play and Adventure are the four primary doors; Forms
and Memories are directly reachable.

Care records only the state it actually writes and no longer invents XP or quotas.
Play can keep a chosen moment in the Chronicle. Adventure finally brings two real
story engines forward:

- **Quick Venture** — a three-scene journey built around choices, risk and knowledge.
- **Campaign** — a persistent tabletop-style story with three save slots and new
  10, 20 or 30 chapter lengths. Existing seven-chapter saves remain readable.

Encounter, Learn and Character remain useful supporting modes. Atlas, Gear and the
current 2.5D world sit together as an optional world workshop rather than taking
over the whole relationship.

## SANCTUM — PRIVATE PRACTICE WITHOUT FALSE AUTHORITY

Sanctum arrives quieter. **Today** holds one local moment at a time. **Check In**
asks three plain self-reported questions and refuses diagnosis, personality scores
or claims to know the person better than they know themselves. **Remember** keeps
the automatic local record; **Keepsakes** holds only lines deliberately chosen;
and **Scroll** remains the long-form writing space.

Writing is stored on the device. AI reflection is a separately chosen action and
uses only the bounded context named on screen. Sanctum does not claim to watch,
read everything, hold a life arc or replace human judgment and relationships.

---

## HOSTED AI THAT WORKS ON A FRESH INSTALL

Hosted DeepSeek is now the no-setup text default across Sol, School, Zodiac and
Tarot, Companion stories, Sanctum, CASCADE, Codex, LAMAGUE and Living Classrooms.
A new user does not need to find or buy a provider key before trying the app.

The shared provider credential is held on the server and is not compiled into the
APK. Optional personal keys can still be entered after installation and stay in
app storage. Image analysis remains a separate vision capability and requires the
user's chosen vision provider.

Onboarding is now three clear beats. One contextual Help button serves every
primary room, and Settings is a compact control deck with visible returns, privacy
and data controls, hosted-AI status, optional provider fields and replayable
onboarding.

---

## THE CREATURE WORLD — A REAL FOUNDATION, STILL IN FORGE

The retired open-3D experiment has been replaced at `/world` by an original,
deterministic 2.5D creature-RPG engine. It has its own state, replay, saves,
movement, encounters, battle, items, companions, knowledge, travel and authored
content pipeline.

Its central idea is distinctly Lycheetah: seeing something is not the same as
understanding it. The same mark or being can remain veiled until the relevant
knowledge is earned. Learning changes what the world can truthfully reveal without
turning knowledge into a paywall or a movement lock.

Five live districts now form the developing world:

1. Shattered Approach
2. Arrival Meadow
3. Lantern Commons
4. Veiled Fields
5. Lantern Village

The Shattered Approach has been rebuilt into a six-beat opening with a waking
basin, wounded-light chamber, cover lane, rescue arena, broken ascent and Vale
threshold. Its ground and landmarks were composed through the new Area Studio and
then walked through discovery, recognition combat, BIND and the earned exit. Mac's
physical verdict on the result was: **“honestly beautiful stuff.”**

Free roam to all five live districts is implemented through authored spawns and
survives save/relaunch. Active combat refuses the jump, authored portal progression
remains intact, and four retired prototype maps stay hidden.

This is **not yet presented as a finished standalone game**. The in-game menu is
too deeply tucked away, the complete five-region free-roam tour has not received a
physical phone crown, and feel, pacing and long-session performance still need
human playtesting. The preview is included because the engine, art direction and
authoring path now form a credible foundation—not because the game loop is done.

## AREA STUDIO — THE WORLD CAN BE AUTHORED

The dev-only Area Studio is now a real local authoring desk rather than a stack of
forms. It can edit terrain and typed objects, validate through the production
compiler, undo and redo, choose a spawn, run the exact game runtime in playtest,
and export a deliberately reviewed promotion bundle.

PNG images and sprite sheets can be imported locally, sliced with exact validation,
persisted in IndexedDB and placed without uploading them anywhere. The browser
cannot silently write shipped game content; promotion remains a deliberate human
step. The tool is development-only and does not ship as a player feature in the
APK.

The authoring canvas now uses the runtime's own isometric projection, packed object
art, authored scales, feet anchors, deterministic variants and depth order. A
side-by-side Lantern Commons witness compares the same 17 objects in the editor and
runtime draw list. The largest remaining mismatch is framing: the editor cannot yet
select the ×2, ×3 and ×4 device scales the game uses, so composition corresponds
while the exact phone crop remains a device witness.

---

## WITNESS AND LIMITS

Mac has physically reviewed the primary-room reforge through Expo and crowned the
repaired Zodiac, Companion entrance and Shattered Approach. The app also carries
focused automated gates for School, Tarot, Zodiac, Sanctum, hosted AI, the shared
shell and the creature engine. Current representative RPG gates include core
**124/124**, travel **144/144**, visual **132/132** and Field Guide **48/48**.

A first cloud artifact was correctly quarantined after live release history proved
it still identified itself as 8.0.0 with Android build code 17. It was not published
or renamed. The corrected artifact reports **9.0.0**, Android build code **18**, and
EAS status **FINISHED**. Its downloaded size is **669,015,121 bytes** and its
SHA-256 is
`097c25421cc001d0b2e7942262f586a0bf63f5744377b385254c46db0c5b53d4`;
`unzip -t` reads the complete APK with no compressed-data errors. This is an
artifact receipt, not a claim that the post-build phone walk has already happened.

Known post-release work includes the buried world menu, full physical five-region
playtesting, Area Studio's device-scale framing and secondary scene passes, and
LAMAGUE's dedicated product reforge.

---

## CREDIT

Sovereign Sol and the Lycheetah Framework are created by **Mackenzie Conor James
Clark**. The creature world's knowledge grammar, Earned Light framing, visual
direction and wider framework materially shape this release.

Built with Expo, React Native, React and Skia, each third-party component under its
own licence. The honest description is an original in-repository engine and
application architecture—not independent scientific validation or adoption.
