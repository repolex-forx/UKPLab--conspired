# Repolex Knowledge Graph of UKPLab/conspired

RDF knowledge graph data for [UKPLab/conspired](https://github.com/UKPLab/conspired), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download UKPLab/conspired
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 7388d896d8d56deac43e680d9ac66aa0517fc855
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 7388d896d8d56deac43e680d9ac66aa0517fc855
│           └── chunk-001.nq.gz
├── blob
│   ├── 064467ab47a22a5baa9f41c9342c01203dae8d18.nq.gz
│   ├── 0d03bf268c448d14aeb9becbc045bcde4ae6c9b7.nq.gz
│   ├── 0d04ca0d3d64fa049c03e162716c13762970accc.nq.gz
│   ├── 0d9360dc35d158ea1ccd025d9520994762579eec.nq.gz
│   ├── 0da4c7b287a1d23b979fa7bf663d75f919a02413.nq.gz
│   ├── 120c6893b8af8f69dddc51b2734ed561b78c6091.nq.gz
│   ├── 14411fd93d699377c6e17280cabaf9a39d67dbdc.nq.gz
│   ├── 229edba242bb190698662cdce6bdacde9f0769fe.nq.gz
│   ├── 24587d37d2a76daaef577f75f23a78abbf0bd8e0.nq.gz
│   ├── 3dc429a6613bf85898a47643fe31d4439fe9d973.nq.gz
│   ├── 4494992e95a890d760734ccf84e8f96ba53b132e.nq.gz
│   ├── 49e01fe6bb0beab27198682845e2f229e4e0b471.nq.gz
│   ├── 4be8d3e243a0581c9c1633b752c1466be6f19053.nq.gz
│   ├── 4cef27e61ea9ac6f982e68a89dcb12432298bb71.nq.gz
│   ├── 4ea99c213c5c0c005ae4e80df8e52169d06896ec.nq.gz
│   ├── 6681829782962f96bf77c41e48426460a8ad0549.nq.gz
│   ├── 68eb69b23434984ce6053d307b6b6b7f709a7e7e.nq.gz
│   ├── 698e9f972a96948e15606d89ceda254e571d2692.nq.gz
│   ├── 77b0e3ea3f554015c8d51e61470763ec697a3960.nq.gz
│   ├── 7a4953d6f0b5e41ea278495b4afb0e7654cc86ed.nq.gz
│   ├── 80f9dedb22582266a9daa4b5a74a2b7ef60f99a4.nq.gz
│   ├── 85408b37bfdb745a3fcfbd63cd3c143cfeaa97eb.nq.gz
│   ├── 8871abfdc9c3745a372d1b55952f4d24481e3ea0.nq.gz
│   ├── 8a32ee34b1603953ed79a91dec01453f67fb93c4.nq.gz
│   ├── 8b137891791fe96927ad78e64b0aad7bded08bdc.nq.gz
│   ├── 8b14d41f730e3642c5986d15e956bb8af5134367.nq.gz
│   ├── 9b3703a912d40f58fb0fb57d20742e53d9fe7671.nq.gz
│   ├── 9ccc7363dcc9155dec920e64a9820737d3fff0e3.nq.gz
│   ├── a4114ab3ef477bcc5c3025ba6b35e7e9aeb318e0.nq.gz
│   ├── a70d291241eea483a3e2ca58d7c779b17cc164b8.nq.gz
│   ├── b3c00dba1f8425a95fe7ce1945d03f48214269e8.nq.gz
│   ├── c08a79032592be8f5e7318991b0242323389469d.nq.gz
│   ├── c6718de5c5ae59d2c22141a147f5afba41af9cbb.nq.gz
│   ├── ca0475593900d0a936ed03cdbe531cbab9badd3a.nq.gz
│   ├── cc98b6933cd0df2705fd39225f24282258cd3685.nq.gz
│   ├── d53bb4f7214e97f220d122229829ee91a5c7e462.nq.gz
│   ├── d62fc66df4b9acdd5381753fde4173a5775b1ddf.nq.gz
│   ├── e2bf2830c56a280a95b781e29696178043e6eb3c.nq.gz
│   ├── e9e3e507b9d9120f7e3a094647805a8e6b2953e6.nq.gz
│   ├── e9e63f715509cb7b032e4b737043df844744fccc.nq.gz
│   ├── ea6d05ea8f9d193059c6b06318dbcc5229e7b33a.nq.gz
│   ├── ed3a9d377ba3c30e6eb8b2a35e08e8dc814a0725.nq.gz
│   └── f47c06cc18baa434989aa2d46756a0b678957242.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 7388d896d8d56deac43e680d9ac66aa0517fc855.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 50 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[UKPLab/conspired](https://github.com/UKPLab/conspired)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
