# AGENTS.md — rules for working in this repo (read first)

This repo is used as the **persistent memory across arena.ai chat sessions**.
The human often cannot reliably say when a session is over ("Continue" on the
platform is flaky), so nothing may depend on an end-of-session trigger.

## Standing instruction — mandatory, no reminder needed

Every session, every turn with new information:

1. **Start of session:** read `README.md` (section „Aktueller Stand") and
   `docs/00_Sitzungsspiegel.md`. Continue from there.
2. **Maintain the mirror continuously, not at session end:**
   - append a dated entry to the **Verlauf** section of
     `docs/00_Sitzungsspiegel.md` for every substantive exchange,
   - keep „Aktueller Stand", „Offene Punkte / wartet auf dich" and
     „Nächste Schritte" up to date,
   - record measurements, decisions, numbers and open questions there.
3. When a topic is settled, it may graduate into a thematic `docs/*.md` file —
   the mirror then links to it.
4. **Commit + push after meaningful updates** (same branch), so the next session
   always finds the freshest state — even if this one dies mid-conversation.
5. Work in the repo's language: German for content/docs, unless the user writes
   English.

This is business as usual. Do not wait to be asked.
