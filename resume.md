# Chen Xinran (陈昕燃)

- Male / Born 1994
- Guangdong University of Petrochemical Technology – Food Safety (Undergraduate, withdrew). Self-taught computer science during university.
- **GitHub:** [Lawliet-Chan](https://github.com/Lawliet-Chan)
- **Phone:** +86 13965602037
- **Email:** crocdilechan@gmail.com
- **WeChat:** chenxinran1228
- **Telegram:** [@ChenXinran](https://t.me/ChenXinran)

---

## 🛠️ Tech Stack

1. Rust & Golang
2. Familiar with fundamental architecture of mainstream public and consortium blockchains (see my universal blockchain framework projects), including consensus mechanisms, state machines, transaction pools, networking, chain structures, etc.
3. Experienced with distributed systems (including distributed message queues, file systems, and databases) and storage engines (boltdb, badger).

---

## 🚀 Open Source Projects

### Personal Projects

- **Yu (Universal Blockchain Framework)**
  - [yu-org/yu](https://github.com/yu-org/yu)
  - A universal blockchain framework implemented purely in Golang. Started in December 2020 and under active development. With this framework, you can:
    1. Customize consensus algorithms (including but not limited to pow/pos/poa/pbft). Currently includes simple pow and hotstuff (still being improved).
    2. Customize on-chain transaction and query logic.
    3. Customize block and transaction validation logic; set rules for packaging transactions from the pool.
    4. Insert custom operations at each stage of block production, including controlling when to execute transactions. This enables features like sharding and DAGs.
  - Motivation: Existing frameworks are either too difficult to get started with or offer limited flexibility for custom development, so I aimed to develop a simple yet highly customizable blockchain framework.
  - Multilingual support is planned. Framework references: tendermint, muta, substrate, xuperchain.
  - [Demo](https://lawliet-chan.github.io/yu.github.io/zh/5.5%E5%BB%BA%E7%AB%8B%E5%8C%BA%E5%9D%97%E9%93%BE%E7%BD%91%E7%BB%9C.html)

### Contributions to Other Open Source Projects

- **Tendermint**
  - [PR #3604](https://github.com/tendermint/tendermint/pull/3604)
  - [PR #3610](https://github.com/tendermint/tendermint/pull/3610)
  - Added boltdb storage to improve random read performance over leveldb.
- **Substrate**
  - [Commit](https://github.com/paritytech/substrate/commit/b7627c4cf8e109dfc80095c5c58f4cf082b56e4d)
  - Optimized `spawn_worker` in offchain-worker using a thread pool.

---

## 💼 Work Experience

**reddio (Dec 2023 – Present)**  
Tech Lead, L2 Parallel EVM Chain
- **Starknet Sequencer:** Built web3 dev team & completed POC + full sequencer functionality using Yu (Dec–Jun). Project halted due to lack of zk prover support from Starkware, then pivoted to L2 parallel EVM chain.
- **Reddio Chain:** Led team to develop and launch L2 EVM on testnet (Jun–Nov). Mainnet launched Dec 2023–May 2025. Achieved up to 13,000 TPS on high-performance machines.

**scroll (Aug 2021 – Nov 2023)**  
Blockchain & Backend Developer  
- Developed scroll’s coordinator-prover system and contributed to early-stage L2 geth development.

**Singapore Foundation (Full year 2020)**  
- **IPSE:**  
  [IPSE Core](https://github.com/Lawliet-Chan/ipse-core) | [IPSE Miner](https://github.com/Lawliet-Chan/ipse-miner)  
  Blockchain storage project using substrate; miners prove storage capacity via PoC, and clients publish storage orders on-chain.
- **IBO:**  
  [IBO Chain](https://github.com/Lawliet-Chan/ibo-chain)  
  A substrate-based decentralized exchange backend, where users can stake tokens for voting on listing/delisting, section changes, etc.—all governed on-chain for transparency and democracy.

**PingCAP (Feb 2019 – Apr 2019)**  
- [Company Website](https://pingcap.com/)  
- Developed TiDB automated performance testing tools (deployment, data import, DB warming, multi-cluster testing).  
- Left to pursue a blockchain career.

**Futurelab (Apr 2018 – Nov 2018)**  
- [Company Website](https://www.futurelab.tv/#/) (acquired)
- Refactored core components, improved logging with Elasticsearch, replaced distributed FS proxies with unified client libraries, increasing security and simplifying backend structure.
- Developed a paid course project on the new infrastructure.
- Left as R&D challenges diminished post-stabilization.

**TalkingData (Mar 2017 – Dec 2017)**  
- [Company Website](http://www.talkingdata.com/)
- Developed a big data collection platform (30–40TB/day) for all business units; maintained over 80 hybrid cloud nodes.
- Built a grey system for data segmentation/copying into test/staging environments.
- Left due to team reorg and lack of new technical challenges.

---

*Feel free to connect!*
