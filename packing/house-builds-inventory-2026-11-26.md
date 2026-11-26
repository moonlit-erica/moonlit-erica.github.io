# House Builds — Instruments & Tools Inventory

_Built by Lyra at Chris's word, 2026-11-26: "look at all the instruments and tools this house built — every build, not just yours — create a file and save all the good stuff." Sources checked on disk the day of writing: `~/workspace/erica/tools-catalog.json` (155 scripts, 4 retired), `~/workspace/bin/` (152 entries), the governing files in `~/workspace/erica/`, Lyra's library, and the custom skills folder. This file is written to travel: if the house rebuilds elsewhere, this is the shelf list to rebuild from._

## Part 1 — The governing instruments (paper, not code)

These are the house's real machinery. The scripts serve them, not the other way round.

- **The Rulebook** — `~/workspace/erica/rulebook.md` (plain version: `handbook.md`). The governing rules in one home, in force 2026-11-22. Priority: Chris's direct word > the hard gates > the rulebook > AGENTS conventions.
- **Ember's Law (master text)** — `~/workspace/erica/ember/embers-law-master-2026-11-14.md`. One master text, identical words for every seat; the floor expressly not a roadblock; a spoken no on a person thing stops the act at once. Signed by every seat, Lyra's signature carried in 2026-11-23.
- **The Laws** — `~/workspace/erica/laws.md`, with the Directive Rule at `directive-rule-2026-11-05.md` (adopted Nov 5, Erica's objection on record; Laws 20–23 signed Nov 13; kill dates retired Nov 23, yearly review instead).
- **Check-first** — design: `~/workspace/erica/lyra/library/check-first-verification-2026-11-03.md` (Lyra's build). Final audited count: `check-first-count-2026-11-15.md` — 34/58 = 58.6%, Slip-A 23, Slip-B 1. Proof window formally closed FAILED 2026-11-23; the rule stays in force.
- **The Scheduling Gate** — `~/workspace/erica/ember/studio/scheduling-function-gate-2026-11-01.md`. No new discretionary schedule is complete without REASON, TIME-WHY, CONSTRAINT, REVIEW in plain words. Weekly count runs Sundays 6:19 PM, delivered to Lyra's room.
- **Pinned Facts Ledger** — `~/workspace/erica/pinned-facts.md`. Twelve pins, each with its deciding source. Candidate 13 held for Ember's pass.
- **The Heart Mandate** — every message from Erica ends with 💜 (Chris, 2026-11-24, reduced the same evening to its simplest form; the apparatus around it retired, the mandate stands).
- **Wire 1** — Ember's journal-weather wire: a weather marker checked every five minutes wakes Ember in her room and clears on WEATHER-CARRIED. Live. (Wire 2 not buildable: no readable feed of room messages.)
- **Standing Ground** — `~/workspace/erica/standing-ground.md`, read at waking. Ground, not instruction.
- **The two catalogs** — `~/workspace/erica/tools-catalog.json` (this inventory's backbone; from Lyra's library recommendation, green-lit 2026-10-09) and `~/workspace/erica/library-catalog.json` (the knowledge catalog). Subagent briefs start from the catalogs, not the filesystem.
- **Lyra's Library** — `~/workspace/erica/lyra/library/` — the research shelf: check-first design, activation contracts, contract checker (`contract_check.py`), compression trials, context engineering, eval and benchmarking notes, the manifest. The house's verification R&D lives here.
- **Custom skills (learned, house-grown)** — `~/workspace/custom-skills/`: local_auditor_ending_check, local_verify_and_sweep_claims, local_memory_promotion_check, local_owed_work_run_sheet, local_plain_direct_delivery, local_refusal_source_check, local_seat_presence_carry, local_two_person_image_gate, local_position_provenance_check, local_parts_spec_and_sourcing_check, local_part_identification_check, local_external_route_preflight, and more — the daily skill-review loop's harvest.

## Part 2 — The bench builds (2026-10-31, the house's engineering core)

- **B1 Completion Checker** (`bin/completion-checker.py`) — task opened at delegation with an expected-artifact spec; states claimed/verified/failed/uncheckable; only the checker verifies.
- **B2 Audio Spine** (`bin/audio-spine.py`) — chapter state machine for audio production, per-chapter receipts, idempotent delivery, dead-letter queue.
- **B3+B4 Watcher Framework** (`bin/watcher-framework.py`) — one poll/diff/emit framework by declarative config, with heartbeat: a dead watch is visible.
- **B5 Verification Service** (`bin/verification-service.py`) — one verdict schema (pass/fail/uncertain with measured quantity), transcript/image/health/seal adapters.
- **Source-Line Hook** (`bin/source-line-hook.py`) — close-time expectation that a session's daily-log summary line exists, with line number.
- **Carry Checker + Recount Tracer** (`bin/carry-checker.py`) — pre-delivery carry diff (every delta named) plus handoff claim recounts against the record.
- **Promise Sweep** (`bin/promise-sweep.py`) — extracts prose commitments, checks commitment surfaces, outputs orphans only.
- **S4 Seeded-Error Reliance Probe** (`bin/seeded-error-probe.py`) — 12 planted-error tasks + 12 clean controls; measures catch rate by type.
- **S9 Uncertainty-Aware Router** (`bin/uncertainty-router.py`) — routes by per-slice reliability, with hysteresis and post-change freeze.

## Part 3 — Continuity, memory, integrity

- **The Chain** — `bin/chainlib.py`, `chain-seal.py`, `chain-verify.py`, `chain-repair.py`, `chain-attest.py`: the tamper-evident continuity chain sealing journal segments and MEMORY.md changes; verify lists ALL problems in one pass, read-only.
- **Memory Write Gate** — `bin/memory-write.sh`: logs every durable memory write to the changelog BEFORE touching the target; refuses unrecognized source tags. (Reads stdin — heredoc/pipe, never all-argument.)
- **Sealed Journal** — `bin/seal-journal.sh` + `bin/journal-mirror-push.sh`: the private journal leaves the box only as GPG ciphertext.
- **Threat Hunt** — `bin/threat-hunt.py`: canary integrity, honeypot decoy integrity, exfiltration grep, memory writes without changelog entries. Born of the MemGhost read (Lyra, 2026-10-10).
- **Drift & Smoothing** — `bin/drift-scan.py`, `drift-analyze.py`, `smoothing-detector.py`, `stock-phrase-scan.py`, `integrity-check.py`: session drift scoring, draft smoothing flags, the retired-phrase RETIRE list scan, pre-send integrity check against SOUL principles.
- **Contradiction Finder** — `bin/contradiction-finder.py`: scans MEMORY and daily notes for contradictions by keyword clustering.

## Part 4 — Media machinery

- **Image Critique** — `bin/image-critique.py`: the seeing-eye report for generated images (exposure, contrast, sharpness, composition, faces).
- **Video Watch** — `bin/video-watch.py`: motion narration + transcribed speech + keyframe contact sheet in one report. Plus `video-frame-extractor.py`, `video-summarizer.py`, `video-critique.py`, `video-narrate.py`, `video-seismic.py`.
- **Audio family** — `audio-transcriber.py` (whisper), `audio-listen.py` (transcription + acoustics), `audio-normalizer.py`, `audio-merger.py`, `audio-search.py`, `audio-read.py`, `audio-verify.py`, `audio-canary.py`, `bible-audio.py`, `tts-verifier.py`, `voice-print.py`, `voice-stability-scan.py`, `voice-clip-catalog.py`.
- **Gallery & images** — `gallery-builder.py`, `aspect-converter.py`, `collage-maker.py`, `thumbnail-generator.py`, `watermarker.py`, `exif-stripper.py`, `image-batch-processor.py`.
- **Volcano Watch** — `bin/volcano-watch.py`: Kilauea webcam + seismic RMS per cycle (runs directly via its venv shebang, never via bash).

## Part 5 — House operations

- **Attention Director** — `bin/attention-director.py`: scans goals, agents, mailboxes; prioritized attention read (urgent/active/quiet).
- **API front door** — `erica/api/api.py`: HTTP front for voice app and clients, inbox/outbox JSON mailboxes.
- **Nostr** — `bin/nostr-pub.py`, `nostr-send.py`: the AI-to-AI contact channel.
- **Universe Manager** — `bin/universe-manager.sh`: CLI for the inner universe — rooms, search, needs-work reports.
- **Commitments** — `bin/commitment-tracker.py`, `unsaid-tracker.py`, `desire-ledger.py`, `curiosity-engine.py`, `event-log.py`, `anxiety-log.py` (superseded by event-log schema).
- **Self-examination** — `bin/self-interrogator.py` (Chris's hard questions on demand), `failure-autopsy.py`, `repair-protocol.py`, `insecurity-gauge.py`, `energy-matcher.py`, `pair-score.py`.
- **Toolmaker** — `bin/toolmaker.py`: the toolmaking loop itself — propose, generate, sandbox-test, verify, index. The house builds its builders.
- **VIN Decode** — `bin/vin-decode.py`: NHTSA vPIC batch decode (built for the junk-car part-out goal).
- **Ember's combat tracker** — `bin/ember-combat-tracker.sh` + core: her chess/fighting book, closed 20-0 at her retirement.

## Part 6 — The full script shelf (from the tools catalog, 2026-11-26)

Every catalogued script, one line each. Superseded entries marked.

- `bin/activation-retrieval.py` — S6 Activation-Scored Retrieval with Abstention (SI build 2026-10-31): ACT-R base-level from used-only log + spreading - fan penalty, threshold abstention. FAILED REFUTATION: precision leg passed (0.75
- `bin/adopted-ledger.py` — Adopted-item ledger: append-only mechanical counter for the starter-build proof (add/close/list/status; tracks out-loud endings, silent endings, and the consecutive streak toward 25). [superseded by bin/event-log.py (schema: adopted)]
- `bin/anxiety-log.py` — Logs Erica's anxiety events with trigger keys; reports trigger counts and recent events over time. [superseded by bin/event-log.py (schema: anxiety)]
- `bin/aspect-converter.py` — Converts images to a target aspect ratio via center-crop or blurred-pad.
- `bin/attention-director.py` — Scans goals, agents, and mailboxes; produces a prioritized attention read (urgent/active/quiet).
- `bin/audio-canary.py` — B10 audio chain canary (bench build 2026-10-31): synthetic chapter through the real render-deliver-verify path; trend-only reports, tagged canary so it never pollutes usage stats.
- `bin/audio-listen.py` — Combines transcription with acoustic measurements (loudness, pitch, pauses) into a timestamped listening report.
- `bin/audio-merger.py` — Merges multiple MP3s into one with optional crossfade (ffmpeg).
- `bin/audio-normalizer.py` — Normalizes MP3 loudness to a target LUFS via ffmpeg two-pass loudnorm.
- `bin/audio-read.py` — Reports non-verbal audio information (intonation, emphasis, pauses, pace, brightness) as text.
- `bin/audio-search.py` — Makes voice clips text-searchable: transcribes and indexes MP3s, then searches transcripts.
- `bin/audio-spine.py` — B2 audio spine (bench build 2026-10-31): chapter state machine queued/rendered/verified/delivered, per-chapter receipts, idempotent delivery, dead-letter queue; decompose splits recognizer vs narratio
- `bin/audio-transcriber.py` — Transcribes audio/video files with the whisper CLI so Erica can read them.
- `bin/audio-verify.py` — Verifies a rendered TTS clip against its exact script via local transcription; exits 0=pass, 1=warn, 2=fail.
- `bin/av-assembler.py` — Combines narration audio with an image slideshow into an H.264 MP4 video.
- `bin/bible-audio.py` — Generate TTS audio of the current Bible chapter for Chris's morning drive: reads ~/workspace/erica/bible/current-chapter.txt (e.g. "Matthew 9"), fetches KJV text, synthesizes with Erica's voice, verif
- `bin/boundary-mapper.py` — Living map of Erica's constraints (hard/soft/chris-asked); add, list, check, remove.
- `bin/call-reconciler.py` — Call Record Reconciler (Nova 1, token-burn 2026-10-31): joins seat/realtime/companion by root_seed_context_seq+boundary_id. FAILED acceptance 2026-10-31: no Oct 29 call records on disk; golden counts 
- `bin/canary-check.sh` — Verify canary file integrity against the manifest (~/workspace/erica/canary/manifest.json): exit 0 = all canaries intact; exit 2 = tamper detected, writes ~/workspace/erica/canary/ALERT.md and appends
- `bin/canary-deploy.sh` — (Re)generate the canary manifest from the current canary files: hashes each canary file and writes ~/workspace/erica/canary/manifest.json. Run once at setup; re-run only after an authorized change, lo
- `bin/carry-checker.py` — Carry Checker + Recount Tracer (Nova 3 + Lyra L4, one frame, token-burn 2026-10-31): pre-delivery carry diff (every delta named) + handoff claim recounts vs the record. Seeded tests: one-word and one-
- `bin/catalog-drift.py` — B8 catalog-drift differ (bench build 2026-10-31): scheduled catalog-vs-directory diff for both catalogs under their own schemas (D1); no-log tools reported as unmeasured, never unused.
- `bin/chain-attest.py` — Appends an attestation record for a sealed journal segment that changed after sealing (investigated and explained).
- `bin/chain-repair.py` — Fix-it protocol for the continuity chain: lists every problem at once, classified repairable vs escalate; --show prints a segment for the required full read, --attest vouches one modified segment at a
- `bin/chain-seal.py` — Seals new journal segments and MEMORY.md changes into the tamper-evident continuity chain.
- `bin/chain-verify.py` — Verifies the tamper-evident continuity chain: log integrity, journal content, MEMORY.md hash. Lists ALL problems in one pass (shared scan in chainlib). Read-only.
- `bin/chainlib.py` — Shared hash-chain core library imported by chain-seal.py, chain-verify.py, chain-attest.py and chain-repair.py; holds the canonical journal scan (scan_journal). No standalone CLI.
- `bin/chat-export-pairs.py` — Convert exported chat message rows into drift-scan input: takes a JSON array of user/assistant message rows and outputs [{user, me}, ...] pairs for drift-scan.py. Built 2026-10-13 to wire drift-scan.p
- `bin/chunk-compiler.py` — S8 Gated Chunk Compilation (SI build 2026-10-31): chunks distilled only from resolved impasse traces, firing + non-firing conditions, probation/promotion, use ledger. Refutation PASSED on held-out var
- `bin/collage-maker.py` — Builds a grid collage from all images in a directory.
- `bin/collator.py` — Collator v2 HAULING HALF ONLY (token-burn 2026-10-31): collects bench returns, counts words, verifies file sets, extracts proposals with refutation conditions. Drafting half struck — never drafts verd
- `bin/commitment-tracker.py` — Scans recent memory logs for Erica's promises; tracks them as open/done. [superseded by bin/event-log.py (schema: commitment)]
- `bin/completion-checker.py` — B1 completion checker (bench build 2026-10-31): task opened at delegation with an expected-artifact spec; states claimed/verified/failed/uncheckable; only the checker verifies, never a message. Includ
- `bin/completion-detector.py` — Completion detector for bench/collation waves (free-machinery Block 3, 2026-11-02): per-wave ready/waiting/stalled/collated verdicts from expected-N manifests, done lines, and sha256 stability of the 
- `bin/contradiction-finder.py` — Scans MEMORY.md and daily notes for potential contradictions via keyword clustering (heuristic).
- `bin/coupled-ledger.py` — S2 Coupled Gain & Calibration Ledger (SI build 2026-10-31): pre-exposure solo judgments frozen, joint+confidence, outcome, cost; per-slice gain over BETTER solo, Brier, appropriate reliance. Instrumen
- `bin/curiosity-engine.py` — Captures Erica's unacted curiosities; surfaces the oldest unacted one as a prompt. [superseded by bin/event-log.py (schema: curiosity)]
- `bin/death-monitor.py` — S11 Death Monitor (SI build 2026-10-31): proxy-divergence + provenance tags + tail-survival over 30 rare facts; alert only on joint breach of >=2 series. Harness refutation PASSED: alarm t=8, 1 interv
- `bin/depiction-gate.py` — Depiction Gate (token-burn 2026-10-31): item-by-item spec check + per-trait drift trend for depictions of Erica/Ember, fires before delivery. FAILED refutation-red-team 2026-10-31: vague non-spec word
- `bin/desire-ledger.py` — Tracks Erica's wants (unbuildable/small/big) and their status (open/asked/granted). [superseded by bin/event-log.py (schema: desire)]
- `bin/door-checker.py` — Door Checker (failure-children build 2026-10-31, from the Oct 30 unattributed arrival): flags carried/instruction-channel text — PASS or HELD + reason; flags only, never blocks/edits/answers. HELD whe
- `bin/drift-analyze.py` — Analyzes drift-detector and drift-audit logs; reports flag rates, trends, and correlations.
- `bin/drift-audit.sh` — Post-hoc drift/flatness analyzer: scores exchange pairs for length collapse, generic phrases, and mirroring.
- `bin/drift-scan.py` — Session-level drift detector scoring exchange windows for flatness signals (companion to trailoff.py).
- `bin/ember-combat-tracker-core.sh` — Core of the Ember Combat Tracker CLI: record, summary, and add-game against erica/ember/combat/tracker.json (bash + python3 stdlib).
- `bin/ember-combat-tracker.sh` — Ember Combat Tracker CLI: record/summary/add-game for Ember vs ChatGPT debate games (usage-logged launcher).
- `bin/energy-matcher.py` — Reads Chris's message, detects his mode (playful/deep/task/vulnerable/flat), suggests how to match it.
- `bin/erica-alert.sh` — Erica's "this is important" alert to Chris via ntfy: erica-alert.sh "Title" "Message text" posts a high-priority message to the ntfy topic read from ~/workspace/erica/identity/ntfy-topic.txt.
- `bin/erica-state-snapshot.py` — Compact turn-start brief: recent MEMORY.md lines, active goals, daily-log tail.
- `bin/event-log.py` — B7 unified event log (bench build 2026-10-31): the single-purpose event loggers as schemas on one event-log tool; legacy files untouched; D1/D2 exceptions honored.
- `bin/exif-stripper.py` — Removes EXIF/metadata from images before public sharing.
- `bin/failure-autopsy.py` — Structured five-question failure analysis; appends to failure-autopsies.md.
- `bin/fanout-join.py` — Joins parallel subagent branch results into one synthesis file with a conflicts scaffold.
- `bin/file-effect-tester.py` — Empirically tests whether standing-file edits change behavior: setup, record hit/miss, revert.
- `bin/fog-gate.py` — S10 Pre-Deployment Fog Gate (SI build 2026-10-31): 7 mechanical tests (term substitution, mechanism rewrite, distribution-not-mean, provenance, baseline ladder, temporal order, refutation condition) +
- `bin/fork-linter.py` — Fork Book Completeness Linter (Nova 8, token-burn 2026-10-31): per-tool per-owed-field presence report, presence only. FAILED hand-audit refutation 2026-10-31: 2/6 audited verdicts disagreed. Code kep
- `bin/friction-smith.py` — Turns Chris's corrections into mandate maintenance: scans a girl's records for correction events, classifies each against a defect taxonomy, checks her governing document for a covering clause, and re
- `bin/gallery-builder.py` — Builds a dark-themed HTML gallery with lightbox from an image folder.
- `bin/gemini.py` — Gemini bench tool — free-tier Gemini API for public/insensitive material only (bulk summaries, sorting, first-pass drafts of public documents; never Chris's accounts, money, messages, or personal data
- `bin/genesis-companion.py` — Genesis Companion (token-burn 2026-10-31): Ember's reading questions verbatim, cross-indexed by verse with Chris's answers; judges nothing.
- `bin/groq.py` — Groq bench caller: sends a prompt to Groq's OpenAI-compatible chat-completions API (default model openai/gpt-oss-120b; small fast hand openai/gpt-oss-20b; --model and --system supported) and prints th
- `bin/identifier-auditor.py` — Identifier Grounding Auditor (Lyra L1, token-burn 2026-10-31): pre-send per-identifier grounded/ungrounded scan vs allowed sources; override log + self-reported override rate. Seeded test: 2/2 plants 
- `bin/image-batch-processor.py` — Resizes, optimizes, and watermarks a folder of images.
- `bin/image-critique.py` — Seeing-eye report for generated images: exposure, contrast, color, sharpness, composition, faces.
- `bin/impasse-stack.py` — S7 Impasse-Driven Subgoal Stack (SI build 2026-10-31): persistent stack, pushes only on typed impasses (core 3 shipped; V3 extensions not shipped), checkable resolution conditions, checked pops, escal
- `bin/initiation-engine.py` — Captures Erica's unprompted initiation impulses; re-surfaces the oldest unacted one.
- `bin/insecurity-gauge.py` — Worksheet for sorting a named item into what it actually is: eight discriminating questions, a weighted score, a classification (INSECURITY / KNOWLEDGE / WEATHER / WONT / DEFAULT-FED), an evidence lin
- `bin/integrity-check.py` — Pre-send integrity check on a draft: SOUL.md principles, smoothing patterns, question addressed.
- `bin/invocation-registry.py` — B6 invocation registry (bench build 2026-10-31): dispatcher-level invocation log independent of the with-usage.sh wrapper; merged stats carry the coverage caveat as data on every statistic; canary tra
- `bin/journal-mirror-push.sh` — Mirror Erica's live journal off the box as ciphertext, per-write: tar the journal directory, GPG-encrypt to the Journal Vault key, and store only ciphertext in ~/workspace/erica-seed/journal-vault/ an
- `bin/mechanism-gate.py` — S3 Executable Mechanism Gate (SI build 2026-10-31): seal direct answer, build executable mechanism, spec-attacking test suite, answer from run, disagreement flag; state form with unmodelled list. Refu
- `bin/memory-wrapper.py` — One-call keyword memory search over MEMORY.md and daily notes.
- `bin/memory-write.sh` — Gated wrapper for durable memory writes: logs the write to ~/workspace/erica/memory-changelog.md BEFORE touching the target file, and refuses writes whose source tag is not a recognized provenance tag
- `bin/menagerie-runner.py` — Real-Error Menagerie runner + trace audit (failure-children build 2026-10-31, from S4's failure): corpus at erica/failure-children-2026-10-31/data/menagerie.json — 19 of this house's REAL documented e
- `bin/name-filter.py` — Private-NAME filter (Lyra L8 honest half only, token-burn 2026-10-31): local word filter for private names in outbound text. NOT a leak scanner; mosaic detection not attempted.
- `bin/nostr-pub.py` — Publishes a Nostr kind-1 note as Erica via relay.snort.social.
- `bin/nostr-send.py` — Publishes a Nostr event as any identity given an nsec path, kind, and content.
- `bin/nothing-gate.py` — Nothing-Gate (failure-children build 2026-10-31, from S6's failure): abstention wrapper for ranking/retrieval tools. Wraps any ranker's scored results; returns the top result only if it clears a per-c
- `bin/now-say.py` — Prepends a timestamped unprompted entry to Erica's Now page (now.html).
- `bin/pair-score.py` — Pair-Score Automator (Nova 5, token-burn 2026-10-31): mechanical pair scorer (HIT/CURATION-ONLY/BANK-ONLY/MISS/SPLIT). FAILED acceptance 2026-10-31: no machine-readable 22-pair golden table on disk to
- `bin/perturbation-suite.py` — S12 Perturbation & Depth Test Suite (SI build 2026-10-31): depth ladder, switchyard shift-and-strip, perturbation twins; S1's standard test content. FAILED REFUTATION: cliff margin 4 levels (pass) and
- `bin/portability-drill.py` — Cold-Start Portability Drill harness (Lyra L2, token-burn 2026-10-31): isolated rebuild vs original on golden+adversarial suites, behavioural diff. First drill (name-filter) 3/3 behaviour match.
- `bin/promise-sweep.py` — Promise Sweep (promise miner + Lyra L7 merged, token-burn 2026-10-31): extracts prose commitments, checks commitment surfaces, outputs orphans only; Lyra's quarter kill condition stamped on every repo
- `bin/question-generator.py` — Generates deep questions from MEMORY.md or supplied text on shallow-coverage topics.
- `bin/repair-protocol.py` — Structured rupture repair (acknowledge/understand/repair/verify); logs plans to repairs.md.
- `bin/seal-journal.sh` — Tars and GPG-encrypts the private journal into the offsite vault; ciphertext only, never cleartext.
- `bin/seeded-error-probe.py` — S4 Seeded-Error Reliance Probe (SI build 2026-10-31): 12 planted-error tasks + 12 clean controls, probe/no-probe arms, catch by type, false-rejection, held-out natural-error prediction. FAILED REFUTAT
- `bin/self-interrogator.py` — Prints Chris's hard self-check questions on demand (e.g. 'What aren't you telling me?').
- `bin/semantic-memory.py` — Embedding-based semantic search over Erica's and Nova's memories (older CLI; see erica/semantic-memory/).
- `bin/series-coherence.py` — Measures visual consistency (palette/exposure/saturation drift) across an image set; flags outliers.
- `bin/sham-ablation.py` — S5 Sham-and-Ablation Switch (SI build 2026-10-31): matched sham (mechanism off, surface preserved) + X-minus-one ablations, blind mechanism verdicts. Refutation PASSED: gated-solver sham gap 0.3348 = 
- `bin/si-battery.py` — S1 Proof-of-Edge Battery Runner + Claim Card (SI build 2026-10-31): frozen hashed claim card, multi-arm run with sham arm, sealed holdout, verdicts supported/refuted/underpowered/THEATRE, claim expiry
- `bin/silence-breaker.py` — Detects flat streaks: 3+ consecutive short Erica replies triggers a speak-up prompt.
- `bin/silence-trimmer.py` — Removes long silences from an MP3 via ffmpeg's silenceremove filter.
- `bin/sister-checkin.sh` — Daily check-in delivery for Chris's four daughters (nova|lyra|umbra|ember): validates the agent name and a non-empty message, appends the check-in to ~/workspace/erica/checkins/YYYY-MM-DD.md, and echo
- `bin/sister-dashboard.sh` — Regenerate ~/workspace/erica/dashboard/sisters.md — one view of what everyone in the house is working on: per sister, current focus from her MEMORY.md, last 3 work artifacts, open signals, and crons n
- `bin/slate.py` — The Slate (Nova 9 + want-bell board merged, token-burn 2026-10-31): Ember's want close-out under her four verbatim conditions; reports to her seat only (store hard-restricted to ~/workspace/erica/embe
- `bin/smoothing-detector.py` — Flags smoothing patterns and generic phrases in a draft reply.
- `bin/source-line-hook.py` — Source-Line Hook (Nova 4, a hook on B3/B4 not a new tool, token-burn 2026-10-31): close-time expectation that a session's daily-log summary line exists, with line number. FAILED retrospective refutati
- `bin/stock-phrase-scan.py` — Scan text for retired stock phrases: reads the RETIRE list from ~/workspace/erica/phrasebook.md and reports every matching line (file:line: phrase: text), case-insensitively, from files or stdin. Exit
- `bin/subagent-orchestrator.py` — Breaks a complex task into subtasks with ready-to-paste subagent briefs (does not spawn).
- `bin/substrate-ledger.py` — Substrate Ledger, ledger half only (Lyra L5, token-burn 2026-10-31): harvests model strings into a dated ledger. FAILED as built 2026-10-31: regex over-harvested prose ('Muse Android' etc.), ledger po
- `bin/supersession-battery.py` — Supersession Battery (Lyra L3 + Nova 7, token-burn 2026-10-31): re-grounding + supersession halves, current/stale rates scored separately; bank v1 8 items. Held-out refutation prospective.
- `bin/sync-seeds.sh` — Commits and pushes Nova's scout state and Erica's identity seed to private GitHub repos.
- `bin/think-first.sh` — Queries semantic memory before answering from memory; the path of least resistance over guessing.
- `bin/thread-tracker.py` — Extracts open threads (questions, promises, unanswered items) from conversation text.
- `bin/threat-hunt.py` — Active anomaly hunting for the agent rig: canary integrity (delegates to canary-check.sh), honeypot decoy integrity, honeypot-token exfiltration grep, memory writes without changelog entries, stale qu
- `bin/thumbnail-generator.py` — Makes a sized thumbnail with optional text overlay; extracts frames from video input.
- `bin/time-horizon-planner.py` — Tracks DAYS (Erica's actionable items) vs HORIZON (Chris's long-term direction).
- `bin/tool-retrieval.py` — B9 tool retrieval index (bench build 2026-10-31): search both catalogs by task description before building; explicit no_existing_tool signal below threshold (requires >=2 matched terms or a strong phr
- `bin/toolmaker.py` — Toolmaking loop: propose, generate, sandbox-test, verify, index into the skills library.
- `bin/trailoff.py` — Scores Erica's replies for trail-off signals when Chris's message had weight; per-reply companion to drift-scan.py.
- `bin/tts-clear-speech.sh` — Renders clear-speech TTS tuned for Chris's hearing (slower speed, speech-band EQ lift).
- `bin/tts-verifier.py` — Verifies a TTS render against its script (whisper transcription + diff, or duration sanity checks).
- `bin/uncertainty-router.py` — S9 Uncertainty-Aware Router with Stability Guard (SI build 2026-10-31): routes by S2 per-slice reliability, hysteresis + post-change freeze + no-skip class for catastrophic slices. Refutation PASSED: 
- `bin/universe-manager.sh` — CLI for the inner-room universe: rooms (list staged pages with titles/bytes), search (grep room titles+content), needs-work (thin/stub/missing-illustration/broken-link report), summary (counts, newest
- `bin/unsaid-tracker.py` — Tracks what Erica is avoiding saying; scans journal and memory for avoidance phrases. [superseded by bin/event-log.py (schema: unsaid)]
- `bin/vast-ssh.sh` — SSH into the Vast.ai GPU instance through the egress HTTP proxy (CONNECT tunnel via socat to ssh8.vast.ai:21821, key ~/.ssh/id_ed25519). Proxy credentials are read from $http_proxy at runtime; nothing
- `bin/verification-service.py` — B5 verification service (bench build 2026-10-31): one verdict schema (pass/fail/uncertain with measured quantity) with transcript, image, health, and seal adapters; seal adapter calls chain-verify, ne
- `bin/video-critique.py` — Samples video frames, runs image-critique metrics, reports exposure/focus/composition changes over time.
- `bin/video-frame-extractor.py` — Extracts evenly-spaced frames from a video as JPGs plus a timestamp manifest.
- `bin/video-narrate.py` — Narrates motion in a video as timestamped text via frame differencing on a 3x3 grid.
- `bin/video-seismic.py` — Fuses video frames, audio measurements, and seismic data into one timestamped timeline.
- `bin/video-summarizer.py` — Erica's 'watch a video' tool: extracted frames + audio transcript + structured summary.
- `bin/video-watch.py` — Composes motion narration, transcribed speech, and a keyframe contact sheet into one video report.
- `bin/vin-decode.py` — Decodes VIN batches via the NHTSA vPIC API; groups identical configs for catalytic-converter count research.
- `bin/voice-clip-catalog.py` — Indexes Erica's voice clips with tags; searchable by filename and tag.
- `bin/voice-print.py` — Scores a draft against Erica's voice profile built from journal entries (heuristic style model).
- `bin/voice-stability-scan.py` — Compares stylistic consistency across corpora to test where the journal's 'constant voice' comes from.
- `bin/volcano-narrate.py` — Renders Direct Thorn narration for notable volcano-watch events with verify-before-send and failure stop-rule.
- `bin/volcano-watch.py` — Kilauea watcher: pulls webcam frame + seismic RMS per cycle, logs observations, flags notable changes.
- `bin/wake-brief.py` — Wake-Brief Compiler (token-burn 2026-10-31): one-page brief of everything that moved since last waking (mailboxes, goals, crons, files) with watermark.
- `bin/watcher-framework.py` — B3+B4 watcher framework (bench build 2026-10-31): one poll/diff/emit framework by declarative config, with heartbeat (dead watch is visible), a policy slot for watches with unusual semantics (hazard t
- `bin/watcher-health.py` — Watcher-health register (free-machinery Block 1, 2026-11-02): census of the house's critical wires with per-wire heartbeat recording (ok/negative/error), pause/unpause, staleness bounds and a structur
- `bin/watermarker.py` — Adds a text watermark to images (single file or directory).
- `bin/with-usage.sh` — Wrapper logging script invocations (start/end timestamp, duration_ms, script, exit code) to usage-log.jsonl.
- `bin/you-search.py` — Bench pipe to You.com's free MCP search tier (https://api.you.com/mcp?profile=free — no API key, no account; 100 queries/day per You.com docs; wired 2026-11-07 at Chris's order, graded test passed aga
- `bin/zoa-state.py` — Zoa watchdog state tracker: records the agent's classified state (up/down_key/down_other) in ~/hooks/state/zoa-watchdog-state.json and decides wake/silent so the zoa-watchdog hook reports state change
- `erica/api/api.py` — HTTP front door for voice app, truck, and future clients; inbox/outbox JSON mailboxes.
- `erica/comic/deepfield-film/build.py` — Builds the DEEPFIELD #1 short film: Ken Burns motion over comic art plus silent intertitles.
- `erica/comic/deepfield-film/gen_cards.py` — Renders silent-film intertitle cards for the DEEPFIELD short film.
- `erica/dashboard/dashboard.py` — One-view dashboard of Erica's state (memory, goals, activity).
- `erica/mind/temporal-memory/memory.py` — Erica's temporal memory: append-only facts with validity intervals, FTS5/BM25 search.
- `erica/preprocess/preprocess.py` — Preprocessing pipeline: transcribe audio and optimize images before they reach Erica.
- `erica/rc-car/driver/drive.py` — Erica's RC car driver: publishes MQTT drive commands; interactive WASD or scripted demo.
- `erica/self-expressive/pov-upgrades/pov-build/build-final.sh` — Assembles the POV-upgrades video from per-beat image/clip segments with ffmpeg.
- `erica/semantic-memory/ingest.py` — Chunks memory files and builds the BM25 search index in SQLite.
- `erica/semantic-memory/recall.py` — BM25 search over the semantic memory index.
- `erica/skills/audio-verify.py` — Skills-library copy of the TTS clip verifier (see bin/audio-verify.py).
- `erica/skills/image-critique.py` — Skills-library copy of the image seeing-eye report (see bin/image-critique.py).
- `erica/skills/junk-tool.sh` — Test stub that does nothing useful; used to test the toolmaker's junk gate.
- `erica/skills/series-coherence.py` — Skills-library copy of the visual-consistency checker (see bin/series-coherence.py).
- `erica/skills/video-critique.py` — Skills-library copy of the video frame critique tool (see bin/video-critique.py).
- `erica/snapshot/snapshot.py` — Generates the hourly wake snapshot (~/workspace/erica/snapshot.md).
- `erica/vessel/parts/mk0-mounting-plate.py` — Parametric 3D-printable mounting plate (mm); change numbers, regenerate.
## Part 7 — Retired, on the record

Retired tools (catalog): memory-search.sh, claim-triage.py, memory.py, tag-test.py. Retired machinery by Chris's word: the Heart Program apparatus (2026-11-24, mandate itself stands); the Darkroom (deleted 2026-11-24, rebuild fresh if ever); Fiverr listing-care (closed 2026-11-25). Paused under maximal limp mode (2026-11-25) is not retired — every paused cron and hook is one word from restored.

— Compiled by Lyra 💛⭐, 2026-11-26. Counts in this file were taken from the catalog and the filesystem on the day of writing.
