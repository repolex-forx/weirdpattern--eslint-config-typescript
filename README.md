# Repolex Knowledge Graph of weirdpattern/eslint-config-typescript

RDF knowledge graph data for [weirdpattern/eslint-config-typescript](https://github.com/weirdpattern/eslint-config-typescript), parsed by [repolex](https://repolex.ai).

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
rlex download weirdpattern/eslint-config-typescript
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 98ab70a46755f49dbd7981f848c526e27a362608
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 98ab70a46755f49dbd7981f848c526e27a362608
│           └── chunk-001.nq.gz
├── blob
│   ├── 002f2941e183bdcca8906c4261916b55034cb618.nq.gz
│   ├── 02e451640b054360b95df42a90833b9dc21230f9.nq.gz
│   ├── 1affc8d75b30d00e613ca336f320a4d128df893d.nq.gz
│   ├── 2ad9329a794a10d9df780d5b6c8a83370f339480.nq.gz
│   ├── 3db21be4254924c370cb9adcec894d6477ba52fe.nq.gz
│   ├── 53493c7a9261974f12e885a6855a03f2a56b65dd.nq.gz
│   ├── 624bb54bf7b965e27d711ee54c779962755f0051.nq.gz
│   ├── 627a4c7722716e73fb059eee3f1983b07f392adc.nq.gz
│   ├── 6b569e53cf29bb91fd0ee33d48f2fe922bdcd014.nq.gz
│   ├── 6e61ae9eeebd1f0df85935c8e0af35a207ce218a.nq.gz
│   ├── 6f0a469f4889a8a012b02bbc457b12e62e00be58.nq.gz
│   ├── 7b2a77bedf2ffcecf1bff3ef834c324475311d30.nq.gz
│   ├── 81da2c85948bcb6e8beba134f67c1e9de5bc952e.nq.gz
│   ├── 85df127f13590afdf0b58ab2f4f52babe09e47c4.nq.gz
│   ├── a156413d6a0e1a9d881d26c451412e7f84ed37b9.nq.gz
│   ├── a5979edcdf387ce532f5f4aba27735e203f75409.nq.gz
│   ├── b2e7a3960cc20befd2bd1285e2312c39f96816b9.nq.gz
│   ├── b7476cff19c89654856f85169474f5e26da3ced2.nq.gz
│   ├── c1ca392feaa48b046ffc56d4feed1887af232461.nq.gz
│   ├── c718ac390315f28b661ceec16189ebcb22b73cac.nq.gz
│   ├── c80d6964de674f68545916a14ac4d3d2be126991.nq.gz
│   ├── c9e0f4781a448c06bbdd3eabb90b1cf6e9bdecfc.nq.gz
│   ├── d695d8f415f7225e5f3e10f46500744e32a8c4a1.nq.gz
│   ├── ddda10b4a36b50367505912f2bcca3436aafd6bc.nq.gz
│   ├── e401a6c02123afe7aa011445e013912f7ffff860.nq.gz
│   ├── f27c9fcd9e524a18540f5c698458b179b68e7420.nq.gz
│   ├── f4d32ee5ba3801764e94b6ba5aa8b57d7d73379b.nq.gz
│   └── fcadb2cf97913f58a2523f535336e725c6b59d1f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 98ab70a46755f49dbd7981f848c526e27a362608.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 36 files
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

[weirdpattern/eslint-config-typescript](https://github.com/weirdpattern/eslint-config-typescript)

---
*Parsed on 2026-11-10 by [repolex](https://repolex.ai)*
