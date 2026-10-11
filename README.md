# Repolex Knowledge Graph of pytest-dev/pytest-timeout

RDF knowledge graph data for [pytest-dev/pytest-timeout](https://github.com/pytest-dev/pytest-timeout), parsed by [repolex](https://repolex.ai).

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
rlex download pytest-dev/pytest-timeout
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 16edd491cb2d65bfd6e0bc1d64173450cf23a01f
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 16edd491cb2d65bfd6e0bc1d64173450cf23a01f
│           └── chunk-001.nq.gz
├── blob
│   ├── 02e5e8f2f16a8ce53ddc8e4a70fa9628b23bf261.nq.gz
│   ├── 192a16cc934e1f8fb0ae475a0837f46b6af960d8.nq.gz
│   ├── 1e6e7b4a5c65a0a8ed62657d4c7345a02fc675e9.nq.gz
│   ├── 2a671c21dba235eb09e9701d9ac105d7237a66eb.nq.gz
│   ├── 56db748554cd6c73bc96100ed1e0b86be67d1bc9.nq.gz
│   ├── 866622f3f13b5ade41e3bc98f408ad239892743e.nq.gz
│   ├── 8f54b882646eeeda1aff10aa13bdf063cc3c0e23.nq.gz
│   ├── 90e22e1576ecda80708c3fa8ecc9107c9ee9e77d.nq.gz
│   ├── bcad554e626d5d0ac851ae8435a6046505f47d3e.nq.gz
│   ├── c03e9e78ab0eaff5df5fb644b3764893c9af8cb9.nq.gz
│   ├── d587992f687a59fceefac81a7e7a9f1bb9d0e723.nq.gz
│   ├── e968817fc44f0854c23699f7e5e631c53c96f2c7.nq.gz
│   ├── fc89131d2da0c35d9524891a2c17b31f2ae84ac9.nq.gz
│   ├── fed528d4a7a148fd0bf0b0198a6461f8c91b87e9.nq.gz
│   └── ff36c40bf9f0a8d8afe6004fe99e4cb71c5e06c9.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 16edd491cb2d65bfd6e0bc1d64173450cf23a01f.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 23 files
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

[pytest-dev/pytest-timeout](https://github.com/pytest-dev/pytest-timeout)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
