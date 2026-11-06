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
│   │   └── 9b19155e6fce04a83704eadc85d3dfe99e520c0c
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9b19155e6fce04a83704eadc85d3dfe99e520c0c
│           └── chunk-001.nq.gz
└── blob
    ├── 004a33532ea2547c10c0074b967733ba91edd9f8.nq.gz
    ├── 007bc813cea92c6555cde19b2ff0f8e779a59614.nq.gz
    ├── 00df9c999bff5a8b3a311e15f9d1bd1b167c04ff.nq.gz
    ├── 019fe75b9ad2644c2c8cd5941e350a6e58528d61.nq.gz
    ├── 01a5755dbadf129f6e8af650174a4b765c8d5234.nq.gz
    ├── 02851f596ceb281acc75c4d6a1aaf17eeee4a809.nq.gz
    ├── 02bbe7d8cb42c08d625711580c665b03770b7e44.nq.gz
    ├── 02f04e1320c4bbb2dd1eb5cb8f8ab17f9ca28223.nq.gz
    ├── 02fc7eda9a5592f0512243ba31d8e628b90ebaf9.nq.gz
    ├── 030e83d740d1197c634c9d105cf9143f60583c6f.nq.gz
    ├── 0345dc4a122b91fb8acbe2e377ab4dfdf0d6233e.nq.gz
    ├── 04880ce64be8a2e7bd5c59194565d55be506c281.nq.gz
    ├── 051ae997350f36ef1af9bfb2b1c64faa3a2a0db6.nq.gz
    ├── 056748648f5c42346e6657888557f1f8dcfee32b.nq.gz
    ├── 05b5462955e3dc113e3accf01e7ff72be00bc093.nq.gz
    ├── 068f0918a38581d97f9c4f0230e1838d107ead4a.nq.gz
    ├── 092d6eb8e36e2329c78d21bf609a8458818995e6.nq.gz
    ├── 0a6e81b440676b68ede88c3cc95ba0e68ab84a75.nq.gz
    ├── 0afd71fdcf4e5dfb465b76589825c2853d99cbe8.nq.gz
    ├── 0b5d2787c4efa04616d6dda7677217baa737925e.nq.gz
    ├── 0be7d5e0364ef72a88774a1fb107eac735cc7f8c.nq.gz
    ├── 0c188d20603d4fadbda4c5eb907c48ec19f68232.nq.gz
    ├── 0cdc0629c7a0e3366364e56b98a170680c099452.nq.gz
    ├── 0e30d83a33f504674cba758b73e14807a831af2e.nq.gz
    ├── 10de6d48bd5d573855a0328d55697b7153b9b88f.nq.gz
    ├── 116f1b7ef0f21fc8ca4591d02b5a896df961c88b.nq.gz
    ├── 12f893523529361bdf239456ea06fd82b0683841.nq.gz
    ├── 135bd908306dda377cc9bcf312d08315de978f90.nq.gz
    ├── 14fffb180f69ee1af6cd6874f745c1f500881e72.nq.gz
    ├── 151d783fce03df214754c83a289c5c6140a1fe72.nq.gz
    ├── 158ae548696abdba16056a9d7d4f9025c2ca8693.nq.gz
    ├── 15961518ee3aa41d1c79e14b48295e7c87eedce3.nq.gz
    ├── 170f4f89e7a291f988a33def9b5f8572c124e28f.nq.gz
    ├── 1728517f2a55dd3b52644af22f9cac76ec6f7701.nq.gz
    ├── 17bc811e968868430904409e513b0115e712aec0.nq.gz
    ├── 180ba5f20d48a2f52485d30803de8f9877d5fa18.nq.gz
    ├── 188f3eccccb5b7f6ff0898aef942364af486a5d6.nq.gz
    ├── 1893cfb96ab0d827e620106de177262396e9290f.nq.gz
    ├── 19965630d339d0087b3e24acb881bf5d39a06dbf.nq.gz
    ├── 1a89b9054d669db9cfb06aa2ce187b37f5d50eeb.nq.gz
    ├── 1bb3a7dcb0a187663898886ac9bd7d336c7b66e2.nq.gz
    ├── 1c8418e21e69277d420ad5970af1d6f7329f4666.nq.gz
    ├── 1cd102c777931aa9dfb09d087bb7ddb1993ecd38.nq.gz
    ├── 1d0d005fa55a9c365b58aef6ecca4d30426e8ae8.nq.gz
    ├── 1d35f132275b4e0ae9d6ec354bf6ecfee3a5493f.nq.gz
    ├── 1ea63b98d7f784e217b096eb1a2aa422eb858a73.nq.gz
    ├── 1ee8ec44e9536b461fc91b5cdb7a543993d7074c.nq.gz
    ├── 1f04ab2a8ec2dd483dd3582256561ec74b6ea8e5.nq.gz
    ├── 1f726ff8c94eae8041e62a72c328ccccecb41ee3.nq.gz
    ├── 1f81cb231efeb352b3bd6721fdf26e5d2ef81c8f.nq.gz
    ├── 200625f3b4a567b06d0aba84ea6d142ca7c787ca.nq.gz
    ├── 201f0b467ce987fe9cabb561a665056cf44fad02.nq.gz
    ├── 20885bbfdaabadd79f34069967eb75ccf84b24fc.nq.gz
    ├── 20e564387810ef697edb4345cef9d6eefcbb7d45.nq.gz
    ├── 217cc721fd364537df46103387f90039ac02cf06.nq.gz
    ├── 21e0b7dec5ba8d9f2478e0f194974dde56bc2a1c.nq.gz
    ├── 223966ff0c218f2b1de01093da1416df169fed85.nq.gz
    ├── 223ace8befa19013c0267f0e9f9203988c4ebe7a.nq.gz
    ├── 224ce5d7ee8ef71d9d4f92abfdd0881f97f4c93b.nq.gz
    ├── 22726a233d142ad2de982f8cc06f905b224bc4ea.nq.gz
    ├── 229a9887c54b2c470e28586d936569077dc1eac1.nq.gz
    ├── 22ac65a3ee70db89a4d3f859dc360ecdabf087ad.nq.gz
    ├── 2441bfb4785b60d97bd8edfaf559e718aaec85e5.nq.gz
    ├── 246ff84d1c947d70ad469c143952514ef1d262ed.nq.gz
    ├── 252de588acfb98fdc5b44964399f68846a9d56bb.nq.gz
    ├── 2583f21a516a15f21a72254dbdfd27fd6616c6f4.nq.gz
    ├── 266468b6f23a045fbbe735d0399a07cace0c063e.nq.gz
    ├── 26ac18c7eb53bbf994f89b75ddb959971f35ef6e.nq.gz
    ├── 26b4aada1454c9ec35a5cabf6682c1a1a1caeb14.nq.gz
    ├── 26d20e77a10c2dcaa5b3d9195a372d79170cd496.nq.gz
    ├── 2772b44dbc0827306fd9edf1b95126fc6e6a6536.nq.gz
    ├── 2857cf6e872a9dffa9cb6dbb8410b0b70e628792.nq.gz
    ├── 288c9cd03d8ef9b6e483c8f7bdfca06006c6ad5c.nq.gz
    ├── 2a053f3acec3d24566cf65bd0e069a3e16e2cb8d.nq.gz
    ├── 2ada5fca319f93f9db15b3e6c4addcd7a3cefbe2.nq.gz
    ├── 2bbc085e42c81cc5956b5d880328b9aace14f0d5.nq.gz
    ├── 2bdfb64a61ebbf6831be76a0cbfde3d533f4a180.nq.gz
    ├── 2c014412dbf6fd68729726e165fd963367b99828.nq.gz
    ├── 2c285515a3b39a35f128698b1daba218bf9f1d06.nq.gz
    ├── 2c74145d5673d5ff6b5dd0f0df2f951896f1cf77.nq.gz
    ├── 2c8dfc752b6b5149153245d64132f1cf13af52d3.nq.gz
    ├── 2cf4d55efd9e3f3e81ed1d296a6aaa2f783f8a53.nq.gz
    ├── 2d3b3d79b63a836d1c27061d9696c60265d1c856.nq.gz
    ├── 2d540b78fe4a24fe492f9b5ac6e72c584fbd5b42.nq.gz
    ├── 2f3fa2b075b173a70671e3910da598ce511e48cc.nq.gz
    ├── 2fc5d4a54b33f32525ce581b53ce4a24ea8c8082.nq.gz
    ├── 304fd46a2379cb3ee36fcd43bb9ae4eadb9339ac.nq.gz
    ├── 313d98e9fe5d92e2ebb62feb1792107f0cd9c9a8.nq.gz
    ├── 31468db114a26d12ed08e83bdc81b5bd4ac971e2.nq.gz
    ├── 31e4746c09d6a0b2fc3fd8b65be75a295412e11e.nq.gz
    ├── 3300fd56fb778ec1ce1f955a30d9236820cc60ed.nq.gz
    ├── 331691719e716cda9cb7596c964b9b0486d206f0.nq.gz
    ├── 3376223da2c54cab79f8670cd11e2ec6e59d0f3a.nq.gz
    ├── 33837ee6ea5a1978771ca186cc0eb107c74396b2.nq.gz
    ├── 33f9c197d6fc60caa222c92a6b1339601949f6b8.nq.gz
    ├── 347e7e71831770f42d7fdaf0b3c63a09409f659d.nq.gz
    ├── 3499547fc0a731cbddefe8881a9ef91c42f0f137.nq.gz
    ├── 35a51b7f994ac827eea19dc287bd4b9fa9990edf.nq.gz
    ├── 363e94f13bb5059ab6888af2fb60314699f1ab1e.nq.gz
    ├── 365affcbb7c1facdd1463b9700dd552d22898ab3.nq.gz
    ├── 368b72d45e9b84446487f59ff0f35e0c86aa236d.nq.gz
    ├── 36dcfa5b717f931e9958e688f3942e91143af4c3.nq.gz
    ├── 36e7c92e2f2ee10eb516b7802c629090d1ad1a10.nq.gz
    ├── 36f7ecc1ccc5025f073332c3ba735c751a7bbca3.nq.gz
    ├── 375fd4c4284a94c2959d74d4b19e5b50949e2053.nq.gz
    ├── 382c3ee645fd1b905a565422270cb5624e18dd5e.nq.gz
    ├── 3845ab1aa44e124247cea65b89f133219bf5909f.nq.gz
    ├── 3aabbc853358be86f0db1efce5bbc382ff1d6bd8.nq.gz
    ├── 3b16aab04338b74cfbbe91fa6f80d2f2b11676f4.nq.gz
    ├── 3bc2bac8bed87911c7644bc03da34b6742e667fd.nq.gz
    ├── 3d3c5f826d53c96dc1c6f98e2b87813b734048e4.nq.gz
    ├── 3d5bde7b2354fab57cdbc158c4a91c2e7bd50972.nq.gz
    ├── 3fb4411ade204e407b9ff6ff14829b7795682969.nq.gz
    ├── 40945770e25fc79bb50d2be0ab45d7513f03cffe.nq.gz
    ├── 40dcac452153063a8559bc4c37781f03d915faf0.nq.gz
    ├── 418558d70565e53de6d1c188c3a6567d900d5545.nq.gz
    ├── 42867d054085f6366e637922f1e565f9eb39c398.nq.gz
    ├── 445d4c28bef1f5d48648c41c365deac96f495d7d.nq.gz
    ├── 4504a6924706df62dfd77d11b431a61caaa1a004.nq.gz
    ├── 452940da2599b526bebb3f4d9abd4ab9812a8052.nq.gz
    ├── 453b1312b7468e3b3cf472c78b38574982db877e.nq.gz
    ├── 45ab254c81d8c23e914894766df7939efc03f5ee.nq.gz
    ├── 4697e3c54a2938b3eadae51ddc6ba64fe0b9092c.nq.gz
    ├── 471f5f139dce69588af65d315c9ba6f6769a722d.nq.gz
    ├── 47c7a408bc75816de0e69775732e924197a997f0.nq.gz
    ├── 480a6ae50921efebf5930dc21caaa3a1a44945dd.nq.gz
    ├── 4815b62d0c3ccfe66707835ba8ceae3084668f99.nq.gz
    ├── 48529e34f275301d2178654e8a96e8bf5ae9ae59.nq.gz
    ├── 489913eb284c86c3fb6f37a8abb56af1246496d9.nq.gz
    ├── 48a0cd807ed538017b31dbb19b54e101ebf288bf.nq.gz
    ├── 49a206cfa529e9dde5c94519bca8036223b66a5b.nq.gz
    ├── 4a4fd22060ccf067d1753be892d08726d62c03e5.nq.gz
    ├── 4ae94fe30964e2e9cc84b53321a10fb2491876bb.nq.gz
    ├── 4bc84ca2dbb066c920816df2f4060ad4d052d0a2.nq.gz
    ├── 4bd7ba833d02d01ba3391a2745ae54a6aedeb8d5.nq.gz
    ├── 4c375112c09cd0db0142892811410b79f4b426d6.nq.gz
    ├── 4c5367166128cecc4336ce7568b47c1a4d5b182b.nq.gz
    ├── 4cd0d6e42c8cbc78f0b7c06b2e856f7d0856bbcf.nq.gz
    ├── 4d4d60b178a204d9aa434ca9663bcb07149a2886.nq.gz
    ├── 4d59340a4daf54f7229eeaee6c00e49a293c568c.nq.gz
    ├── 4f1df26089793fbe98cd417456f6f9c533085109.nq.gz
    ├── 4f442b69ec9651ef2be94fea4ea95070de1d6a3e.nq.gz
    ├── 4f586fdf301a743ae21753a757bd87226ba96810.nq.gz
    ├── 4fb5ecd14ae18a6e67f1751587f4ea13b4ff7ed6.nq.gz
    ├── 4fd6e9f45c8e2239eefc067097dfaca384c309c8.nq.gz
    ├── 506102a9207f2eabe8ed7b581a2bf5d162e95199.nq.gz
    ├── 508c1043b3b1aca3728849e1db089549a89e7a5f.nq.gz
    ├── 510695644e7be31512125c2e48bee33d8104e2e8.nq.gz
    ├── 521f1f607264fbf469013f69a14db2c8c87d2504.nq.gz
    ├── 52297747e5e4c7f0066db2c47615c41a43e11e7d.nq.gz
    ├── 5242c141fd7d4fa156c21712f6b5a981e15631e5.nq.gz
    ├── 52b1c8f303cef1d401aaf4095fd804dc51642a5d.nq.gz
    ├── 5347bcf46402997e644c2a6b3de8372bfac63874.nq.gz
    ├── 542e26147a0a80c8409ea8457ff85e878e633b44.nq.gz
    ├── 54653bc88e08cf4139e72003054f0fc6313cb463.nq.gz
    ├── 54adf649909f1ffaff5f4f2470df49edca3d72e4.nq.gz
    ├── 56b170d380376604f308a28cb2ca92ed1f1481cc.nq.gz
    ├── 56e747dac3f74dfea3bc4887781c0c44ab83bcfa.nq.gz
    ├── 573082131bf29c855440a4e23c6a3596659e4060.nq.gz
    ├── 5736c348b384f0ea525d634a6dbc443b96cc6273.nq.gz
    ├── 575655079b550e39bc2fe93129d31e6ccc262a46.nq.gz
    ├── 581c65de788284b089fce26a7cc2359b6767dde0.nq.gz
    ├── 5857341f7cbab436a530d787ea5956cbadefe23b.nq.gz
    ├── 58bc74d12b8d4bf28c2c008b57ea9eb32ac0244a.nq.gz
    ├── 58e015e5df012567fe2553eabcefc383549d002d.nq.gz
    ├── 590cd99352fb7706ca5b4390d534144a8af6cee2.nq.gz
    ├── 59f847c91a4d1029530045676a576fa33d7c1c42.nq.gz
    ├── 5a02b2ca907733a8e1ab404d1107bb702e977748.nq.gz
    ├── 5a76ee266bf5c9ae235ccf677e499a071f3c6bf5.nq.gz
    ├── 5a7f202a7a966765b85fa8b1a5e8564ceb72c736.nq.gz
    ├── 5b5f87085a0b933d73826c970b078a4f573aeedc.nq.gz
    ├── 5c4e66640c4926cfaca36159e85db68c496af4a6.nq.gz
    ├── 5c82f781e53ab3f1f943b9ab00be4ab0c20fcbb2.nq.gz
    ├── 5d344400d3b8771d2c1b93ba48def361615a132f.nq.gz
    ├── 5d4859f7a72d4510b35164bae50a0f16c66b9da1.nq.gz
    ├── 5d50d7e082e43d98d3bad958d9c21fffea910cb7.nq.gz
    ├── 5e00ec899886e4c4a5fe6ff298eefee9396e3cf5.nq.gz
    ├── 5f3f5a690bc2a2545da8f0f66cc081a370e5085b.nq.gz
    ├── 603aa51c569fd175b85061bc53f9bab59bea0d39.nq.gz
    ├── 604e23271cb556ca7f9a0dcb4a969cc9989f5fda.nq.gz
    ├── 60a7105d04f1fcf15232cdb06c7961da19e60671.nq.gz
    ├── 61aa879a8a125b323b03a744081b36ec24e913a6.nq.gz
    ├── 61bcdf8ee3a29910be92b4a1711a096db8acf452.nq.gz
    ├── 6267d77b28dc0d38959c35ef1f8467d925fc4eac.nq.gz
    ├── 62738acda775d5f28eaded3c83c44c13a7d90af0.nq.gz
    ├── 627a4c5f24dae3067fa2413f2ce70f1db6698fde.nq.gz
    ├── 62a4c57e7ee2e910e9c46f23140214a4f43eed0d.nq.gz
    ├── 634914cbf5cb241c0cc2112420620faba9436543.nq.gz
    ├── 64cc80b411dc9868c864c0c0f4f610418cd2fbdd.nq.gz
    ├── 65a8037835879ed4095e847d2ae928c0524395c6.nq.gz
    ├── 661efc783477167f450d8cf15a9cf1b971fd31bb.nq.gz
    ├── 6694ae5ad3d466f77082d63a869b810d55aafd85.nq.gz
    ├── 66bf1739a00b0cdd7d72e0927fc49589f1917cce.nq.gz
    ├── 670f27aaa13c6767a37d88f072950c077b6e519d.nq.gz
    ├── 679caa5ab3a77aaec65540ed562078203f478bfd.nq.gz
    ├── 67ad3f75b543f0a34b516b0178414abdfb22e1d1.nq.gz
    ├── 688fbe7775ac26b327b75bffbe23ed26f999293f.nq.gz
    └── 68d7394fd7b4668ba764d2bc54eafe3b475e19ce.nq.gz

7 directories, 200 files
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
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
