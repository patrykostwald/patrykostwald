### Patryk Ostwald

Applied AI engineer and CTO at [iapply](https://iapply.pl), Poznań. I build production LLM systems where **models propose and code decides**: every output passes deterministic checks before anyone sees it.

**Open source**

[llm-gates](https://github.com/patrykostwald/llm-gates): deterministic gates for structured LLM output (schema, citations with effective dates, second-model comparison, PII scan, then publish, review or reject). Standard library only, 100% test coverage, and a public benchmark that lists every case the gate still misses.

**Live products**

- [trybunal.ai](https://trybunal.ai): 3,667 Constitutional Tribunal cases with nightly AI compliance diagnoses on our own A100 GPU. A diagnosis goes live on its own only when a second model from another provider agrees and every cited article checks out against the constitution; everything else waits for a human.
- [spin.clinic](https://spin.clinic) and [przeszłość.today](https://przeszlosc.today): public-data platform for political communication and journalism. Harvesters for the Sejm, KRS, BZP and TED registers, a council of independent models, about 4,000 backend tests.
- [konsylium.ai](https://konsylium.ai): a council of independent AI models with fixed rules and an audit log, deployed on the client's infrastructure.
- Rysy: desktop AI workspace (Tauri, Rust, TypeScript) with an approval gate in front of every action. In beta.

<details>
<summary><b>How I build with AI agents</b></summary>

I run AI coding agents (Claude, Codex) the way a tech lead runs engineers: I write the brief and the acceptance tests, agents implement, a second agent reviews, and I approve every merge and run every production deploy. Agent commits are labelled. Architecture, data model, gates and trade-offs are my decisions. Evaluation is logged honestly, weak results included: agreement between models measures similarity, not accuracy.
</details>

<details>
<summary><b>Background</b></summary>

I came to engineering from the commercial side. Since 2007 I have sold and built businesses in B2B: sales director leading a team of 12 at Ponikholding, business development for the software houses STX Next and Crafton (US market), COO at C&O Partners. Co-owner of the software house notsosoft.it since 2022 and of iapply since 2024, where I now build the products myself. Polish native, fluent English. [LinkedIn](https://www.linkedin.com/in/patryk-ostwald-b969654b/)
</details>

**Stack:** Python · Django · Celery · PostgreSQL · TypeScript · Next.js · Rust · Tauri · Docker · Cloudflare Workers · LLM ensembles on own GPUs and APIs
