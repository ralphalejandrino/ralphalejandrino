## Ralph Alejandrino

I build and operate Django systems for small businesses, and I am usually also the person
who deploys them, gets the call when they break, and finds out what actually happened.

**Locus** — multi-tenant CRM and delivery tracking for an LPG distribution business.
Django, delivered as a frozen Windows binary so it runs unattended on the client's own
machine. A language model parses free-text customer messages into order *drafts* that a
human approves before any stock moves. 2,800 customer records, 139,000 messages, in daily
production use.

**Tabula** — point of sale, inventory and cost of goods, running on the register a café
takes money with. Offline-capable PWA with a versioned service worker, ~2,000 automated
tests, and a deploy process that snapshots the database and records a rollback commit
before every push.

Both are client systems, so the source is not public. What I can share is the writing:

- **[Engineering case notes](https://ralphalejandrino.github.io/)** — five production
  incidents where the tooling reported success and was wrong, what hid each one, and the
  check that caught it.
- **[CV](https://ralphalejandrino.github.io/cv/)**

### How I work

I use AI assistants throughout and treat their output as draft work. Three habits make
that safe rather than fast and sorry:

- **Prove the test can fail.** After a fix passes, remove the fix and confirm the test
  goes red. A green test that was never shown to fail is decoration.
- **Run a negative control.** Every change gets a case that must *not* change.
  Deduplication is only correct if a genuine repeat still gets through.
- **Verify against the code, not the summary.** Migrations, fields, versions and line
  numbers get checked in the repository before they shape a decision. I learned that one
  expensively.

Python · Django · Django REST Framework · SQLite and PostgreSQL · progressive web apps ·
LLM integration · Linux · Baguio, Philippines · UTC+8

Reachable at ralphmiguelalejandrino@gmail.com

<!-- profile -->
