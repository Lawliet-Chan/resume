# XinRan Chen

 - Male/1994
 - Guangdong University of Petrochemical Technology - Food Safety major, dropped out of undergraduate program. Self-taught computer science during university.
 - Github: https://github.com/Lawliet-Chan
 - Phone: +86 13965602037
 - email: crocdilechan@gmail.com
 - wechat: chenxinran1228
 - blog: https://lawliet-chan.github.io/
 
### Tech Stack
1. rust + golang  
2. Familiar with the underlying principles of mainstream public chains and consortium chains (see my universal blockchain framework), including consensus mechanisms, state machines, transaction pools, networking, chain structures, etc.  
3. Familiar with distributed systems (including distributed message queues, distributed file systems, distributed databases) and storage engines (boltdb, badger)

# Open Source Projects
### My Personal Projects
- Yu (Universal Blockchain Framework)   
 https://github.com/yu-org/yu  
 **Already deployed in production (reddio and AW-Research), and received grants from Starkware and Nervos**   
 A universal blockchain framework implemented in pure golang. Development started in December 2020 and is still ongoing. Using this framework, you can:  
   1. Customize consensus algorithms (including but not limited to PoW/PoS/PoA/PBFT, etc.). Currently built-in simple PoW and HotStuff (this part is still being improved).  
   2. Customize on-chain transaction and query logic, as well as transaction pool related operations
   3. Component modularization, and all components support dependency injection
   4. Customize block validation logic, transaction validation logic, and rules for packaging transactions from the transaction pool  
   5. Insert custom operations at various stages of the block generation cycle, including controlling when to execute transactions in blocks. Can be used to implement sharding and DAG.  
   
  The original intention of developing this project was to address the fact that existing frameworks either have high learning curves or low freedom for customized development. I wanted to create a blockchain framework that is easy to get started with and highly customizable.  
 In the future, it will support multi-language development. This framework references Tendermint, Muta, Substrate, and XuperChain.   
 Demo: https://lawliet-chan.github.io/yu.github.io/zh/5.5%E5%BB%BA%E7%AB%8B%E5%8C%BA%E5%9D%97%E9%93%BE%E7%BD%91%E7%BB%9C.html   

### Ethereum ecosystem contributions
- draft EIP: https://github.com/ethereum/EIPs/pull/10855
- draft RIP: https://ethereum-magicians.org/t/rip-8031-mevless-protocol-the-way-to-anti-mev/25615


## Code Contributions to Open Source Projects
- zkevm-circuit
  https://github.com/privacy-ethereum/zkevm-circuits  
  Early contributor to the Ethereum Foundation's zkEVM project
- Tendermint  
   https://github.com/tendermint/tendermint/pull/3604  
   https://github.com/tendermint/tendermint/pull/3610  
   I provided boltdb to extend Tendermint's underlying storage so it can achieve higher performance than leveldb in random read scenarios.
- Substrate  
  https://github.com/paritytech/substrate/commit/b7627c4cf8e109dfc80095c5c58f4cf082b56e4d  
  Optimized 'spawn_worker' in offchain-worker using thread pools. 
---  

## Work Experience  

#### reddio (2023.12 ~ Present)
L2 Parallel EVM Chain Tech Lead
- starknet sequencer  
  Built web3 development team, December ~ June, used Yu to complete POC + full sequencer functionality development. Later, due to Starkware's delay in providing zk prover support, the project was forced to halt and pivot to L2 parallel EVM public chain.
  https://github.com/reddio-com/itachi   
- Reddio Chain  
  June ~ end of November, used Yu to lead the team to complete L2 EVM development and launch testnet. December ~ May 2025 launched mainnet. On high-performance machines, extreme TPS can reach 13,000.   
  https://github.com/reddio-com/reddio
#### scroll (2021.8 ~ 2023.11)
Blockchain Development & Backend Development
Participated in developing scroll's coordinator-prover system, and participated in early-stage L2 geth secondary development.    
https://github.com/scroll-tech/scroll   
https://github.com/scroll-tech/scroll-prover   
https://github.com/privacy-ethereum/zkevm-circuits   

#### A Foundation in Singapore (Full year 2020)  
- IPSE   
https://github.com/Lawliet-Chan/ipse-core  (The main repository has been moved to their GitLab, this is my backup)  
https://github.com/Lawliet-Chan/ipse-miner    
This is a blockchain storage project developed using Substrate. Miners (the algorithm is copied from BHD's proof of capacity) calculate hashes based on device storage capacity and submit them to the chain. The chain needs to verify these hashes to validate the miner's approximate storage capacity. Clients publish storage orders to the chain and select miners based on on-chain data. The subsequent proof of whether miners actually stored user data was implemented by the foundation's own R&D team.   
- IBO  
 https://github.com/Lawliet-Chan/ibo-chain (The main repository has been moved to their GitLab, this is my backup)  
 This is a decentralized exchange backend service (very similar to DAO) developed using Substrate. The exchange itself remains centralized. However, users can stake tokens as voting rights to democratically propose, review, vote, and execute actions such as listing coins, delisting coins, switching sections, etc. This entire process takes place on-chain. A proposal must pass congressional review before entering democratic voting. Congress members are also democratically elected. The voting weight each citizen can exercise is determined by the amount and duration of staked tokens. When democratic voting produces results, they are uniformly pushed to the centralized exchange. This ensures transparency and democratization of actions such as listing and delisting digital currencies on cryptocurrency exchanges.    

#### PingCAP (2019.2 ~ 2019.4)
Company website: https://pingcap.com/  
Developed TiDB automated performance testing tools, including automatic deployment, data import, database preheating, and multi-cluster testing.  
Reason for leaving: Preparing to work in the blockchain industry.

#### futurelab (2018.4 ~ 2018.11)   
Company website: https://www.futurelab.tv/#/ (The company has been acquired)   
- Refactoring Infrastructure  
Refactored code for some basic components, classified logs by level and stored them in Elasticsearch with indexing to distinguish between human operations and bugs, preserving a clean online environment for debugging. Removed HTTP proxies for the backend distributed file system and search system, and developed a client library for the distributed file system so that all operations on the distributed file system and search system are uniformly sent from the backend business system, rather than directly accessing infrastructure via HTTP from external sources. This refactoring layer shields frontend and mobile clients from backend business details, reduces the complexity of the backend system structure, and improves security to some extent, preventing some paid static resources from being browsed arbitrarily.
- Developing Paid Courses  
Developed a paid course project based on the newly refactored infrastructure.

Reason for leaving: Development tasks were basically completed, and the company entered a stable operation phase. The R&D team no longer had challenging tasks.

#### Talkingdata (2017.3 ~ 2017.12)  
Company website: http://www.talkingdata.com/ 
- Big Data Collection Platform  
Participated in developing the big data collection platform. All external data that needs to be integrated into the company must go through this platform, which serves as the entry point connecting all business departments. The platform needs to compress external data, persist it, distribute data to various business department product lines by topic combination, and ensure data traceability within one week.
The platform's daily data collection volume is 30-40TB, and at peak times the team needed to maintain over 80 hybrid cloud nodes.
- Gray System   
A gray system developed based on the big data collection platform, which splits or replicates online data flows to gray environments or test environments for use. Business departments can configure their own online data for splitting or replication according to their needs. The rules for splitting and replicating data are pushed to the data collection platform cluster to take effect.

Reason for leaving: The system was running stably with no iteration needs. The department's organizational structure was adjusted, and my team was disbanded and merged into various BU operations. The work no longer had challenges.
