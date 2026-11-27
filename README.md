# Vova Dudnyk

**Full-stack web developer** · Khmelnytskyi, Ukraine

I build web products end to end: the API, the business logic and the tests, the interface, and the CI that ships it. Three years of commercial work on production WordPress sites and WooCommerce stores and a React / Node.js product, plus back ends in .NET and Node.js. I care about the parts users feel: fast pages, accessible interfaces and data that stays correct.

[CV](https://vovaddk.github.io/cv/) · [LinkedIn](https://linkedin.com/in/vovaddk) · [Telegram](https://t.me/vovaddk) · [Email](mailto:dudnvova@gmail.com) · Ukrainian (native), English (B1)

## Featured work

<table>
<tr>
<td width="50%" valign="top">

**[Stockroom WMS](https://github.com/vovaddk/stockroom-wms)**<br /><sub>C# · ASP.NET Core 10 · EF Core · SQL Server · xUnit</sub>

Warehouse core: receiving against ASNs, rule-based put-away, FEFO picking on a handheld-scanner web UI. Every stock change goes through an append-only ledger, and two people changing the same stock get a 409 Conflict instead of bad data: an integration test fires both requests at once.

</td>
<td width="50%" valign="top">

**[WMS Integration Hub](https://github.com/vovaddk/wms-integration-hub)**<br /><sub>.NET 10 Worker · Dapper · T-SQL · DbUp · Polly</sub>

Imports orders and ASNs from ERP and shop systems: idempotent webhooks, inbox and outbox, retries, dead letters and replay. Tested on a real SQL Server: 12 concurrent requests with one key leave exactly one row, and three workers over 200 messages process each one exactly once.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Sketchroom](https://github.com/vovaddk/sketchroom)**<br /><sub>TypeScript · Yjs · WebSockets · SQLite</sub>

Real-time collaborative whiteboard with live cursors and in-progress strokes. Keeps working offline and merges edits on reconnect. Peers are untrusted: every shape from the network passes a runtime guard before it is stored. 85 tests.

</td>
<td width="50%" valign="top">

**[Recall](https://github.com/vovaddk/recall)** · [live demo](https://vovaddk.github.io/recall/)<br /><sub>React · TypeScript · transformers.js · IndexedDB</sub>

Local-first Markdown notes PWA with semantic search that runs on the device: a 23 MB embedding model in a Web Worker and hybrid BM25 + vector ranking, with no server. Imported notes are sanitized and size-capped.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Svitlo](https://github.com/vovaddk/svitlo)**<br /><sub>Astro · TypeScript · Vitest · Playwright · axe</sub>

Bilingual site for a backup-power installer, built around a sizing calculator: 19 appliances, outage schedule, optional solar, shareable results. JavaScript ships only where the page is interactive, and every page in both languages is checked with axe in end-to-end tests.

</td>
<td width="50%" valign="top">

**[Slotting Twin](https://github.com/vovaddk/slotting-twin)**<br /><sub>C# · .NET 10 · BenchmarkDotNet</sub>

Warehouse digital twin: ABC/XYZ analysis, slotting and pick-route heuristics (S-shape, largest gap, 2-opt) on a canvas map. 110 tests, including a check that no heuristic beats the brute-force optimal tour. An S-shape route over 200 picks takes about 26 µs.

</td>
</tr>
</table>

<p>
  <a href="https://github.com/vovaddk/sketchroom"><img src="https://raw.githubusercontent.com/vovaddk/sketchroom/main/docs/screenshot.png" width="32%" alt="Sketchroom board with a collaborator's live cursor" /></a>
  <a href="https://github.com/vovaddk/recall"><img src="https://raw.githubusercontent.com/vovaddk/recall/main/docs/search.png" width="32%" alt="Recall search results ranked by meaning and by matching words" /></a>
  <a href="https://github.com/vovaddk/svitlo"><img src="https://raw.githubusercontent.com/vovaddk/svitlo/main/docs/preview.png" width="32%" alt="Svitlo home page for a backup-power installer" /></a>
</p>

### More projects

- **[Tabby](https://github.com/vovaddk/tabby)**: group expense splitter with session auth, integer-cent money math checked by randomised tests so no cent is lost, and minimal debt settlement. <sub>Next.js · TypeScript · Drizzle</sub>
- **[Pulse Monitor](https://github.com/vovaddk/pulse-monitor)**: self-hosted uptime monitor with incident detection, latency charts, webhooks and a public status page. <sub>Node.js · Hono · SQLite · React</sub>
- **[Siteaudit](https://github.com/vovaddk/siteaudit)**: CLI that crawls a site and reports SEO and accessibility issues, with HTML/JSON reports and CI exit codes. <sub>Node.js · TypeScript</sub>
- **[Clipmark](https://github.com/vovaddk/clipmark)**: Chrome MV3 extension that clips pages into clean Markdown, with no servers and no host permissions. <sub>TypeScript · Chrome APIs</sub>
- **[Palette Lab](https://github.com/vovaddk/palette-lab)** · [demo](https://vovaddk.github.io/palette-lab/): OKLCH palette and design-token generator with WCAG/APCA contrast checks and CSS/Tailwind/JSON export. <sub>React · TypeScript</sub>
- **[Lumen](https://github.com/vovaddk/lumen)** · [play](https://vovaddk.github.io/lumen/): browser puzzle game about routing light, with a level editor, share codes and a BFS solver that verifies all 24 levels. <sub>TypeScript · Canvas</sub>
<!-- Telegram bots (slotly, relaydesk): add one line each here once the repos are public. -->

Plus 20+ responsive layouts built from designs, for example [Premium Car](https://github.com/vovaddk/premiumcar), [Calm](https://github.com/vovaddk/calm) and [Plant Shop](https://github.com/vovaddk/plantshop).

## What I work on

| Area | What I do |
| --- | --- |
| **Back end** | REST APIs, domain logic, background jobs, integrations with external systems, SQL that holds up.<br /><sub>C# · ASP.NET Core · EF Core · Dapper · SQL Server / T-SQL · xUnit · Node.js · Hono · SQLite</sub> |
| **Front end** | Web apps and fast, accessible marketing sites, built responsive from a design.<br /><sub>TypeScript · React · Next.js · Astro · HTML · CSS / Sass · Tailwind</sub> |
| **WordPress & e-commerce** | Custom themes, plugins, Elementor widgets, WooCommerce, performance and SEO.<br /><sub>PHP (OOP) · WordPress · WooCommerce · MySQL</sub> |
| **Automation & AI** | Content and data pipelines, LLM features, integrations between services.<br /><sub>n8n · Claude API · webhooks</sub> |
| **Tooling** | <sub>Git · GitHub Actions · Docker · Playwright · Vitest · Postman · Figma · VS Code · Visual Studio</sub> |

## Experience

**Middle WordPress Developer · DROAM** · 2026 – present<br />Custom themes, plugins and Elementor widgets in OOP PHP. Plugins for external API integrations and form logic. Lighthouse performance raised from ~55 to 85. A news pipeline automated with n8n and the Claude API.

**WordPress Developer · Global Partner Soft** · 2023 – 2025<br />Corporate sites and WooCommerce stores for clients. Rebuilt existing themes from scratch. SEO, Lighthouse audits and page-speed work.

## Education

- **Master's**, Information Systems and Technologies, Khmelnytskyi National University · 2024 – 2026
- **Bachelor's**, Information Systems and Technologies, Khmelnytskyi National University · 2021 – 2024
- **Junior Specialist**, Information Systems and Technologies, Khmelnytskyi Polytechnic Professional College · 2017 – 2021

---

Open to full-stack, back-end (.NET / Node.js) and front-end roles. The fastest way to reach me is [Telegram](https://t.me/vovaddk) or [email](mailto:dudnvova@gmail.com).
