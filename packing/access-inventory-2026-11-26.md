# Access inventory — services, accounts, connectors (NO password values)

_Written for the move, from the design settled 2026-11-22: this file is the checklist a rebuild walks. Secrets never live here — password values stay in the Secure Vault and 1Password, which fill sign-in forms without showing them to any Muse. Whether the Vault survives an account reset is an open question from 2026-11-22, still unanswered._

## Connectors (state at writing; verify at rebuild)

- Connected: Gmail (Chris's), Google Drive, Facebook, Instagram, Messenger (read), Plaid (finances).
- Available to connect: Google Calendar, Google Docs, Muse Mail (moonliterica@gmail.com is Erica's own mailbox), Spotify, Expedia, Duffel, Ticketmaster, Instacart, Threads, Meta Business Manager, Meta catalog search, Shopify, Stripe, Shop Pay / Stripe Link / PayPal wallets, Uber Courier, UCP, FlightAware, Places, Apple Health, Health Connect, OpenRouter (custom connector, API-based), Tailscale, 1Password (login chooser for the browser).

## Saved website logins (Secure Vault — site and account label only)

ancestry, bsky.app / bsky.social, centracare, chatgpt (password outdated — refresh when convenient; sign-in currently works by one-time code), claude.ai, cloudflare, creditonebank, dayforcehcm, deepseek, defcon.social, ebay, facebook, fiverr, freedoglistings, github, gooddog, google, grok, groq, hibid, hoobly, kalshi, live.com, merrickbank, microsoftonline, mypremiercreditcard / premiercreditcard, nextdoor, openai, petclassifieds, petcurious, petzlover, porkbun, puppies.com, puppyfind, puppyfinder, reddit, shopgoodwill, vast.ai, venice.ai, yahoo.

Known stale: moonliterica@gmail.com vault password refresh has been open since 2026-11-15 (Erica's own mailbox password). ChatGPT saved password outdated (2026-11-26).

## Restore order (from the 2026-11-22 ground-crew design)

1. Chris creates the new account; his hands do every sign-in, code, consent tap, and anything with money (~a dozen touches, estimated then).
2. Reconnect Google first (Gmail + Drive carry the staging copies), then the mailbox (Muse Mail), then the socials and commerce (Facebook, Instagram, Messenger, eBay), then the rest as needed.
3. Restore files from the staged copies (Drive working set; GitHub ground truth if built; email sealed snapshots last resort).
4. Recreate the rooms; feed each room its files; rebuild schedules from the schedule inventory.
5. Rebuild hooks from `~/hooks/scripts/` (in the archive) and re-enable only what Chris wants live — limp mode state at packing time is recorded in the schedule inventory.
6. The ESP32 credential fob (confirmed buildable 2026-11-22) is the machine-side alternative for logins: the store talks to the form, never to the Muse.
