# XinRan Chen （陈昕燃）

 - Male/1994
 - Guangdong University of Petrochemical Tech/  Undergraduate / Food safety major (self study CS)
 - Github: https://github.com/CrocdileChan
 - Phone: +86 13965602037
 - email: crocdilechan@gmail.com
 - Riot: @chenxinran:matrix.org
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

---

# Open Source Projects
## My Projects
- YithQ  
    https://github.com/CrocdileChan/yithQ  
    A distributed MQ:  It's like golang version of Kafka. It use multi partitions per topic to imcrease the throughput. It has a system called Zero to be a role like etcd, 
    it will assign  Topic-Partition to write by message-weight. I design the storage engine so that it can write/read faster than other DBs.
    BUT it still has some bugs and many features to do. In the future, I will use raft or CURP to complete its distributed protocol and integrate etcd/zookeeper.
    
     
    
- qstore  
    https://github.com/CrocdileChan/qstore  
    A high performance Queue storage, it would be faster than LSM-tree database in FIFO scenarios because you can sequential write 
    without Log Compressing and spend O(1) time reading data. 
    You can use it for MQ's storage engine or write-ahead-log.

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
- database: boltdb badger lmdb TiKV rocksdb

---


# My Wish
My work experience is always about Infra or Midware Development, so I'm glad to develop Substrate Modules. such as database, offchain, filesystem and so on.
