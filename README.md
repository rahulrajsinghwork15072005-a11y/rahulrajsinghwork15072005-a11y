# Rahul Raj Singh — Systems From Scratch

> **7 FAANG-hire-signal projects** built **pure Python stdlib, zero deps** — DB engine, replicated log, blockchain, search engine, language + VM, HTTP server, 3D renderer. Each proven with **deterministic simulators / differential tests / conformance harnesses**.

`forgelang` · `forgehttp` · `pylog` · `leafdb` · `miniraster` · `searchforge` · `minichain` — all `80+ /100` under strict FAANG resume bar.

---

## 📌 Pinned — Lead with these 7

| Project | /100 | What it proves | Tests | Links |
|---|---|---|---|---|
| **[pylog](https://github.com/rahulrajsinghwork15072005-a11y/pylog)** — Kafka-style replicated log + Raft | **90** | Segmented `PLG1` log `log.py:27`, `truncate_from:394`, Raft `raft.py:620` PreVote/Raft lease/snapshot, deterministic `sim.py:185` virtual-clock | 53 tests | `pylog/log.py:27` `pylog/raft.py:620` |
| **[leafdb](https://github.com/rahulrajsinghwork15072005-a11y/leafdb)** — SQLite-inspired DB engine | **89** | B+ split/borrow/merge `btree.py:186` + `check():363`, WAL `core.cpp:666` CRC+redo, shadow pager `pager.py:88`, SQL `sqlparse.py:568` | 137 tests vs SQLite | `leafdb/btree.py:186` |
| **[searchforge](https://github.com/rahulrajsinghwork15072005-a11y/searchforge)** — Hybrid search IR engine | **89** | Positional index `index.py:107`, BM25 `bm25.py:35` k1=1.5, phrase `search.py:36`, co-occurrence vectors `vector.py:110`, RankNet `ltr.py:116`, global-IDF sharding `shard.py:50` `ARCHITECTURE.md:56` | 50 tests | `searchforge/search.py:36` |
| **[minichain](https://github.com/rahulrajsinghwork15072005-a11y/minichain)** — Minimal blockchain | **88** | PoW `block.py:84` compact `block.py:9`, retarget `chain.py:82` 0.25-4×, Merkle, heaviest-work `chain.py:299`, gas VM `contract.py:76` 21 opcodes, P2P `node.py:17` | ~40 tests | `minichain/chain.py:82` |
| **[forgelang](https://github.com/rahulrajsinghwork15072005-a11y/forgelang)** — Language + dual VM | **86** | Pratt `parser.py:365`, slot/upvalue `compiler.py:192` `vm.py:368`, mark-sweep `gc.py:75`, conformance harness `driver.py:62` | 64 tests | `forgelang/compiler.py:192` |
| **[forgehttp](https://github.com/rahulrajsinghwork15072005-a11y/forgehttp)** — HTTP/1.1 from sockets | **83** | `StreamParser` `parser.py:219` CL vs chunked smuggling guard `122`, `selectors` `loop.py:43` vs thread `server.py:26`, proxy `proxy.py:132` | 112 tests | `forgehttp/parser.py:122` |
| **[miniraster](https://github.com/rahulrajsinghwork15072005-a11y/miniraster)** — Software 3D renderer | **72** | Clip `rasterizer.py:31`, `1/w` correct `206`, shadow PCF `322`, PNG `image.py:69` | 35 tests | `miniraster/rasterizer.py:206` |

> Strict bar: `90-100` = distributed DB with proofs, `80-89` = complex system from scratch, `60-79` = solid, `40-59` = clone/CRUD, `<40` = trivial.

---

## 🗂️ Full portfolio (25) — remove duplicates before resume

| Repo | /100 | Type | Keep? |
|---|---|---|---|
| forgelang | 86 | language | ✅ pin |
| forgehttp | 83 | systems | ✅ pin |
| pylog | 90 | distributed | ✅ pin |
| leafdb | 89 | database | ✅ pin |
| miniraster | 72 | graphics | ✅ 5th |
| searchforge | 89 | IR/search | ✅ pin |
| minichain | 88 | blockchain | ✅ pin |
| healthcare-appointment-manager | 68 | full-stack CRUD+ | optional 6th |
| Compiler_Visualised_RRS | 66 | compiler viz | merge into forgelang |
| TOWER_DEFENCE | 64 | A* game | portfolio only |
| LOGIC-GATES | 62 | circuit sim | portfolio only |
| wikiConnect | 54 | canvas demo | keep 1 of 3 |
| makeNOTES | 52 | canvas demo | **duplicate — hide** |
| compiler-forge | 52 | compiler viz | **duplicate — hide** |
| mockDM | 48 | canvas demo | **duplicate — hide** |
| OSWEBSITE | 47 | OS viz | hide |
| spotifytiers | 45 | API wrapper | hide |
| Netflix_Clone_Portfolio | 40 | portfolio site | hide |
| dsa-tracker | 38 | tracker | hide |
| OS_CLONE | 38 | WinXP clone | hide |
| CSKWEBSITE | 28 | fan site | hide |
| LFC_WEBSITE | 26 | fan site | **duplicate — hide** |
| MY-portfolio | 22 | portfolio | **duplicate — hide** |
| Mepersonal | 12 | tribute | hide |
| healthcare_appointment_manager | 0 | empty duplicate | **removed** |

*Interview-prep notes in `Desktop/projects/interview_prep/` are local whiteboard scripts for the 7 above — not repos.*

---

## 🚀 Quick start (any of the 7)

```bash
git clone https://github.com/rahulrajsinghwork15072005-a11y/<repo>.git
cd <repo>
pip install -e .   # or just pytest (stdlib only for most)
python -m pytest -q
```

## Docs

* Each repo has `README.md` + `ARCHITECTURE.md` + `tests/` proving correctness (differential vs SQLite, Raft simulator, global-IDF shard proof, etc.)
* No frameworks, no ORMs, no `npm` — everything is data structures + math you can whiteboard.

---

**Contact:** Rahul Raj Singh · `rahulrajsinghwork15072005-a11y` · focus: systems, DB, distributed, IR, compilers

*Built Aug 2026 — all projects `pure Python stdlib` unless noted.*
