# XinRan Chen

- Github: https://github.com/Lawliet-Chan
- Blog: https://lawliet-chan.github.io/

---

## Ethereum Ecosystem Contributions

- **EIP-8099**: https://github.com/ethereum/EIPs/blob/master/EIPS/eip-8099.md

---

## Work Experience

#### reddio (2023.12 ~ Present)

L2 Parallel EVM Chain Tech Lead

- **Starknet Sequencer**

  Built the web3 development team. Dec ~ Jun: used Yu to complete POC + full sequencer development. Later pivoted to L2 parallel EVM public chain due to Starkware's delayed zk prover support.

  https://github.com/reddio-com/itachi

- **Reddio Chain**

  Jun ~ end of Nov: led team using Yu to complete L2 EVM development and launch testnet. Dec ~ May 2025: launched mainnet. Extreme TPS reaches 13,000 on high-performance machines.

  https://github.com/reddio-com/reddio

#### scroll (2021.8 ~ 2023.11)

Blockchain Development & Backend Development

Participated in developing scroll's coordinator-prover system and early-stage L2 geth secondary development.

https://github.com/scroll-tech/scroll
https://github.com/scroll-tech/scroll-prover
https://github.com/privacy-ethereum/zkevm-circuits

#### A Foundation in Singapore (Full year 2020)

- **IPSE** — Storage Public Chain

  https://github.com/Lawliet-Chan/ipse-core (backup; main repo moved to their GitLab)
  https://github.com/Lawliet-Chan/ipse-miner

  A Substrate-based storage public chain. Miners submit hashes based on storage capacity (BHD proof-of-capacity algorithm) for on-chain verification. Clients publish storage orders and select miners via on-chain data.

- **IBO**

  https://github.com/Lawliet-Chan/ibo-chain (backup; main repo moved to their GitLab)

  A Substrate-based decentralized exchange governance backend (DAO-like). On-chain democratic mechanisms (staking-based voting, congressional review, public referendum) govern coin listing/delisting decisions.

#### PingCAP (2019.2 ~ 2019.4)

https://pingcap.com/

Developed TiDB automated performance testing tools: automatic deployment, data import, database warm-up, and multi-cluster testing.

#### futurelab (2018.4 ~ 2018.11)

https://www.futurelab.tv/#/ (acquired)

- **Infrastructure Refactoring**: Classified logs into Elasticsearch, replaced HTTP proxies with a distributed file system client library, reducing backend complexity and improving security.

- **Paid Course Development**: Developed a paid course system on top of the refactored infrastructure.

#### Talkingdata (2017.3 ~ 2017.12)

http://www.talkingdata.com/

- **Big Data Collection Platform**: 30–40TB daily ingestion, maintained 80+ hybrid cloud nodes at peak. Handled compression, persistence, and topic-based distribution to business lines with one-week data traceability.

- **Gray System**: Built on top of the collection platform; splits/replicates live data flows to gray or test environments based on configurable rules.

---

## Open Source Projects

#### Personal Projects

- **Yu (Universal Blockchain Framework)**

  https://github.com/yu-org/yu

  **Deployed in production (reddio and AW-Research); received grants from Starkware and Nervos**

  A pure-Go universal blockchain framework under continuous development since December 2020. Features: customizable consensus (PoW/PoS/PoA/PBFT, built-in simple PoW and HotStuff), custom on-chain transaction/query logic, modular components with dependency injection, custom block/transaction validation, and hooks at all block lifecycle stages (enabling sharding and DAG). References: Tendermint, Muta, Substrate, XuperChain.

#### Open Source Contributions

- **zkevm-circuits** — Early contributor to the Ethereum Foundation's zkEVM project

  https://github.com/privacy-ethereum/zkevm-circuits

- **Tendermint** — Added boltdb storage backend for better random-read performance

  https://github.com/tendermint/tendermint/pull/3604
  https://github.com/tendermint/tendermint/pull/3610

- **Substrate** — Optimized `spawn_worker` in offchain-worker using thread pools

  https://github.com/paritytech/substrate/commit/b7627c4cf8e109dfc80095c5c58f4cf082b56e4d

---

## Published Articles

Web3Caff Column: https://web3caff.com/archives/author/weiwenhou

- [The Difficulty of Delay Encryption Against MEV](https://web3caff.com/archives/130787)
- [Rust Is Not the Most Suitable Language for Blockchain Development](https://web3caff.com/archives/130784)
- [PBS: Ethereum's Thorn-Carved Monkey](https://web3caff.com/archives/130780)
- [MEVless: The Way to Solve MEV](https://web3caff.com/archives/130463)
- [ReStake: Ethereum's Death Knell](https://web3caff.com/archives/130457)
- [Blockchain Layering: We Need Our Own Consensus](https://web3caff.com/archives/130467)
- [Blockchain Layering: A New Beginning](https://web3caff.com/archives/130460)
- [All BFT Consensus Is a Consortium Chain](https://web3caff.com/archives/130391)
- [Chain-Native vs. Chain-Extension](https://web3caff.com/archives/129909)

---

## Education

Guangdong University of Petrochemical Technology — Food Safety, dropped out of undergraduate program

Self-taught computer science during university
