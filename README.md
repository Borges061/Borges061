**Software Developer — Back-end & Full Stack**
Brasília, Brazil
---

## Experience

**Sicoob** — Software Developer Intern
*1 year and 5 months*

- Developed and maintained internal applications in a corporate financial-sector environment.
- Wrote automated tests following Test-Driven Development as part of the daily workflow.
- Worked with continuous integration and delivery pipelines covering build, testing and deployment.
- Collaborated within an engineering team under code review and versioning standards.

  **Puma** — Scrum Master
*2 years* · [Repository](https://github.com/yourusername/puma)

- Led the Scrum cycle: sprint planning, daily stand-ups, sprint reviews and retrospectives.
- Worked with the Product Owner to refine and prioritize the product backlog.
- Removed impediments and protected the team's focus during each sprint.
- Tracked delivery with sprint metrics such as velocity and burndown, using them to improve planning.

---

## Selected Work

### GuildHall

A multi-server Discord bot and web dashboard for managing Albion Online guilds: verified member registration through the game's public API, event sign-ups and attendance, a points ledger, fines, guild finances and weekly and monthly rankings.

- **Architecture:** business rules live in a service layer independent of Discord and shared by the bot and the web dashboard. The dashboard never writes to Discord directly; it queues requests in the database and the bot executes them within seconds, so the bot token never leaves the server.
- **Data integrity:** financial records and points are an append-only ledger. Nothing is deleted; mistakes are corrected through audited reversals. Currency is stored as integers, and dates are stored in UTC and shown in each guild's time zone.
- **Access control:** role-based permissions (Admin, Treasurer, Caller and custom roles) enforced on both the bot and the dashboard, with a full action history.
- **Integrations:** Albion Online public API across three regions, Albion Data Project market prices, killfeed and loot log imports.
- **Deployment:** one-command installer for a VPS with Docker, PostgreSQL and automatic HTTPS (Caddy and Let's Encrypt), versioned migrations and daily backups. The test suite runs against both SQLite and PostgreSQL.
- **Migration:** replaced two legacy bots, fixing an exposed token, commands that destroyed data and missing per-server isolation, with an import script for existing records.

**Stack:** Python, FastAPI, HTMX, PostgreSQL, Alembic, Docker, Caddy, pytest · [Webpage](https://painel.guildbot.org)

### Fonseca & Cavalcanti Advogados

Website for a law firm specializing in digital fraud cases. Presents the firm's practice areas and credentials and captures leads through a structured contact form and direct WhatsApp, phone and email channels.

**Stack:** HTML, CSS, JavaScript · Netlify · [Live](https://fonsecavalcanti.netlify.app)

### Roberto Pimenta — Event Barbecue Catering

Website for a professional barbecue chef serving weddings, corporate events and restaurants. Showcases services and past events and includes a quick event briefing form that sends the request directly to WhatsApp.

**Stack:** HTML, CSS, JavaScript · Netlify · [Live](https://robertopimenta.netlify.app)

---

## Technical Skills

| Area | Tools |
| --- | --- |
| Languages | Python, JavaScript, Java, C++ |
| Back-end | Node.js, FastAPI |
| Front-end | HTML, CSS, Tailwind CSS, HTMX |
| Databases | PostgreSQL, MongoDB, SQLite |
| Infrastructure | Docker, Linux VPS, Caddy, Netlify |
| Quality & Delivery | TDD, pytest, CI/CD, database migrations |
| Methodologies | Scrum, Agile |

---

## How I Work

**Tests first.** Every feature starts with a test that defines the expected behavior. This makes refactoring safe and keeps the code self-documenting.

**Data is never silently lost.** Records are corrected, not deleted. Every change is traceable, money is never stored as floating point, and time is always stored in UTC.

**Automated delivery.** Every change goes through automated build and test steps before reaching production. Deployments, migrations and backups are scripted, not manual.

---

## Contact

[luisguilhermebm91@gmail.com](mailto:luisguilhermebm91@gmail.com)
