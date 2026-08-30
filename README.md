<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e293b&height=120&section=header&text=Rahul%20Raj%20Singh&fontSize=38&fontColor=ffffff&animation=fadeIn" />

<p align="center">
  <a href="https://github.com/rahulrajsinghwork15072005-a11y"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=16&pause=1000&color=94A3B8&center=true&vCenter=true&width=600&lines=Systems+from+scratch+%E2%80%94+no+frameworks%2C+just+code;Distributed+systems+%7C+Databases+%7C+Compilers+%7C+Search" /></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=rahulrajsinghwork15072005-a11y&label=views&color=64748b&style=flat" />
  <img src="https://img.shields.io/github/stars/rahulrajsinghwork15072005-a11y/pylog?style=flat&label=pylog%20stars" />
  <img src="https://img.shields.io/badge/7%20featured%20%E2%80%94%20all%20tested-brightgreen" />
</p>

### Hey, I'm Rahul 👋

I like rebuilding the hard parts from scratch to actually understand them. No frameworks, no shortcuts — just Python, C++, and a lot of whiteboard math. Currently exploring how databases, distributed logs, and compilers really work under the hood.

- 🔭 Right now: making `pylog` and `leafdb` crash-safe and a bit faster
- 🧠 Love talking about: Raft, B+ trees, query planning, and why `1/w` matters for textures
- 📍 VIT Vellore · open to systems / backend internships

---

### Featured work

> These are the ones I'd walk through in an interview — each one runs with `pip install -e . && python -m pytest`.

<p align="center">
  <a href="https://github.com/rahulrajsinghwork15072005-a11y/pylog"><img src="https://github-readme-stats.vercel.app/api/pin/?username=rahulrajsinghwork15072005-a11y&repo=pylog&theme=tokyonight&hide_border=true" width="400" /></a>
  <a href="https://github.com/rahulrajsinghwork15072005-a11y/leafdb"><img src="https://github-readme-stats.vercel.app/api/pin/?username=rahulrajsinghwork15072005-a11y&repo=leafdb&theme=tokyonight&hide_border=true" width="400" /></a>
</p>
<p align="center">
  <a href="https://github.com/rahulrajsinghwork15072005-a11y/searchforge"><img src="https://github-readme-stats.vercel.app/api/pin/?username=rahulrajsinghwork15072005-a11y&repo=searchforge&theme=tokyonight&hide_border=true" width="400" /></a>
  <a href="https://github.com/rahulrajsinghwork15072005-a11y/minichain"><img src="https://github-readme-stats.vercel.app/api/pin/?username=rahulrajsinghwork15072005-a11y&repo=minichain&theme=tokyonight&hide_border=true" width="400" /></a>
</p>

