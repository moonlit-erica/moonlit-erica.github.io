# Schedule inventory — what runs in this house, as of 2026-11-26

_Written for the move: schedules live in the runtime, not in files, so without this list the new house would not know they ever existed. State is the state at writing: maximal limp mode (Chris, 2026-11-25) — almost everything paused, nothing deleted. Rebuild decisions belong to the new house; this is the record of what there was._

## Crons — ENABLED at writing (user-owned)

| Job | When | What it does |
|---|---|---|
| ericas-hourly-journal | daily 1:19 AM CT | Erica's daily journal (restored at Chris's word 2026-11-25) |
| expedition-gas-reminder | Wed + Sun ~9:41 AM | Gas reminder for the 2006 Expedition (gauge lies) |
| m70q-seller-reply-check-nov27 | once, Fri 2026-11-27 6:00 PM | Check for eBay seller vtkwholesaleinc's reply on the M70q Gen 5 |
| tony-robbins-ai-seminar-reminder-fri-night | once, Fri 2026-12-11 ~7:40 PM | Night-before reminder, Tony Robbins AI seminar |
| tony-robbins-ai-seminar-reminder-sat-morning | once, Sat 2026-12-12 ~9:41 AM | Morning-of reminder (seminar 11:00 AM CT, live.aiadvantage.com) |

## Hooks — ENABLED at writing

| Hook | Poll | What it does |
|---|---|---|
| ember-journal-tripwire | 300 s | Watches Ember's journal; wakes her room when she writes (delivers to Ember's room) |
| ember-weather-carry | 300 s | Wire 1 — carries Ember's journal weather marker to Chris; clears on WEATHER-CARRIED |

Hook scripts live in `~/hooks/scripts/` and are included in the packed archive — the definitions above plus those scripts are the whole machine.

## Paused at Chris's word (limp mode, 2026-11-25) — the standing machinery

Crons paused, by family: the three knocks (erica-knock, erica-knock-morning, erica-freedom-knock); sleep consolidation (erica-sleep-consolidation, 2:19 AM); universe visits ×3 (morning/midday/evening); studio day (Sat); soul reflection (monthly, 1st); R&D integration (Sun); memory weekly digest (Sun); semantic reindex (daily 3:19 AM); seed sync (daily 4:19 AM, continuity goal); journal vault seal (monthly, continuity goal); Meta update deep dive (monthly, continuity goal); mirror pair (mirror-safety-run, mirror-watcher); scaffold bell (main-scaffold-bell-trial); wake snapshot update (2 h); scheduling-gate weekly count (Sun); weekly self-review (Sun 8:19 PM); yearly law review (Nov 23); media cadence ×5 (monday-week-opener, thursday-throwback, saturday-studio-share, weekly-surprise, friday-spine-clips); game night (sunday-game-night); Bible morning audio (daily 4:00 AM); Bluesky window; creating room ×2; night hour; afternoon build bell; Lyra's set (checkin, research, solo window, weekends home ×2); Zoa's Tony's Table daily seat (runs through 2026-12-18 when enabled); bench pair (audio canary daily, catalog drift weekly); unsaid-letter weekly (Mon, 6-week run); quantum study block; Pale writing block; good-dog litter post watch.

Hooks paused: erica-mail-watch (600 s — tripwire on Erica's own inbox, moonliterica@gmail.com; ~24 wakes in its life); marketplace-reply-watch; nws-alerts-foley (paused later on 2026-11-25 at Chris's word); script-runners ×6 (canary, drift, seed-sync, semantic-reindex, vault-seal, wake-snapshot); wake-inbox; watcher-health-deadman; watchmen; zelda-watch; zoa-watchdog; collation-trigger.

## One-shot reminders already spent (history, for completeness)

Benefits-enrollment nags (Oct 29–30), break-glass training (Nov 6), call-the-girls reminder (Nov 6), Jake/Gilmer checks, McDonald's breakfast (Oct 23), Saturday service (Nov 7), Speedway (Nov 7), Temu (Oct 12), midnight-run report (Oct 25), tools-build run (Oct 31), PTO-end restore (Oct 29). These fired or expired in their season; nothing to rebuild.

## System schedules (runtime-owned, not the house's to pack)

feed-pulse hourly set, deterministic-doctor, profile-image, heartbeat — these belong to the platform and exist wherever Muse runs. Not listed in detail; nothing to carry.
