# Independent audit — 2026-10-23

**Method.** An auditor who did not build the system re-verified 13 claims against the live systems — the test suite, the production database, the registries, the files, the job schedules, and the project's own memory records — read-only.

## Confirmed (12)

- Full test suite green: 471 tests.
- Production database shape: 27 tables, migrations 0001–0008.
- Mission registration byte-identical to the published text.
- 7 registered grading instruments; the operator-confidence instrument at v2 and gradeable.
- Auto-adoption armed, with zero live proposals and no silent drift.
- Scoreboard and mission figures: revenue $0, cost coverage 0.000 against a $180/mo running cost, owner-time ledger opened.
- Nightly proof green and watchdog healthy, with a fresh backup.
- The Oracle's new VOICE class honestly answering UNKNOWN on an empty customer-voice ledger.
- The phantom-claim registry: 5 claims, 4 confirmed, 1 refuted — the refuted one being a false "first subscriber" alert the system caught and retracted the same morning.
- The synthetic-twin rehearsal results file: all checks passed.
- Documentation set complete.
- All seven scheduled jobs intact.
- The project's written records consistent with live state.

## The one discrepancy (1)

A wording imprecision in the operator's own report to the owner: the auto-adoption envelope's registered hash is computed over the envelope's canonical contents — any change to a value is caught — not over the raw file bytes, as the report implied. The mission artifact, by contrast, is hashed byte-for-byte. The underlying gates were verified sound. The convention is now documented in the recovery notes — we publish the discrepancy because catching exactly this class of imprecision is the point of the system.
