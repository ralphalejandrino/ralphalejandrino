## Hi, I'm Ralph

I build Django systems for small businesses, and I'm also the one who deploys them, picks up the
call when something breaks, and digs in until I know what actually happened.

**Locus** is a multi-tenant CRM with delivery tracking, built for an LPG distribution business.
It ships as a Windows desktop app, so it runs unattended on the client's own machine. A language
model reads free-text customer messages and turns them into order *drafts*, and a person approves
each one before any stock moves. It has been tested on that business's real data: 2,800 customer records and 139,000
messages. Source: **[ProjectCRM](https://github.com/ralphalejandrino/ProjectCRM)**.

**Tabula** is a point-of-sale, inventory and cost-of-goods system that runs on the register a café
takes payments with. It's an offline-capable web app with a versioned service worker and 670+
automated tests. Before every release, the deploy process snapshots the database and records the
commit to roll back to. Source: **[ProjectPOS](https://github.com/ralphalejandrino/ProjectPOS)**.

Both repositories are public, with every client name, number and address replaced by invented
ones. Also worth a look:

- **[Engineering case notes](https://ralphalejandrino.github.io/)**: five production incidents
  where the tooling said everything was fine when it wasn't, what hid each problem, and the check
  that caught it.
- **[How I work with AI agents](https://ralphalejandrino.github.io/agents/)**: the Claude Code
  agent I run my engineering through, with four real sessions you can step through.
- **[CV](https://ralphalejandrino.github.io/cv/)**

### How I work

I use AI tools throughout my work, and I treat what they produce as a first draft. Three habits
keep that safe:

- **I make sure a test can fail.** Once a fix passes, I remove it and check that the test goes
  red. A test I've never seen fail doesn't prove anything.
- **I run a negative control.** Every change gets a case that must *not* change. Deduplication
  only works if a genuine repeat order still goes through.
- **I check the code, not the summary.** Migrations, fields, versions and line numbers get
  confirmed in the repository before I act on them. I learned that one the hard way.

Python · Django · Django REST Framework · SQLite and PostgreSQL · progressive web apps · LLM
integration · Linux

Baguio, Philippines (UTC+8) · ralphmiguelalejandrino@gmail.com
