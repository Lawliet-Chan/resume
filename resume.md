# Chen Xinran

- Male / Born 1994
- Guangdong University of Petrochemical Technology – Food Safety (Undergraduate, withdrew). Self-taught computer science during university.
- **GitHub:** [Lawliet-Chan](https://github.com/Lawliet-Chan)
- **Phone:** +86 13965602037
- **Email:** crocdilechan@gmail.com
- **WeChat:** chenxinran1228
- **Blog:** https://lawliet-chan.github.io/

---

## 🛠️ Tech Stack

1. Rust & Golang
2. Familiar with the core principles of mainstream public and consortium blockchains (see my universal blockchain framework projects), including consensus mechanisms, state machines, transaction pools, network architecture, and chain structure.
3. Experienced with distributed systems (including distributed message queues, file systems, databases) and storage engines (boltdb, badger).

---

## 🚀 Open Source Projects

### Personal Projects

- **Yu (Universal Blockchain Framework)**
  - [yu-org/yu](https://github.com/yu-org/yu)
  - **Production usage:** Adopted by Reddio and AW-Research, and received grants from Starkware and Nervos.
  - A universal blockchain framework implemented purely in Golang. Started development in December 2020 and is still actively maintained and iterated. With this framework, you can:
    1. Customize consensus algorithms (including but not limited to pow/pos/poa/pbft). Currently includes simple pow and hotstuff (hotstuff is still being improved).
    2. Customize on-chain transaction and query logic.
    3. Customize block and transaction validation logic; set rules for packaging transactions from the pool.
    4. Insert custom operations at each phase of block production, including controlling when transactions within blocks are executed. Enables features like sharding and DAG.
  - Motivation: Existing frameworks either have high barriers to entry or offer limited flexibility for custom development, so I aimed to develop a simple yet highly customizable blockchain framework.
  - Multilingual support is planned. Framework references: tendermint, muta, substrate, xuperchain.
  - [Demo](https://lawliet-chan.github.io/yu.github.io/zh/5.5%E5%BB%BA%E7%AB%8B%E5%8C%BA%E5%9D%97%E9%93%BE%E7%BD%91%E7%BB%9C.html)
  - Draft RIP: [MEVless Protocol](https://ethereum-magicians.org/t/rip-8031-mevless-protocol-the-way-to-anti-mev/25615)

### Contributions to Other Open Source Projects

- **Tendermint**
  - [PR #3604](https://github.com/tendermint/tendermint/pull/3604)
  - [PR #3610](https://github.com/tendermint/tendermint/pull/3610)
  - Provided boltdb integration to extend Tendermint’s underlying storage, improving random read performance over leveldb.
- **Substrate**
  - [Commit](https://github.com/paritytech/substrate/commit/b7627c4cf8e109dfc80095c5c58f4cf082b56e4d)
  - Optimized the `spawn_worker` in offchain-worker using a thread pool.

---

## 💼 Work Experience

**reddio (Dec 2023 – Present)**  
Tech Lead, L2 Parallel EVM Chain
- **Starknet Sequencer:** Built web3 development team, Dec–Jun, used Yu to complete POC and full sequencer functionality. Project halted due to lack of zk prover support from Starkware, then pivoted to L2 parallel EVM public chain.
- **Reddio Chain:** Jun–Nov, led team to develop and launch L2 EVM testnet using Yu; mainnet launched Dec 2023–May 2025. Achieved extreme TPS of up to 13,000 on high-performance machines.

**scroll (Aug 2021 – Nov 2023)**  
Blockchain & Backend Developer  
- Developed scroll’s coordinator-prover system and contributed to early-stage L2 geth development.

**Singapore Foundation (Full year 2020)**  
- **IPSE:**  
  [IPSE Core](https://github.com/Lawliet-Chan/ipse-core) | [IPSE Miner](https://github.com/Lawliet-Chan/ipse-miner)  
  Blockchain storage project using substrate; miners calculate hash submissions based on device storage capacity (similar to BHD’s proof of capacity) for the chain to verify approximate storage capability. Clients publish storage orders to chain and select miners based on on-chain data. Subsequent proof of actual storage was implemented by the foundation’s own R&D team.
- **IBO:**  
  [IBO Chain](https://github.com/Lawliet-Chan/ibo-chain)  
  Decentralized exchange backend service using substrate (akin to DAO). The exchange itself remains centralized, but users can stake tokens for voting rights to propose, audit, and vote on listing/delisting coins, section changes, etc. All steps are governed and executed on-chain. Proposals must pass parliamentary review before entering the democratic vote; parliamentary members are themselves democratically elected. Voting weight is determined by staked token amount and duration. After a vote, results are pushed to the centralized exchange, ensuring transparency and democracy for exchange operations.

**PingCAP (Feb 2019 – Apr 2019)**  
- [Company Website](https://pingcap.com/)  
- Developed TiDB automated performance testing tools (deployment, data import, DB warming, multi-cluster testing).
- Left to pursue a blockchain career.

**Futurelab (Apr 2018 – Nov 2018)**  
- [Company Website](https://www.futurelab.tv/#/) (acquired)
- Refactored core infrastructure components, implemented graded and categorized logging in Elasticsearch for clear debugging, replaced distributed FS/search HTTP proxies with client libraries for unified backend requests. This masked backend details from frontend/mobile, reduced backend complexity, and improved security.
- Developed a paid course project based on the new infrastructure.
- Left as development tasks completed and company entered stable operation phase; R&D team faced no more technical challenges.

**TalkingData (Mar 2017 – Dec 2017)**  
- [Company Website](http://www.talkingdata.com/)
- Developed a big data collection platform (30–40TB/day) for all business units; maintained over 80 hybrid cloud nodes.
- Built a “grey system” for data segmentation/copying into test/staging environments, with rule-based configs effective cluster-wide.
- Left after system stabilized, team was disbanded and merged into BU ops due to departmental restructuring.

---

*Feel free to connect!*
