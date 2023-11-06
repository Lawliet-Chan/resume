# XinRan Chen （陈昕燃）

 - Male/1994
 - Guangdong University of Petrochemical Tech/  Undergraduate / Food safety major (self study CS)
 - Github: https://github.com/Lawliet-Chan
 - Phone: +86 13965602037
 - email: crocdilechan@gmail.com
 - telegram: @ChenXinran
 - wechat: chenxinran1228

---

# Work Experience

## Qiniu （Practice 2016.6 ~ 2016.8 ）
- company link: https://www.qiniu.com/  
#### Big Files Monitor  
This system would check all the files that Qiniu accepts from customs every day. We use every file's MD5 to request for a hash value and check this hash
 with a black/white list. If they hit the black list, we call alarm API. I was in charge of deploy NSQ , develop the base library and alarm service.  
 

## Talkingdata (2017.3 ~ 2017.12)
- company link: http://www.talkingdata.com/  
#### Data Collector  
I joined the development of Data-Collector. All data from outside ( including bussinesses and personnal users) to Talkingdata will be collected by Data Collector. There are about 30-40TB every day  we hold,
 the tps was about 4000-7000 per server.  
#### Gray System
I developed this system based on Data Collector. I use qconf to notify every Data-Collector node reloading config and 
split the online data-flow into gray environment with configured rules.

## Futurelab （ 2018.4 ~ 2018.11 ）
- company link: https://www.futurelab.tv/#/
### Refactor Infrastructure
First, I fixed a bug that always troubled them. The bug is their SeaweedFS lost files sometimes.And then,
I logged in some important operating codes and collect these logs into ES according to different grades 
so that We can clearly debug the online environment.  
I rewrote parts of app backend with golang. I canceled the seaweedFS's and ES's proxys and just 
write a seaweedFS's client library so that all the external HTTP requests cannot directly operate 
the infra systems. Since then, we can safely put the fee videos on it.  
### Online Fee Courses 
I used the new infrastructure , gin web-framwork and gorm to develop the online fee courses. The students need to pay money for their courses. BUT now this module was offline because of copyright.

## PingCAP (2019.2 ~ 2019.4)
- company link: https://pingcap.com/
### Benchmark Tools  
 Developed a tools to bench the performance of TIDB automatically. It Integrated sysbench so that it can auto-sysbench the TiDB cluster. It contains
 deployment, data import, preheating, multi group benchs.


## A foundation in Singapore （2020）

- IPSE
https://github.com/Lawliet-Chan/ipse-core （The main library has been included in their gitlab, this is the backup I left）  
https://github.com/Lawliet-Chan/ipse-miner  
This is a blockchain storage project developed using substrate. The miner (the algorithm is copied from BHD's proof of capacity) calculates the hash based on the device storage capacity and submits it to the chain. The chain needs to verify the hash to verify the miner's approximate storage. ability. The client issues a storage order to the chain and obtains the miner's basic information based on the data on the chain to choose who to use for storage. The follow-up process involves proving whether the miner actually stores the user's data, which will be implemented by the foundation's own R&D team.

- IBO
https://github.com/Lawliet-Chan/ibo-chain （The main library has been included in their gitlab, this is the backup I left）   
This is a decentralized exchange backend service developed using substrate (much like DAO), and the exchange itself is still centralized. However, users can pledge tokens as voting rights to make democratic proposals, reviews, referendums, and final executions on whether a coin should be listed on the exchange, removed from the exchange, switching sections, etc. This series of processes is carried out on the chain, a proposal. It needs to be reviewed by the Congress before it can enter the democratic referendum. The members of Congress themselves are also democratically elected. The voting weight that each citizen can exercise is determined by the number of mortgage tokens and the mortgage period. When the results of the democratic referendum are released, they will be pushed to the central government. in the exchange. This is to ensure the transparency and democratization of currency listing and delisting on digital currency exchanges.

## Scroll (2021.8 ~ 2023.11)
Blockchain infra engineer  
https://github.com/scroll-tech/scroll  
https://github.com/scroll-tech/scroll-prover  
Develop Rollup prover and Coordinator, Zkevm ffi interface.

---  


# Open Source Projects
## My Projects
- Yu (general blockchain framework)  
  https://github.com/yu-org/yu  
  A universal blockchain framework implemented in pure golang. From December 2020 to now, it is still under development and iteration. Using this framework can achieve:  
     1. Custom consensus algorithms (including but not limited to pow/pos/poa/pbft, etc.) currently have built-in simple pow and hotstuff (this part is still being improved)    
     2. Customize the logic of transactions and queries on the chain   
     3. Customize block verification logic, transaction verification logic, and rules for packaging transactions from the transaction pool   
     4. Insert custom actions at various stages of the block generation cycle, including controlling when transactions within a block are executed.
  
  The original intention of developing this project was because we found that existing frameworks either had high barriers to entry or low freedom in customized development, so we wanted to develop a blockchain framework that was easy to get started and highly customizable.  
  running result: https://lawliet-chan.github.io/yu.github.io/zh/5.5%E5%BB%BA%E7%AB%8B%E5%8C%BA%E5%9D%97%E9%93%BE%E7%BD%91%E7%BB%9C.html

## Contributions
- Substrate  
  https://github.com/paritytech/substrate/commit/b7627c4cf8e109dfc80095c5c58f4cf082b56e4d  
  I use ThreadPool to optimize 'spawn_worker' in OffchainWorker so that it can make full use of CPUs.

- Tendermint  
   https://github.com/tendermint/tendermint/pull/3604  
   https://github.com/tendermint/tendermint/pull/3610  
   I provided boltdb to expand Tendermint's db-engine so that it can support better performance for random reading than levelDB.
( Ironically, the Tendermint's developer just closed my PR and copied my codes into their PR. And then, they just don't put my githubID into their Contributors-List. What an open-source-spirit !)

---

# Skills

- language: golang / rust / java
- distributed-systems: distributed theory. kafka  NSQ seaweedfs 2pc raft and so on.
- database: boltdb badger  TiKV rocksdb

---


# My Wish
My work experience is always about Infra or Midware Development, so I'm glad to develop Substrate Modules. such as database, offchain, filesystem and so on.
