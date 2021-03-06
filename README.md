# Love-Ethereum

----------------------------------------------------------------------------------------

<img width="300" height="100" src="https://github.com/xianfeng92/Love-Ethereum/blob/master/icons/horzlogo.png"/>

----------------------------------------------------------------------------------------

| [版本说明](#版本说明) | [以太坊开发基础](#以太坊开发基础) | [以太坊相关研究](#以太坊相关研究) | [以太坊源码的分析](#以太坊源码的分析) | [区块链开源学习项目](#区块链开源学习项目) | [补充资料](#补充资料)| [参与贡献](#参与贡献)
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
------------------------------------------------------------------------------------------------------

# Progress

![Progress](http://progressed.io/bar/19)

-----------------------

# 版本说明

* [Frontier](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Frontier.md)

  简单的介绍区块链基础知识，通过阅读此版本可以对区块链技术有个初步的认知。
  
* [Homestead](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Homestead.md)

  介绍以太坊项目，并对涉及到的区块链核心技术点进行介绍和分析。

* [Metropolis](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Metropolis.md)

  该本版主要是关于智能合约和Dapp
  
* [Serenlity](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Serenlity.md)
  
  以太坊源码分析

-------------------------------------------------------------------------------------------

# 以太坊开发基础

## 以太坊私有链上测试和部署一些经典的智能合约

### Solidity

* [Solidity官方文档翻译](https://github.com/xianfeng92/Solidity-Docs)

### Web3 Api

* [Web3 Api](https://github.com/xianfeng92/Web3js-Doc)

### 经典的智能合约案例

* 基于区块链的投票　－－Ballot
* 盲拍 -- Blind Auction
* 权限控制　－－　AccessControl

### 智能合约设计模式

* CD（Controller-Data）模式

### Dapp

* [NBASTAR](https://github.com/xianfeng92/NBASTAR)

* [dog-shop](https://github.com/xianfeng92/dog-shop)


### Dapp开发利器－Truffle

* [Truffle技术文档翻译](https://github.com/xianfeng92/Truffle-Docs)


 [点击直达](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Metropolis.md)
 
--------------------------------------------------------------------------------------------------------------

## P2P网络

-----------------------------------------------------------------------------------------------------------

## 可信之石(共识算法)

在一个分布式系统中，如何保证集群中所有节点中的数据完全相同并且能够对某个提案（Proposal）达成一致是分布式系统正常工作的核心问题，而共识算法就是用来保证分布式系统一致性的方法。无论是 Bitcoin、Ethereum 还是 EOS，作为一个分布式网络，首先需要解决分布式一致性的问题，也就是所有的节点如何对同一个提案或者值达成共识，这一问题在一个所有节点都是可以被信任的分布式集群中都是一个比较难以解决的问题，更不用说存在拜占庭节点的区块链网络中了。


* [共识算法介绍](https://github.com/xianfeng92/Love-Ethereum/blob/master/DistributedSystem/consensus.md)

* [Paxos](https://github.com/xianfeng92/Love-Ethereum/blob/master/DistributedSystem/paxos.md)

* [PBFT](https://github.com/xianfeng92/Love-Ethereum/blob/master/DistributedSystem/pbft.md)

* [Proof of Stake FAQs](https://github.com/ethereum/wiki/wiki/Proof-of-Stake-FAQs)

* [V神实现的99%容错算法](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/99fault.py)


-------------------------------------------------------------------------------------------------------------

# 以太坊相关研究

## Sharding

以太坊仍处于初级阶段。现在，它不具备安全性和可扩展性。以太坊和web3期望建设的——一个安全、易用、由一套共同的经济协议约束、可供数十亿人使用的分布式互联网，仍处于发展阶段，直到关键基础设施建成之后才能实现。致力于构建此 __基础架构__ 并扩大以太坊容量的项目通常称为扩容方案。

* [Sharding FAQ 英文版](https://github.com/ethereum/wiki/wiki/Sharding-FAQs)

* [Sharding FAQ 中文版](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/ShardingFAQ.md)


## Cross-Shard

### [几种跨分片的方案](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/%E5%87%A0%E7%A7%8D%E8%B7%A8%E5%88%86%E7%89%87%E7%9A%84%E6%96%B9%E6%A1%88.md)

--------------------------------------------------------------------------------------------------------------------------

关于跨分片解决方案之一拜占庭原子提交的讨论，多分片问题最理想的解决方案可能就是归并成单分片处理。如果每个"交易状态都涉及到多分片"那将严重影响分片的性能，所以分片以后的重点问题可能就是处理应用和分片的关系。

* [Sharded Byzantine Atomic Commit](https://ethresear.ch/t/sharded-byzantine-atomic-commit/1285)

--------------------------------------------------------------------------------------------------------------------------

以太坊的一个跨分片的解决方案，方案核心就是多分片的单分片的处理方式，在EVM级别处理，可能比其他方案相对“简单”。

* [Cross-shard contract yanking](https://ethresear.ch/t/cross-shard-contract-yanking/1450)

--------------------------------------------------------------------------------------------------------------------------

* [Cross-links between main chain and shards](https://ethresear.ch/t/cross-links-between-main-chain-and-shards/1860)

* [Cross Shard Locking Scheme](https://ethresear.ch/t/cross-shard-locking-scheme-1/1269/25)

 
### Casper

### Plasma

* [Minimal Viable Plasma](https://ethresear.ch/t/minimal-viable-plasma/426)
* [Plasma Whitepaper](https://plasma.io)

### Economics

### Ecosystem

* [Women in Blockchain Series](https://medium.com/@Melt_Dem)
* [Where Can I Join The Ethereum Community?
](https://medium.com/blockchannel/where-can-i-join-the-ethereum-community-3aa5c795b1e5
)
* [State of the Dapps
](http://dapps.ethercasts.com/
)
* [Ethereum Business Directory
](http://ethereumall.com/business-directory/page/9/?wpbdp_view=all_listings
)

### Applications
-----------------------------------------------------------------------

## Gas

* [Calculating Costs in Ethereum Contracts](https://hackernoon.com/ether-purchase-power-df40a38c5a2f)
* [Gas 计算源码](https://github.com/xianfeng92/ethereum-code-analysis/blob/master/notes/gas.md)

------------------------------------------------------------------------------------------------------------

# 以太坊源码的分析

* 目前主要是阅读一些以太坊源码解读的文章

下面的文章主要是CSDN上的一个teaspring的技术专栏里面关于以太坊源代码分析的文章，文章写的超级好，强烈推荐！

* [区块和交易，合约和虚拟机](https://blog.csdn.net/teaspring/article/details/75389151)
* [数据的呈现和组织，缓存和更新](https://blog.csdn.net/teaspring/article/details/75390210)
* [挖矿和共识算法的奥秘](https://blog.csdn.net/teaspring/article/details/78050274)
* [Clique共识算法](https://ethfans.org/posts/Clique-Consensus-Algorithm)
* [ 椭圆曲线密码学和以太坊中的椭圆曲线数字签名算法应用](https://blog.csdn.net/teaspring/article/details/77834360)
* [从钱包到客户端](https://blog.csdn.net/teaspring/article/details/78350888)

## 源码分析

从源码上去分析以太坊上 tx 的执行，节点通信以及数据存储的具体流程和实现细节。

## 节点中tx

* [tx_contract](https://github.com/xianfeng92/ethereum-code-analysis/blob/master/articles/tx_contract.md)

* [tx_process](https://github.com/xianfeng92/ethereum-code-analysis/blob/master/articles/tx_process.md)

* [tx_consensus](https://github.com/xianfeng92/ethereum-code-analysis/blob/master/articles/tx_consensus.md)


 [点击直达](https://github.com/xianfeng92/Love-Ethereum/blob/master/version/Serenlity.md)
 
### [源码分析](https://github.com/xianfeng92/ethereum-code-analysis)

-------------------------------------------------------------------------------------------

# IPFS

星际文件系统IPFS（InterPlanetary File System）是一个面向全球的、点对点的分布式版本文件系统，目标是为了补充（甚至是取代）目前统治互联网的超文本传输协议（HTTP），将所有具有相同文件系统的计算设备连接在一起。

* [IPFS基本介绍](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/IPFS.md)
* [IPFS基本操作](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/IPFSCommand.md)
* [IPFS项目中的使用](https://github.com/xianfeng92/Love-Ethereum/blob/master/notes/IPFSBlockchain.md)
* [IPFS + 区块链 系列](https://github.com/xianfeng92/IPFS-Ethereum-Image)
* [IPFS 筆記和教學](https://github.com/miaoski/ipfs-tutorial)


## Vickrey auction

* [Vickreyauction](https://github.com/xianfeng92/Love-Ethereum/tree/master/Vickreyauction)

-----------------------------------------------------------------------------------------------

# 区块链开源学习项目

* [Mastering Bitcoin(精通比特币—英文版)](https://github.com/bitcoinbook/bitcoinbook)
* [Mastering Ethereum(精通以太坊－英文版)](https://github.com/ethereumbook/ethereumbook)
* [Blockchain Tutorial](https://github.com/liuchengxu/blockchain-tutorial)
* [blockchain_demo](https://github.com/seanjameshan/blockchain) ---区块链的演示
* [blockchain_guide](https://github.com/yeasy/blockchain_guide)
* [awesome-blockchain](https://github.com/dily3825002/awesome-blockchain) -- 区块链白皮书、书籍、交易所、币种、自媒体等资源汇总
* [ethereumjs-tx](https://github.com/ethereumjs/ethereumjs-tx) -- A simple module for creating, manipulating and signing ethereum transactions
* [EthList](https://github.com/Scanate/EthList) EthList: The Crowdsourced Ethereum Reading List

--------------------------------------------------------------------------------------------------------------------


# 补充资料

这部分资料没有阅读和学习过,后面学习中可能有用.

#### [区块链入门](https://liuchengxu.gitbook.io/blockchain)

--------------------------------------------------------------------------

## Some vedio about Ethereum

* [thereum the world computer](https://www.youtube.com/watch?v=j23HnORQXvs)

* [italik Buterin explains Ethereum](https://www.youtube.com/watch?v=TDGq4aeevgY)

* [BBC explains Ethereum](https://www.youtube.com/watch?v=0X33lgMbvdI)

* [Techcrunch on Ethereum](https://www.youtube.com/watch?v=WfULutvxvzY)

* [Vitalik Buterin's Ethereum introduction at Devcon 1](https://www.youtube.com/watch?v=gjwr-7PgpN8)

*  [Devcon 0 (Berlin, 2014) talks and videos](https://www.youtube.com/watch?v=_BvvUlKDqp0&amp;list=PLJqWcTqh_zKEjpSej3ddtDOKPRGl_7MhS)

*  [Devcon 1 (London, 2015) talks and videos](https://www.youtube.com/watch?v=BUARih8_f68&list=PLJqWcTqh_zKHQUFX4IaVjWjfT2tbS4NVk)

*  [Devcon 2 (Shanghai, 2016) talks and videos](https://www.youtube.com/watch?v=1wayaZ1-iBE&list=PLaM7G4Llrb7xqzgOwbvNv63_KM7VH84Rd)

* [Devcon 3 (Cancún, 2017) talks and videos](https://www.youtube.com/channel/UCNOfzGXD_C9YMYmnefmPH0g/playlists)

## Wallet

- [My Ether Wallet](https://myetherwallet.com) 网页版以太坊钱包 [源码](https://github.com/kvhnuke/etherwallet)
- [MetaMask](https://metamask.io/) Chrome Extension浏览器插件版
- [Multi-platform Jaxx Wallet](https://jaxx.io/) 同时兼容比特币钱包
- [Mist Wallet](https://github.com/ethereum/mist/releases/latest) 官方版钱包
- [Parity Wallet](https://github.com/paritytech/parity/releases/latest)
- [Harmony Wallet](https://github.com/ether-camp/ethereum-harmony/releases/latest)
- [imToken](https://token.im/) 移动App版钱包
- [Ledger Nano S](https://theethereum.wiki/w/index.php/Ledger_Nano_S) 硬件钱包
- [Trezor](https://blog.trezor.io/trezor-integration-with-myetherwallet-3e217a652e08) 硬件钱包

## Development Videos

* [Building Ethereum DApps using Solidity](https://www.youtube.com/watch?v=9_coM_g7Dbg&list=PLH4m2oS2ratdoHFEkGvwvd7TkeTv4sa7Z)
* [Devcon 0 (Berlin, 2014) talks and videos](https://www.youtube.com/watch?v=_BvvUlKDqp0&amp;list=PLJqWcTqh_zKEjpSej3ddtDOKPRGl_7MhS)
* [Devcon 1 (London, 2015) talks and videos](https://www.youtube.com/watch?v=BUARih8_f68&list=PLJqWcTqh_zKHQUFX4IaVjWjfT2tbS4NVk)
* [Devcon 2 (Shanghai, 2016) talks and videos](https://www.youtube.com/watch?v=1wayaZ1-iBE&list=PLaM7G4Llrb7xqzgOwbvNv63_KM7VH84Rd)
* [**Devcon 3** (Cancún, 2017) website and registration](http://ethereumfoundation.org/devcon3/)


## Explorer

- [Etherscan](https://etherscan.io) 以太坊区块链浏览器
- [Ethplorer](https://ethplorer.io) 以太坊区块链浏览器，提供API调用
- [Eth Gas Station](https://ethgasstation.info/index.php) 以太坊Gas目前定价

## Documents

- [Mastering Ethereum](https://github.com/ethereumbook/ethereumbook) 精通以太坊开发Oreilly开源书
- [Solidity语言文档](http://www.tryblockchain.org/) 语言中文手册
- [Web3.JS接口文档](http://web3.tryblockchain.org/) 接口中文手册
- [Truffle框架文档](http://truffle.tryblockchain.org/) 框架中文手册
- [Open Zeppelin框架文档](http://zeppelin.tryblockchain.org/)
- [Ethplorer接口](https://github.com/EverexIO/Ethplorer/wiki/Ethplorer-API?from=etop) Ethplorer接口文档

## SDK

- [Truffle](https://github.com/trufflesuite/truffle) 以太坊Dapp开发脚手架
- [Cakeshop](https://github.com/jpmorganchase/cakeshop) 来自JP Morgan的以太坊可视化管理工具
- [Zeppelin](https://github.com/OpenZeppelin/zeppelin-solidity) 用于编写安全的以太坊合约框架
- [Web3j](https://github.com/web3j/web3j) 以太坊官方轻量级java SDK


## YouTube Channels
- [Crypt0's News - Daily Video Blog](https://www.youtube.com/user/obham001/videos)
- [Ameer Rosic](https://www.youtube.com/user/AmeerRosic/videos)
- [Decypher Media](https://www.youtube.com/channel/UC8CB0ZkvogP7tnCTDR-zV7g)
- [Ivan on Tech](https://www.youtube.com/c/IvanOnTech)

----------------------------------------------------------------------------------------------------------------------

# 参与贡献

区块链技术自身仍在快速发展中，生态环境也在蓬勃成长。欢迎 [参与维护项目](https://github.com/xianfeng92/Love-Ethereum/blob/master/contribute.md)。

-----------------------------------------------------------------------------------------------------------















