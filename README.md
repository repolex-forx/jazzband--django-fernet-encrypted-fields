# Repolex Knowledge Graph of jazzband/django-fernet-encrypted-fields

RDF knowledge graph data for [jazzband/django-fernet-encrypted-fields](https://github.com/jazzband/django-fernet-encrypted-fields), parsed by [repolex](https://repolex.ai).

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
rlex download jazzband/django-fernet-encrypted-fields
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── fb8f3bf51eb4bb03ffc6afa0ebcc8dfa55f3dc44
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── fb8f3bf51eb4bb03ffc6afa0ebcc8dfa55f3dc44
│           └── chunk-001.nq.gz
├── blob
│   ├── 0a9ff2401fa66edd3d6ba3447f4eabf43f3bacd3.nq.gz
│   ├── 86f8d2d72dcb1f2f23d1fe8457c0c1f87a57f732.nq.gz
│   ├── 8a1ce8710bfbfa4388b096dce9fbb57f78fff853.nq.gz
│   ├── 918ff66dc0042da05b657494c52dc03faf94df99.nq.gz
│   ├── 94c503f50a6f8a0c767382a2ec725eaae318f9f2.nq.gz
│   ├── 9d56770724cd8a66d5e81e915f25bfd8f224cf01.nq.gz
│   ├── bf8f3001e1fa09efbf01627f69b7b00910871691.nq.gz
│   ├── c5770023ac372bbf6f2b9364472e9ff5a4262df6.nq.gz
│   ├── c60db26624dcb5abd3191eee679e339ad176f419.nq.gz
│   ├── dbe5feafb9711d6d7289ecd71c29dd1ce6f98714.nq.gz
│   ├── e169bcbc5f5b648814639340e8587f28d2160e00.nq.gz
│   ├── e2c9c3abded4100ef2e090a5bdf731a204faa634.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ef44a07087bc87d83f3179d1e3471c0a8f050c5b.nq.gz
│   └── ff1f2f0d0a1dc802507d271870f8e9b621902b78.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── fb8f3bf51eb4bb03ffc6afa0ebcc8dfa55f3dc44.nq.gz
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

[jazzband/django-fernet-encrypted-fields](https://github.com/jazzband/django-fernet-encrypted-fields)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
