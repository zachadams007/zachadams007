# Zachary Adams

Mathematics and Engineering at Queen's University, Systems and Robotics sub-stream. First year complete with a 4.20 cumulative GPA, entering second year. Expected graduation April 2030.

Writes C. Builds in TypeScript, Rust and Python by directing AI coding agents, with deterministic code and tests checking what they produce.

[LinkedIn](https://www.linkedin.com/in/zachary-adams-239894386/)

## Main projects

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/zachadams007/catalyzed-alpha-platform"><img src="images/catalyzed-alpha.png" alt="Catalyzed Alpha market map"></a>
<h3><a href="https://github.com/zachadams007/catalyzed-alpha-platform">Catalyzed Alpha</a></h3>
<p>Equity research platform. A daily pipeline narrows about 21,000 US listings to 500, scores them on 13 dimensions and ranks them with a deterministic engine. Language models collect evidence and the engine computes every score.</p>
<p>127,648 lines of TypeScript, 1,877 tests, 26 Postgres tables.<br><a href="https://catalyzed-alpha.vercel.app">Live site</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/zachadams007/praxis-desktop"><img src="images/praxis-brain.jpg" alt="Praxis brain window, a 3D graph of projects and agents"></a>
<h3><a href="https://github.com/zachadams007/praxis-desktop">Praxis</a></h3>
<p>Windows desktop environment that orchestrates coding agents. Reads live Claude Code, Codex and Cursor sessions, runs headless agents in parallel lanes, verifies each lane on exit, and is driven by voice.</p>
<p>48,429 lines of Rust, 67,645 of TypeScript, 418 Rust unit tests.<br>Tauri, React, Three.js</p>
</td>
</tr>
</table>

| Project | Summary |
|---|---|
| [AI Development Workflow](https://github.com/zachadams007/ai-development-workflow) | Operating setup for coding agents: rules injected on every turn, memory that new sessions rebuild from, ten skills, and a snapshot that refuses to commit a credential |
| [Earnings Print Detector](https://github.com/zachadams007/earnings-print-indicator) | TradingView indicator in Pine Script v6 that finds the candle where a market starts reacting to earnings, Python tools that read the SEC filing, and a scalping research package that checks its signals against shuffled data |
| [3D Print Quoting Site](https://github.com/zachadams007/3d-print-quoting) | Storefront that prices an STL or 3MF in the browser from its true solid volume. Next.js, 22 API route files, 10 tables. [Live site](https://3d-print-site-ten.vercel.app/) |

## Code worth opening

| Problem | File |
|---|---|
| A published ranking that any visitor could have overwritten, and the migration that closed it | [`0013_daily_signals_trusted_writer.sql`](https://github.com/zachadams007/catalyzed-alpha-platform/blob/main/supabase/migrations/0013_daily_signals_trusted_writer.sql) |
| Cross-sectional ranking of the day's universe in one module | [`normalizeUniverse.ts`](https://github.com/zachadams007/catalyzed-alpha-platform/blob/main/src/engine/normalizeUniverse.ts) |
| A watchdog that tells a silent webview from a crashed one | [`lib.rs`](https://github.com/zachadams007/praxis-desktop/blob/main/src-tauri/src/lib.rs#L1031) |
| A process registry that survives PID reuse | [`flightdeck.rs`](https://github.com/zachadams007/praxis-desktop/blob/main/src-tauri/src/flightdeck.rs#L5591) |
| A shuffled-bars control test that passed because it had tested nothing | [`controls.py`](https://github.com/zachadams007/earnings-print-indicator/blob/main/scalping/src/bot/scalp/controls.py) |
| Six credential patterns checked before anything is staged | [`snapshot.py`](https://github.com/zachadams007/ai-development-workflow/blob/main/versioning/snapshot.py) |

## Data engineering

The [Catalyzed Alpha data model](https://github.com/zachadams007/catalyzed-alpha-platform/blob/main/docs/data-model.md) covers 26 Postgres tables with row-level security and 28 migrations. The [daily scan](https://github.com/zachadams007/catalyzed-alpha-platform/tree/main/scripts/universe_scan) and the [point-in-time replay harness](https://github.com/zachadams007/catalyzed-alpha-platform/tree/main/scripts/backtest) are the pipeline.

## Working method

Agents write most of the code, under written rules. In Catalyzed Alpha the ranking engine owns the score; in Praxis a lane's verify command outranks its exit code. A failure that gets through becomes a written rule, often with a test. [AI Development Workflow](https://github.com/zachadams007/ai-development-workflow) holds the rules.

## Robotics and hardware

- MARC, the Moon Autonomous Rover for Cargo, a Canadian Space Agency client project. Team lead, with work on servo control and camera-guided autonomous pickup.
- A scratch-built RC airplane with CAD.