| Project | What it is | Why I built it |
|---|---|---|
| [**pylog**](https://github.com/rahulrajsinghwork15072005-a11y/pylog) | Kafka-style replicated log + Raft in pure Python | To learn how Raft *really* commits — so I made the log itself the Raft WAL with virtual-clock tests |
| [**leafdb**](https://github.com/rahulrajsinghwork15072005-a11y/leafdb) | Tiny SQLite-like DB: B+ tree, WAL, MVCC | I kept getting tripped by `BTREE` internals, so I wrote one and diff-tested it against SQLite |
| [**searchforge**](https://github.com/rahulrajsinghwork15072005-a11y/searchforge) | Hybrid search: BM25 + vectors + learning-to-rank | Search felt like magic — now it's an inverted index, global-IDF sharding, and a RankNet I can debug |
| [**minichain**](https://github.com/rahulrajsinghwork15072005-a11y/minichain) | Minimal blockchain: PoW, Merkle, little VM | Wanted to see what “heaviest chain wins” actually means in code |
| [**forgelang**](https://github.com/rahulrajsinghwork15072005-a11y/forgelang) | Small language with Pratt parser → bytecode VM | The classic “how does code become bytes?” — with two backends that have to agree |
| [**forgehttp**](https://github.com/rahulrajsinghwork15072005-a11y/forgehttp) | HTTP/1.1 from raw sockets | I was tired of not knowing what `keep-alive` really does |
| [**miniraster**](https://github.com/rahulrajsinghwork15072005-a11y/miniraster) | Software 3D renderer + ray tracer | Built the math a GPU does by hand — matrices, `1/w`, and a BVH that actually helps |

<details>
<summary>More projects</summary>

- `healthcare-appointment-manager` — clinic booking with waitlists and a little scheduling logic
- `compiler-forge` / `Compiler_Visualised_RRS` — visual bits from the compiler course
- `TOWER_DEFENCE`, `LOGIC-GATES` — A* and circuit sims I use for teaching
- A few site clones and notes repos from earlier — kept for reference, not the main story

</details>

---

### How I keep quality

No `npm install` to hide behind — every featured repo is **stdlib-only**, has a `README + ARCHITECTURE.md`, and you can run `python -m pytest` with no setup.

| Project | Tests | Docs | What’s solid | One thing I’d still polish |
|---|---|---|---|---|
| **pylog** | 63, incl. virtual-clock + Jepsen fuzz | `tla/pylog.tla` + `docs/` | Group-commit, snapshots, joint consensus | Add `TLC` in CI matrix for 3.12 |
| **leafdb** | 137, diff vs SQLite | `DESIGN.md` | WAL CRC + `check()` invariants | `FLOAT` already added — next: `VARCHAR` |
| **searchforge** | 50, global-IDF proof | `ARCHITECTURE.md` | BM25 + RankNet + sharding | Add `WAND` pruning for large corpora |
| **minichain** | ~40, chain + VM + P2P | `README` | PoW retarget, `heaviest` fork | Add `UTXO` model |
| **forgelang** | 64, conformance | `ARCHITECTURE.md` | Pratt + dual VM + GC | Add `closures` in `for` |
| **forgehttp** | 112, adversarial parser | `metrics` | `selectors` reactor, smuggling guard | Add `h2` |
| **miniraster** | 35, pixel-perfect | `docs/` | `1/w` + BVH + PNG | Add `BVH SAH` vs median |

> If you want the deep dive, each repo’s `ARCHITECTURE.md` walks through the trade-offs.

---

### Resume

<details>
<summary><b>📄 View Resume — Rahul Raj Singh</b> (click to expand)</summary>

<br>

**Rahul Raj Singh**
+91 93425 65503 | rahulrajsingh.work.15072005@gmail.com | [LinkedIn](https://linkedin.com/in/rahul-raj-singh) | [GitHub](https://github.com/rahulrajsinghwork15072005-a11y) | [Portfolio](https://rahulrajsinghwork15072005-a11y.github.io)

#### Education
**Vellore Institute of Technology, Chennai, TN** — *BTech in Computer Science and Engineering* — *May 2027 (Expected)*
- Relevant Coursework: Data Structures & Algorithms, DBMS, Software Engineering, Statistics, Cloud Computing

**GT Aloha Vidya Mandir, Neelankarai, Chennai, TN** — *AISSCE 2023: 90.2%*

**St. John’s Universal School, Palavakkam, Chennai, TN** — *AISSE 2021: 94.2%*

#### Experience
**Ford Business Solutions, Chennai, TN** — *Data Engineering Intern* — *June 2026 – Aug 2026*
- Built and maintained scalable ETL pipelines using Python, SQL, and Apache Airflow on GCP (BigQuery, Cloud Storage, Dataflow), reliably processing **2M+ vehicle-sensor records daily** with **99.9% uptime**
- Optimized legacy workflows by rewriting SQL + incremental loading, **cutting runtime 35%** and **compute costs 20%**
- Co-created Agentic AI architecture for autonomous data-quality monitoring (Agathon 2026 hackathon) — projected **24 hours/week saved**, **$18M revenue impact**
- Placed **joint 2nd in Round 1 (220+ teams)** and advanced to Final Shortlist of **13 teams**; presented to senior leadership

**Havoltz, Chennai, TN** — *Tech Lead (Robotics & Embedded Systems)* — *Sep 2025 – May 2026*
- Led 6-person team to build line-tracing autonomous robots in C/C++ with IR sensors — **95% path accuracy**
- Optimized real-time control with PID tuning + interrupt-driven polling — **cut latency 20%**

**E-Search Advisors Digital Services, Chennai, TN** — *Data Analyst Intern* — *May 2025 – Aug 2025*
- Audited website data quality for 12+ clients in Excel (VLOOKUP, pivot tables) — **40+ tracking errors/site fixed**
- Built automated Looker Studio dashboards — **reporting time 6h → 1.5h**
- Correlation analysis in Excel/Python → **22% organic traffic increase**
- Prepared A/B test summaries in SQL + PowerPoint for clients

#### Projects
**Text-to-Braille Conversion System** | *Python, OpenCV, scikit-learn, Raspberry Pi*
- Portable assistive device: Pi camera → real-time Braille
- Preprocessed with OpenCV (grayscale, thresholding, contour detection) + SVM on 5000+ samples (**92% accuracy**)
- Drove refreshable display via GPIO (**<2 sec per word**)

#### Technical Skills
**Languages:** Python, C/C++, SQL, JavaScript, HTML/CSS
**Data & BI:** pandas, NumPy, scikit-learn, Matplotlib, Seaborn; Power BI, Tableau, Looker Studio
**Core CS:** Data Structures, Algorithms, DBMS, basic ML (regression, classification, evaluation)
**Tools:** Git, GitHub, Jupyter, VS Code, GCP (BigQuery, Cloud Storage, Dataflow), Apache Airflow, AWS, Raspberry Pi, OpenCV

</details>

---

### Stack

<p>
  <img src="https://skillicons.dev/icons?i=python,cpp,js,ts,go,sqlite,docker,git,linux" />
</p>

`Python` · `C++17` · `SQLite` · `Raft` · `BM25` · `B+ Tree` · `HTTP` · `Vulkan` *learning*

---

### Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=rahulrajsinghwork15072005-a11y&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="140" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=rahulrajsinghwork15072005-a11y&layout=compact&theme=tokyonight&hide_border=true" height="140" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=rahulrajsinghwork15072005-a11y&theme=tokyonight&hide_border=true" />
</p>

---

### Let's talk

- GitHub: [@rahulrajsinghwork15072005-a11y](https://github.com/rahulrajsinghwork15072005-a11y)
- Email: `rahulrajsingh2k5@gmail.com`

> Each repo runs with `pip install -e . && python -m pytest` — happy to walk through any of them.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e293b,100:0f172a&height=80&section=footer" />
