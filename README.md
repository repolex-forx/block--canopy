# Repolex Knowledge Graph of block/canopy

RDF knowledge graph data for [block/canopy](https://github.com/block/canopy), parsed by [repolex](https://repolex.ai).

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
rlex download block/canopy
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── dfd2d6d8131745d3358255d3e3e794b34e0eb67b
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── dfd2d6d8131745d3358255d3e3e794b34e0eb67b.nq.gz
│   └── repolex
│       └── dfd2d6d8131745d3358255d3e3e794b34e0eb67b
│           └── chunk-001.nq.gz
├── blob
│   ├── 004145cddf3f9db91b57b9cb596683c8eb420862.nq.gz
│   ├── 00852b00daa400538045542a9c4aaa1f3a0b82d6.nq.gz
│   ├── 05435e9590c819ae56fa4aa8cdcf252533b500c0.nq.gz
│   ├── 0795e378b22b9a9f956e1b1010942a3d5f2af8c9.nq.gz
│   ├── 0b0b3e1c16e31b149cde716369b8586bb5257777.nq.gz
│   ├── 0ba9db25329d0b336e39ca8cde8470c5b7bc45eb.nq.gz
│   ├── 0fdb747685f624132a50bb01a3f33eb617c8a17d.nq.gz
│   ├── 108498c7e8fbfba03bc94527f3b777c3281ffca2.nq.gz
│   ├── 145fb45785e0f0e6cbcdde5e6a71e25f9929918b.nq.gz
│   ├── 17ebe99c82411a06769a90c1d176da0d502c9165.nq.gz
│   ├── 187e6dda4dc6ea27b0ada4bb3f38bef1b14f613b.nq.gz
│   ├── 18886f2e669a02ab20d7488706cefad122814644.nq.gz
│   ├── 1c6f8f3f35fc09486c6f507d7e37dad34bec002e.nq.gz
│   ├── 1ddbd7879ce411a6d4a421ea9c7bf8368ec39dbd.nq.gz
│   ├── 1fd89b07b98437c445d14f126497c290b60d2982.nq.gz
│   ├── 218eda26e4b8a008a31c523dec7486af3420724f.nq.gz
│   ├── 24672e229f42bd9346d51be332be4d87f9315efc.nq.gz
│   ├── 253a5337eee4f333db04f27f3b64d3eca513bd16.nq.gz
│   ├── 25f0bc5ed80683a81f46e6bfd1cf8ea0b56c6807.nq.gz
│   ├── 260dbe05a61b0eed0a422be8b04605d44989e142.nq.gz
│   ├── 2888a620dce58a6aadc63e5a8a9cb44bcca2b96d.nq.gz
│   ├── 294fd027002b5cfa323bf7ce9926a700670fc92c.nq.gz
│   ├── 2be9c310fea5cfe4916377ab4bd897e74f8c6fcf.nq.gz
│   ├── 2c739faa98eba7114ff364dd55fd79c7986f4a03.nq.gz
│   ├── 2d46221c47d9f24a6c1161490017f44fed2cf5b9.nq.gz
│   ├── 2d891b5400d90b17380e3990448acdb599604ca5.nq.gz
│   ├── 2f1ab140212f6ce091b2c53cb785037e4258e0c9.nq.gz
│   ├── 2ffbf24b68988bd935f5c695a59753fcb1a5de0e.nq.gz
│   ├── 333388e02cd78c9e358a163526ea2291218c5144.nq.gz
│   ├── 36fcb7452e9b03d22f10347d76bcff6d1dc1d6a4.nq.gz
│   ├── 39e6faf04c797f573484f33765d78797246afdc1.nq.gz
│   ├── 3e46199fc8d942aaac0fef8d014ed9908125ff71.nq.gz
│   ├── 42e524761cd59d4558bf3240cdd1f06a3a0231d2.nq.gz
│   ├── 43775ed9ba7d9b90b942b692251d6d2b773ee753.nq.gz
│   ├── 43da9ef60645a86b7c8ba013862edba31d1acba7.nq.gz
│   ├── 47e90d4bc01490943179e4013ea5cf882a0131c4.nq.gz
│   ├── 4902d6ef4d728ddebf0b55fbe4c2a61d8dedf2a5.nq.gz
│   ├── 4aca4300aea6f9f60c00448a0b890d0aaf6c9520.nq.gz
│   ├── 4d191609dbd0b4baa13a94bf25e4db70f9a22a04.nq.gz
│   ├── 4e691339c7a1419cc045c2b8eb06f7c4ed0aea6b.nq.gz
│   ├── 5174b28c565c285e3e312ec5178be64fbeca8398.nq.gz
│   ├── 567f17b0d7c7fb662c16d4357dd74830caf2dccb.nq.gz
│   ├── 58f069734bc4cf25e7e39e95778467a311c431ef.nq.gz
│   ├── 6161c9330f4d1e876b2a3d127fa50df4ca395b31.nq.gz
│   ├── 6715325f453cfa859f128be8d4e3aecc1dd00514.nq.gz
│   ├── 693e1c903c39329adade7a88ea0d7acd5ccd80aa.nq.gz
│   ├── 6a4a50f8125f2310a7cfaa10b8eea882e3ccb030.nq.gz
│   ├── 6aea79de5b4a09845b7e6102f1f06f8a8b0883de.nq.gz
│   ├── 6bccf43368fd7c96d9c659562a5142b8b8cb98a1.nq.gz
│   ├── 6c244448335e7eeeb4fddee005e4f9cfbcff0518.nq.gz
│   ├── 6e7549eab466a2b2dec6512506f4fb3ad5e2dbe3.nq.gz
│   ├── 71840b5ac80aefaf72db3f9c32babee0d2d5a0f9.nq.gz
│   ├── 718d6fea4835ec2d246af9800eddb7ffb276240c.nq.gz
│   ├── 71a3a01f2e475d42d7b01f5e7e72d8650c9e7c47.nq.gz
│   ├── 74c71b5c4bf8f3685da6327637f0e1eb6a8f536a.nq.gz
│   ├── 75abee0d9e1289039e1b74215c59e638b71b9b28.nq.gz
│   ├── 77053960334e2e34dc584dea8019925c3b4ccca9.nq.gz
│   ├── 7893f83ce82437973e93a376159ec45df44dbaa7.nq.gz
│   ├── 79ca6db7ad493eafa157f07696c46b916a4b441d.nq.gz
│   ├── 7f8cdbc31132982748b3aafb63d0f41f56f09b40.nq.gz
│   ├── 7fe2d420c7a0b614096704ddf1a531b88b2a89d3.nq.gz
│   ├── 80fadc44053cbc1760b7ed5180d250c27655fbb7.nq.gz
│   ├── 81f92973b16d9324d581be8f35346369dd56596d.nq.gz
│   ├── 842f7cfae8eba745fa732d131a69c8220b873f32.nq.gz
│   ├── 862ee3c28647e7a58801a75236855c269c1448ae.nq.gz
│   ├── 887545bdc87e415edb82bdcd1e289c579be2fd1a.nq.gz
│   ├── 8a4cfe1cf162a6894c0b6ed75b2c0eb4d979fea5.nq.gz
│   ├── 91a4f0836da70908f0a29b2f4a31e9618b916646.nq.gz
│   ├── 9582fc588754f78d9875691a3bd5e674295436b3.nq.gz
│   ├── 96dbc20298e484812c93755e343abb40bd941c2c.nq.gz
│   ├── 97c4ee602bb9de5a66a29e680375287f135b62d9.nq.gz
│   ├── 98a162d53eaec3e0eb65e92a3606afab8d1ae01e.nq.gz
│   ├── 9903d04e3085c794b4386101bb0e476fe626f2ae.nq.gz
│   ├── 9de786ab487fba8f511dede15e72353addf6180a.nq.gz
│   ├── 9fb74cf286ae51e17a5917b15fba5e50feab6a0a.nq.gz
│   ├── a34a3d560dc9b4387f995bc4692208c8a1f2381f.nq.gz
│   ├── a351705ebf9122d5c9b8ae337bb90a3dbed644f8.nq.gz
│   ├── a8c3ef9a35f1b81fb51c9af33a5662f1e37d2183.nq.gz
│   ├── aa922f770dfed57cab164ce111dc941ee4041027.nq.gz
│   ├── b2b2a44f6ebc70c450043c05a002e7a93ba5d651.nq.gz
│   ├── b52c0941ae3cca91ecbd98fd3d2660835cc070b3.nq.gz
│   ├── b57cc9d60b50031f4ef8e5ffba818363369cc930.nq.gz
│   ├── b71bbd999fdbfc348382bd19db286254201633ed.nq.gz
│   ├── bca6d4b13bb4be68283b80698ba4094d4d24aec3.nq.gz
│   ├── bcb1af877da3e3a5a609e48fe7f2e80f713340f6.nq.gz
│   ├── bd262bf5bac27f458e38432a88d099683f2b3d00.nq.gz
│   ├── bda6f01627489dd5cda0942d95d0605de1893fbd.nq.gz
│   ├── c110431151eaeb5425ce36a93d9caa5f790a23a0.nq.gz
│   ├── c325bbfaea0b556dbfab2017ae99810851d629c2.nq.gz
│   ├── c328baad19f80c797e95f007d76602291c1be533.nq.gz
│   ├── c38ca4dab722023599ea024451ca4332b035ebc1.nq.gz
│   ├── c41ce6926c15034427852a110d432f45dab026c4.nq.gz
│   ├── c42b177a8e2d608bd3b8967ccd8289db50f68a1a.nq.gz
│   ├── c71366c5cd4d0bb2864b3f962edcb60c39ca0a76.nq.gz
│   ├── c8724ce801e1e975348b5377485bd5989c8d2fae.nq.gz
│   ├── ca1d57f82ceec627e95aee8decfee43e8eb378e6.nq.gz
│   ├── cad74528b631ef416d6575a9bf9fb2e34c6ef94b.nq.gz
│   ├── cc8e155745e06da9eb3806141e76b44100a2b1bb.nq.gz
│   ├── cd26636a4ce111dda69bfc784debb162b3a0896a.nq.gz
│   ├── cdca62e4f7460226d1a7f889934430f9893070ec.nq.gz
│   ├── d0fd7f6d304365272de1f4a937f70311b43a2937.nq.gz
│   ├── d2c9f4715c4d4a5a28661d2d11e85749c5067862.nq.gz
│   ├── d3c7989d7210231374fb8ebc2ff243fcc84aea72.nq.gz
│   ├── d4a123730d7c20a2a8b6fb31fc1151288ac10c3f.nq.gz
│   ├── d61dd18be1bd803f9f4ab791ef69cf606f739e86.nq.gz
│   ├── d860e1e6a7cac333c3cc0bc9cb67faf286b07d69.nq.gz
│   ├── dada0552f29fa953a2889da82032d6071a32d0c6.nq.gz
│   ├── db70fc0f36f0f4fccff47be36a61ef29264b5117.nq.gz
│   ├── de33c611adef81009e0f977bbe559cbe341bb9e6.nq.gz
│   ├── dedd82f5f73fd83090f2a277769546239c4e20e4.nq.gz
│   ├── e4bcf29fc20b41e11a08e6474093655e4ed4bfa5.nq.gz
│   ├── e4c10b00b948b7c7f3b226836ef5f43163bcfc06.nq.gz
│   ├── e51f8665a61a0a72bca24836c5b903614dcdbb89.nq.gz
│   ├── ea9c223a6cbab0465000584a9d5dd052adffe3c2.nq.gz
│   ├── ec735377d24693c433b5bb2328d0d7a602819686.nq.gz
│   ├── f7aea06d00db3741a52661d4398b9ca98ef39b80.nq.gz
│   ├── f9b5c54392d4fa4b12d9e57080dc4f0022e9e75a.nq.gz
│   ├── f9ff2c404e1bb3967cbe034fdef513ce66c5cae6.nq.gz
│   └── fad946238ef5694e014a230b54c68781f0f3056e.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── dfd2d6d8131745d3358255d3e3e794b34e0eb67b.nq.gz
├── filetree
│   └── dfd2d6d8131745d3358255d3e3e794b34e0eb67b.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 129 files
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

[block/canopy](https://github.com/block/canopy)

---
*Parsed on 2026-10-02 by [repolex](https://repolex.ai)*
