# Repolex Knowledge Graph of pytorch/audio

RDF knowledge graph data for [pytorch/audio](https://github.com/pytorch/audio), parsed by [repolex](https://repolex.ai).

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
rlex download pytorch/audio
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 34c52a67e8941bbd8e6adaca0eb0b9eabec11d78
│   │   │   └── chunk-001.nq.gz
│   │   └── 9b19155e6fce04a83704eadc85d3dfe99e520c0c
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 34c52a67e8941bbd8e6adaca0eb0b9eabec11d78.nq.gz
│   └── repolex
│       ├── 34c52a67e8941bbd8e6adaca0eb0b9eabec11d78
│       │   └── chunk-001.nq.gz
│       └── 9b19155e6fce04a83704eadc85d3dfe99e520c0c
│           └── chunk-001.nq.gz
└── blob
    ├── 00111e68b7a6ac9dac86ea5bb15fe1d935c41da4.nq.gz
    ├── 004a33532ea2547c10c0074b967733ba91edd9f8.nq.gz
    ├── 007bc813cea92c6555cde19b2ff0f8e779a59614.nq.gz
    ├── 00a7cd637b255cfd409a6e8f8bf9214776c79f80.nq.gz
    ├── 00df9c999bff5a8b3a311e15f9d1bd1b167c04ff.nq.gz
    ├── 00dfe68b9d318eda3b9937a7c5ca452ef4ca4e94.nq.gz
    ├── 00e57a2de2454acf102cc99daa92739831b3baf8.nq.gz
    ├── 0104e752b5a6f62526ed688ec55adc196d6e8ede.nq.gz
    ├── 0120c997c0bec7790186646ca0f5f3be657c5fc6.nq.gz
    ├── 019fe75b9ad2644c2c8cd5941e350a6e58528d61.nq.gz
    ├── 01a5755dbadf129f6e8af650174a4b765c8d5234.nq.gz
    ├── 01c14a05c97bac997f77c4c0ee75f95ae462ed19.nq.gz
    ├── 01e51939c8cfeffaa10296766a2aa51bbc7bdb49.nq.gz
    ├── 01e820013e0d6fdc2aa9d69c8ae95a7817ad75e3.nq.gz
    ├── 01ee3f7e60e2caf3ca0b692689f4ca77a2fb4e8c.nq.gz
    ├── 020b04f4b834e65811d75e37fd87fd9e510e24dc.nq.gz
    ├── 0236732dfbaa5e1c62d5b4febdcb1dd9ec59e3f3.nq.gz
    ├── 02851f596ceb281acc75c4d6a1aaf17eeee4a809.nq.gz
    ├── 02bbe7d8cb42c08d625711580c665b03770b7e44.nq.gz
    ├── 02f04e1320c4bbb2dd1eb5cb8f8ab17f9ca28223.nq.gz
    ├── 02fc7eda9a5592f0512243ba31d8e628b90ebaf9.nq.gz
    ├── 030e83d740d1197c634c9d105cf9143f60583c6f.nq.gz
    ├── 0333ca605dd09e752e6f637ef17451c7450386f5.nq.gz
    ├── 0345dc4a122b91fb8acbe2e377ab4dfdf0d6233e.nq.gz
    ├── 037b053099ebb566e9b74e79de46c96225e6dd7b.nq.gz
    ├── 03d47ce576464730683d08a6fb2a965e893e0426.nq.gz
    ├── 042020f12036300ae84591761c900b8298cdace8.nq.gz
    ├── 0457b5dd707f7216adc3ea919ba8e257d86f4f71.nq.gz
    ├── 0482e4293b225ddb752346cc46637931969d0fe1.nq.gz
    ├── 04880ce64be8a2e7bd5c59194565d55be506c281.nq.gz
    ├── 049d7a7fa1ce786799433a01e85e61e70d1f5e75.nq.gz
    ├── 04e4264bf2789ad305b4a4c2529652a9235678f7.nq.gz
    ├── 04ee24350fd6780e9a48751c1944dd320dce51c0.nq.gz
    ├── 05023f5cc6ce098d5e1677f3e85b48b6b14d5d51.nq.gz
    ├── 051ae997350f36ef1af9bfb2b1c64faa3a2a0db6.nq.gz
    ├── 056748648f5c42346e6657888557f1f8dcfee32b.nq.gz
    ├── 0588dd29ab9f9921ca7f33f5693e05df8011c93f.nq.gz
    ├── 05b5462955e3dc113e3accf01e7ff72be00bc093.nq.gz
    ├── 0601b7c5003fb402291e9bef36bcf1c623179e77.nq.gz
    ├── 064423c4494850f2ad8f43fb00a956be21fcb95e.nq.gz
    ├── 0660de3ef1b293c8117220598d2ad4c92100aca8.nq.gz
    ├── 068f0918a38581d97f9c4f0230e1838d107ead4a.nq.gz
    ├── 069d13192420834bfdaf6266038476a19c708382.nq.gz
    ├── 06f616fe758f8399b9d1916614aeae0eb0281238.nq.gz
    ├── 07646f64ae9284f0ac0adc651b74251eb8dd6d05.nq.gz
    ├── 077a04c950335c7a1a1ee3592b514b1ef73994c2.nq.gz
    ├── 07a26974c59e066235806962302aa8241a3b8a7a.nq.gz
    ├── 07a835f91702b30a26f4e6e7ff503e7a1b79ee95.nq.gz
    ├── 07b78050e81cbf7a2edcabc8297be7422841a9a9.nq.gz
    ├── 081dc1415563c02a87a4ce20b7470e46a6e5092c.nq.gz
    ├── 0837d3e173d3c1bb237acafb50da3ab8e9329eb1.nq.gz
    ├── 08469e1031ea03a310706f689e20e2e80d06f2b3.nq.gz
    ├── 089c261c20205a47e54b4df68bc73747675ffa0d.nq.gz
    ├── 092d6eb8e36e2329c78d21bf609a8458818995e6.nq.gz
    ├── 09cd68a047ed371a163afc031816434192cc1557.nq.gz
    ├── 09f5e94df44c3b4a45440155ec72726add1de661.nq.gz
    ├── 0a6e81b440676b68ede88c3cc95ba0e68ab84a75.nq.gz
    ├── 0a84e4cb24d8b71b0443407fa2b8603befe36f6c.nq.gz
    ├── 0af68c17b948baad8aac82cfd3adb92d904cb603.nq.gz
    ├── 0afd71fdcf4e5dfb465b76589825c2853d99cbe8.nq.gz
    ├── 0b01694edbb75aa1d539df606b3f64ca647280e2.nq.gz
    ├── 0b1c7b1f92a75756fa12180be714cfd0c7892f49.nq.gz
    ├── 0b2ca6f1e0fef22ffb6bee977e358c1020543351.nq.gz
    ├── 0b5d2787c4efa04616d6dda7677217baa737925e.nq.gz
    ├── 0b7a33dd2455a98f0a14eb709d09caca42d7b3f7.nq.gz
    ├── 0b93add2e779607d911437e12bbefdee7c45aa96.nq.gz
    ├── 0be7d5e0364ef72a88774a1fb107eac735cc7f8c.nq.gz
    ├── 0c188d20603d4fadbda4c5eb907c48ec19f68232.nq.gz
    ├── 0c7e28c3b35489872d3425dc7cbe511911140cbc.nq.gz
    ├── 0cdc0629c7a0e3366364e56b98a170680c099452.nq.gz
    ├── 0d0608801d824d7c3e1123053fbeb3c1a1e707e4.nq.gz
    ├── 0d482a6e4d12f4960a6c0a10de785b161d45af0f.nq.gz
    ├── 0d56b09c7c2f446548e763752a388639c635be88.nq.gz
    ├── 0dd2dcba9cc5fd9bc0d8dfd6fa3f3c765fd29260.nq.gz
    ├── 0dd5cf962701bfb088ca6c2deea711fd697e38f4.nq.gz
    ├── 0dec0362ed1f4606d9464d98f150eda1039e7b35.nq.gz
    ├── 0e06357ae62d5844a62102248b68ee4af2bf7a41.nq.gz
    ├── 0e30d83a33f504674cba758b73e14807a831af2e.nq.gz
    ├── 0e6e872082f170288210c62bfe6ce593fdc73786.nq.gz
    ├── 0fba71e451872554714b5f9e915b158c62421316.nq.gz
    ├── 0fc09d08e980285aebdc84f6707b69b1f551d5a7.nq.gz
    ├── 0ff97b036e37af19f4007db1104b14342c4cf085.nq.gz
    ├── 107a251da8201851f12a63320efdea689dc5a7e7.nq.gz
    ├── 107de5ac6934f3d52b64da3f27e489ab6d1f04fd.nq.gz
    ├── 10de6d48bd5d573855a0328d55697b7153b9b88f.nq.gz
    ├── 114d9f6e0a8a45b59ecaddda5c0c9fd78f12926c.nq.gz
    ├── 115b977cd14b4278a818b4ba43ea8147e8c76237.nq.gz
    ├── 116f1b7ef0f21fc8ca4591d02b5a896df961c88b.nq.gz
    ├── 122da5a5e2474b02cc209e747364d1f32b1c2c24.nq.gz
    ├── 127afa8bf9af536a5c4e7e5a30726fc8fb1b594e.nq.gz
    ├── 12e73ea10d54ad3d5b5ad2bc6edfa1f2828fdc6a.nq.gz
    ├── 12f51c29cb927012ba19c6552d4f95775dc2753d.nq.gz
    ├── 12f893523529361bdf239456ea06fd82b0683841.nq.gz
    ├── 135bd908306dda377cc9bcf312d08315de978f90.nq.gz
    ├── 136e6844f29f56153c49b324fa668a9d812c1737.nq.gz
    ├── 137bd3ef508d8f11b0de24e82bd2b39e2c7c9780.nq.gz
    ├── 13eb0275afb437b85abda6770f4ac4898e3186e2.nq.gz
    ├── 1409d9c506cfdef2976fad6719ad6403cbff81de.nq.gz
    ├── 14fffb180f69ee1af6cd6874f745c1f500881e72.nq.gz
    ├── 150687b04a7206ec272a76abee47d48742f6d561.nq.gz
    ├── 151d783fce03df214754c83a289c5c6140a1fe72.nq.gz
    ├── 158ae548696abdba16056a9d7d4f9025c2ca8693.nq.gz
    ├── 15961518ee3aa41d1c79e14b48295e7c87eedce3.nq.gz
    ├── 15da3576219b1fd55ece2417d09e0f8033f1fe19.nq.gz
    ├── 15df99e3dcac61d97de7ffb43b30b137409fbd0d.nq.gz
    ├── 16a9045ad663d309f3b0bd599d9ec8801fa5d464.nq.gz
    ├── 16c387f4f8c189379f6844a24691f3bf47db8362.nq.gz
    ├── 170f4f89e7a291f988a33def9b5f8572c124e28f.nq.gz
    ├── 171bfe8554f2db6d1a6bef6180fe8bc5be47a021.nq.gz
    ├── 1728517f2a55dd3b52644af22f9cac76ec6f7701.nq.gz
    ├── 178767e4a156aff96d72b67cc87c781866283d63.nq.gz
    ├── 17bc811e968868430904409e513b0115e712aec0.nq.gz
    ├── 180ba5f20d48a2f52485d30803de8f9877d5fa18.nq.gz
    ├── 182c9f7e3f89f5bb58c03504780e961e0ca3aded.nq.gz
    ├── 184bd2fd3a8ba742e00f561ac7c0773a67540dcb.nq.gz
    ├── 188f3eccccb5b7f6ff0898aef942364af486a5d6.nq.gz
    ├── 1893cfb96ab0d827e620106de177262396e9290f.nq.gz
    ├── 18f22b33b4d44311f0168bd0f8f9147a95862d34.nq.gz
    ├── 1945fc75c18b474404b733e43d50156f3c3d6652.nq.gz
    ├── 194dabc4a97be8e163f3b410ef83ba77129c1c27.nq.gz
    ├── 19827e184d63efbd6daa46a7a33662cb3c23ac43.nq.gz
    ├── 19965630d339d0087b3e24acb881bf5d39a06dbf.nq.gz
    ├── 19bfa85ee0c15fbcfc1343ea3ad136a689bbb8d5.nq.gz
    ├── 1a046637f8d8b6b300b6ebd95d087c8ecd46cef1.nq.gz
    ├── 1a2a9ef0e625b95d0dd3d26c4c97dcd41b297d96.nq.gz
    ├── 1a2cce7ace2ced46495ace65af3a989d82e69ab6.nq.gz
    ├── 1a89b9054d669db9cfb06aa2ce187b37f5d50eeb.nq.gz
    ├── 1b1adcafa692a10e728a8ec2d77a5580312d21fb.nq.gz
    ├── 1b2b3a8a3f737e83203f8dc7c19a6dc254261e01.nq.gz
    ├── 1b4da14679666bae44922277c7ed9808692265fe.nq.gz
    ├── 1b9834666d1bfdf9bb1719697f5c92c28bf529d8.nq.gz
    ├── 1bb3641c57ea4e32ec04e957da249bb956f71301.nq.gz
    ├── 1bb3a7dcb0a187663898886ac9bd7d336c7b66e2.nq.gz
    ├── 1bec23eaf1dd562ae3d3216420b1b1bbfbd39cbc.nq.gz
    ├── 1c135fef4e598319348ed020eba32fd857f1d595.nq.gz
    ├── 1c4017ff39b79daa31f30c496461589a2d01b756.nq.gz
    ├── 1c8418e21e69277d420ad5970af1d6f7329f4666.nq.gz
    ├── 1cab09a7e2a56f24deca5cc13be760cc216d8c77.nq.gz
    ├── 1cd102c777931aa9dfb09d087bb7ddb1993ecd38.nq.gz
    ├── 1cdbd66b9cd0d77ef2576beab4ef8d46e5cd4f89.nq.gz
    ├── 1d0baf75a71792a7b27646542bc92cef97f50c50.nq.gz
    ├── 1d0c100266e2f8df56ad0fad1026f26a0d81d888.nq.gz
    ├── 1d0d005fa55a9c365b58aef6ecca4d30426e8ae8.nq.gz
    ├── 1d35f132275b4e0ae9d6ec354bf6ecfee3a5493f.nq.gz
    ├── 1d4212c2231aa1a0daecdf29e1cd2a919abceda7.nq.gz
    ├── 1e66c978b17f55fb306f9e029ac2e79475abeac4.nq.gz
    ├── 1ea63b98d7f784e217b096eb1a2aa422eb858a73.nq.gz
    ├── 1ee8ec44e9536b461fc91b5cdb7a543993d7074c.nq.gz
    ├── 1f04ab2a8ec2dd483dd3582256561ec74b6ea8e5.nq.gz
    ├── 1f3117b609d4f580358adb96a3278f4a914ae4d2.nq.gz
    ├── 1f42644ae8019fbe5a4adf0795bc96e80b5097ca.nq.gz
    ├── 1f50b1b05b530204bf32c6986fffc0aa8370ce54.nq.gz
    ├── 1f726ff8c94eae8041e62a72c328ccccecb41ee3.nq.gz
    ├── 1f81cb231efeb352b3bd6721fdf26e5d2ef81c8f.nq.gz
    ├── 200625f3b4a567b06d0aba84ea6d142ca7c787ca.nq.gz
    ├── 201f0b467ce987fe9cabb561a665056cf44fad02.nq.gz
    ├── 206009e29e6d3b166203b98769b78c6ccbce97a3.nq.gz
    ├── 20885bbfdaabadd79f34069967eb75ccf84b24fc.nq.gz
    ├── 20e564387810ef697edb4345cef9d6eefcbb7d45.nq.gz
    ├── 217cc721fd364537df46103387f90039ac02cf06.nq.gz
    ├── 21e0b7dec5ba8d9f2478e0f194974dde56bc2a1c.nq.gz
    ├── 2217ef49849b460d2b581ba7e7d17d8c6404ec03.nq.gz
    ├── 222d3ef8a4bc1c04a0a14f3618615920e0b3bd53.nq.gz
    ├── 223966ff0c218f2b1de01093da1416df169fed85.nq.gz
    ├── 223ace8befa19013c0267f0e9f9203988c4ebe7a.nq.gz
    ├── 224300a84f5ec3ae217f030783c825fc3db56c8a.nq.gz
    ├── 224ce5d7ee8ef71d9d4f92abfdd0881f97f4c93b.nq.gz
    ├── 22726a233d142ad2de982f8cc06f905b224bc4ea.nq.gz
    ├── 229a9887c54b2c470e28586d936569077dc1eac1.nq.gz
    ├── 22ac65a3ee70db89a4d3f859dc360ecdabf087ad.nq.gz
    ├── 22dd37216f8c64cdc497db01e19c08897ebc3f5c.nq.gz
    ├── 22f09569b659bbd46395f3c6ff8213faa92796f2.nq.gz
    ├── 234f85af3ae29e4b6d1d1b607952941fe9956d2d.nq.gz
    ├── 239209778d53aa0717bc36558b20f5afdfbca872.nq.gz
    ├── 239cf8e21ae2593b8b08d92deb573b1dc6152fe6.nq.gz
    ├── 2410764f36bd62eb5cf7673d0f576bd1acc898f2.nq.gz
    ├── 2441bfb4785b60d97bd8edfaf559e718aaec85e5.nq.gz
    ├── 246ff84d1c947d70ad469c143952514ef1d262ed.nq.gz
    ├── 24bc77e627cca2211d82d4823f3acdf633dbd445.nq.gz
    ├── 252de588acfb98fdc5b44964399f68846a9d56bb.nq.gz
    ├── 254122f0eee21906ec50f3d4238a5b3024e74a0a.nq.gz
    ├── 2583f21a516a15f21a72254dbdfd27fd6616c6f4.nq.gz
    ├── 25a67c3cd5e7f3e8442f70d1998c849f198ddd82.nq.gz
    ├── 266468b6f23a045fbbe735d0399a07cace0c063e.nq.gz
    ├── 266c80582c64399111c793937ed8906a08b5366e.nq.gz
    ├── 26ac18c7eb53bbf994f89b75ddb959971f35ef6e.nq.gz
    ├── 26b4aada1454c9ec35a5cabf6682c1a1a1caeb14.nq.gz
    ├── 26cabe1dcf4118ecbcd46159bf49b7a5cf798796.nq.gz
    ├── 26d20e77a10c2dcaa5b3d9195a372d79170cd496.nq.gz
    ├── 2772b44dbc0827306fd9edf1b95126fc6e6a6536.nq.gz
    ├── 277d4bb0b9b98ff6782344eb1c4cc2f056fac58b.nq.gz
    ├── 27b647c673eaba888729074a1a6e5466d93375fa.nq.gz
    ├── 27d5b788caf113bfaedee043baa381abb27632a7.nq.gz
    ├── 2857cf6e872a9dffa9cb6dbb8410b0b70e628792.nq.gz
    └── 288c9cd03d8ef9b6e483c8f7bdfca06006c6ad5c.nq.gz

10 directories, 200 files
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

[pytorch/audio](https://github.com/pytorch/audio)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
