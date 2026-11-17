### Patryk Ostwald

CTO at [iapply](https://iapply.pl), Poznań. I build products on top of public data and AI, where every model output is checked by deterministic rules before anyone sees it.

**Background**

I came to engineering from the commercial side. Since 2007 I have sold and built businesses in B2B: sales director leading a team of 12 at Ponikholding (2022 to 2023), business development for the software houses STX Next and Crafton (US market), COO at C&O Partners. Co-owner of the software house notsosoft.it since 2022 and of iapply since 2024, where I now build the products myself. That mix shapes how I engineer: scope with the customer in mind, ship fast, measure what matters. Polish native, fluent English. [LinkedIn](https://www.linkedin.com/in/patryk-ostwald-b969654b/)

**Products**

| | |
|---|---|
| [spin.clinic](https://spin.clinic) | Shows how political messages are built: persuasion techniques in politicians' posts, with every claim checked against sources. Same yardstick for everyone. |
| [przeszłość.today](https://przeszlosc.today) | Public figures on one timeline: statements, Sejm votes, KRS companies and public money, each link backed by a source. |
| [trybunal.ai](https://trybunal.ai) | All 3,600+ cases of Poland's Constitutional Tribunal, the backlog year by year, and AI diagnoses of constitutional compliance, published daily. |
| [konsylium.ai](https://konsylium.ai) | A council of independent AI models that reviews each result under fixed rules, deployed on the client's own infrastructure. |
| Rysy | Desktop AI workspace (Tauri, Rust, TypeScript): agents, mail and social in one place, with an approval gate in front of every action. In beta. |
| [zbudujmi.com](https://zbudujmi.com) | Websites, shops and apps with a clickable preview before payment and a fixed price. |

**In numbers**

- trybunal.ai: 3,667 Constitutional Tribunal cases catalogued; new AI diagnoses generated every night on our own A100 GPU and published only after code gates pass (PII scan, citation sanity, completeness, duplicates); when a second model from another provider disagrees, the case is marked as contested on the page.
- spin.clinic and przeszłość.today: dozens of public-data harvesters (KRS, Sejm, BZP, TED), about 4,000 backend tests, CI green on every merge.
- trybunal.ai: 436 tests, offline by default. Rysy: about 650 commits to a desktop beta with a security review before each release.

**How I build with AI agents**

I run a small team of AI coding agents (Claude, Codex) the way a tech lead runs engineers: I write the brief and the acceptance tests, agents implement, a second agent reviews, and I approve every merge and run every production deploy myself. Commits co-authored by agents are labelled as such. Architecture, data model, gates and trade-offs are my decisions.

**How I work**

- Models propose, code decides: structured outputs, citation checks and comparators between independent models.
- Small, tested increments with CI on every merge. Evaluation logged honestly, including weak results: agreement between models measures similarity, not accuracy.
- Engineering with agent teams: specialised AI agents build and review, a human owns the gate and every production deploy.
- Privacy by design: public figures and public data only, GDPR and the EU AI Act considered from day one.

**Stack**

Python · Django · Celery · PostgreSQL · TypeScript · Next.js · Rust · Tauri · Cloudflare Workers · Docker · LLM ensembles on own GPUs (A100) and APIs
