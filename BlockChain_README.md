# BlockChain_Smart_Contracts

### Whitepaper Concepts

- [ ] 1 [**What is BlockChain?** Ref. DEvCon2018](https://www.youtube.com/watch?v=HNCwbKAY7AM) 
> **Open Distribuited Ledger** which is **immutable** . Then what is **Block**? Block is physical space which contains 3 thing **DATA, HASH** and **HASH of previous Block.** **What is Hash?** You can consirder it like fingerprit which is unique all over system.  
- [ ] 2 [What is **Consensus** Algo?](https://channel9.msdn.com/Series/Beginners-Series-to-Blockchain/Consensus-algortihms-10-of-20)
>Search a 64 digit hex work until it's unique in System.
- [ ] 3 [What is **Byzantine's Genral** Problem ?](https://channel9.msdn.com/Series/Beginners-Series-to-Blockchain/Byzantine-Generals-Problem-4-of-20)
>In a Byzantine fault, a component such as a server can inconsistently appear both failed and functioning to failure-detection systems, presenting different symptoms to different observers. It is difficult for the other components to declare it failed and shut it out of the network, because they need to first reach a consensus regarding which component has failed in the first place.
- [ ] 4 [What is **Double Spending** Problem ?](https://channel9.msdn.com/Series/Beginners-Series-to-Blockchain/Double-spending-13-of-20)
>Double Spending problem is repleacating digital currency and assesing it to two owners, if transaction is done with credits it can be reversed, but in case of contracts it may be difficult. Solution are accepting transaction in order the rewarding miners, **Mining Proof of Work**.
- [ ] 5 [What is **Proof of Work vs Proof of Stake** ?](https://www.youtube.com/watch?v=M3EFi_POhps)
> Every miners in network try to find cryptographic key and then first one to find is rewarded, whereas **Proof of Stake**have **Validators** instead of miners who forg blocks. **51 % attack** if person acquires 51% of mining power then they can  approve fake transaction.
- [ ] 6 [**Demo of difficulty level in POW** ](https://github.com/kotharismeet-3/BlockChain_Smart_Contracts/blob/main/18BCE230_Prac3.ipynb)
>Understanding Proof of Work difficulty level. 
- [ ] 7 [**P2P Cash System by Satoshi Nakamoto** ?](https://bitcoin.org/bitcoin.pdf)
>Understanding Network.<br> 1. New transactions are broadcast to all nodes.
> 2. Each node collects new transactions into a block.
> 3. Each node works on finding a difficult proof-of-work for its block.
> 4. When a node finds a proof-of-work, it broadcasts the block to all nodes.
> 5. Nodes accept the block only if all transactions in it are valid and not already spent.
> 6. Nodes express their acceptance of the block by working on creating the next block in the
chain, using the hash of the accepted block as the previous hash.

### Etheruem & Smart Contracts

- [ ] 8 [Understanding **Ethereum**](https://www.youtube.com/watch?v=JD120_jN4ZU)
>Ethereum is open access to digital money and data-friendly services for everyone.Node on ETH Network is machine running on Ethereuem Client.
- [ ] 9 [Proof of Stake](https://www.youtube.com/watch?v=M3EFi_POhps)
- [ ] 10 [Parameters of Eth Transaction]()
> 1. nonce : how many times sender has sent a transaction
> 2. to : address of account this money to going
> 3. value : amount of ether to send to the targeted address
> 4. gasPrice : fee per transaction
> 5. gasLimit : unit of gas transaction can consume
> 6. (v,r,s) : Owner's cryptographic keys
- [ ] 9 [What are **Smart Contracts** ?]()
> A source code to handle contracts. Class is wriiten by developer which has many Instances! 
- [ ] 10 [What is **Solidity** ?](https://www.youtube.com/watch?v=ipwxYa-F1uY)
>Similar maybe to javascript but strongly typed. Solidity Compiler has two parts Byte Code ready for Deployment  as well as Application Binary Interface. ABI works betwwen ByteCode and Javascript.
- [ ] 11 [Ethereum in deep](http://web.archive.org/web/20131228111141/http://vbuterin.com/ethereum.html)

### Architecture

- [ ] 15 [**web3.js and Truffle**]()
>For developers 
- [ ] 16 [**Metamask**]()
> Extension for browsers for client side interface!
- [ ] 17 [**Rinkeby / Rapsten Test Network**]()
> In Manniet Original Money are requierd whereas Rinkeby is testing platform
- [ ] 18 [**Account's Key's**]()
> 1.*Account Adress* :- 
> 2.*Public key* :- 
> 3.*Private Key* :- 
- [ ] 19 [What is SHA256 Hash?](https://blockchaindemo.io)
- [ ] 20 [Javascript Implementation of Bitcoin with difficulty level 1](https://github.com/kotharismeet-3/BlockChain_Smart_Contracts/blob/main/18BCE230_PRAC2.js)
>As data hash changes Nonce tries to match with hash which is also called **mining**.
- [ ] 21 [Total Explanation for Blockchain!](https://andersbrownworth.com/blockchain/)

### Crypto wrt Consensus

- [ ] 22 > [What is Defi](https://www.youtube.com/watch?v=k9HYC0EJU6E)
>New Financial System which are open to everyone and dosen't need any trusting mediocore parties are known as Decentralized Finiancial System.Made up of Cryptography,Blockchain and Smart Contracts. Etheruem is built on language called **Solidity**. **MakerDAO** is DEFI System built in 2015 which uses lock in collateral system produced **DAI**
which is stable coin.
- [ ] 23 > [What is Compound?]()
- [ ] 24 > [Binance](https://www.youtube.com/watch?v=G0gmPW8N88M)
> Delegated PoS :- Top 21 people go for block validation, Low Transaction fees , Canva allowed payment in BNB.
- [ ] 25 > [Tether](https://www.youtube.com/watch?v=cK8bAA6H5PY)
> Bank Run can happen with Tether
- [ ] 26 >  [Solona](https://www.youtube.com/watch?v=1jzROE6EhxM)
> Proof of History - 
- [ ] 27 > [Cardano](https://www.youtube.com/watch?v=UMUztLQNqSI)
> Deflationary compared to ETH
- [ ] 28 > [Polkadot](https://www.youtube.com/watch?v=YlAdEQp6ekM)
> Focuses on Layer 0 

### Designing of BCT Network

- [ ] 29 > [Soft Fork vs Hard Fork](https://www.youtube.com/watch?v=Bu1GcyyFZ7w)
- [ ] 30 > [On-chain Scaling vs Off-chain Scaling and Block Size?](https://www.youtube.com/watch?v=9pJjtEeq-N4)
- [ ] 31 > [Shrading]()
- [ ] 32 > [Sidechain](https://www.youtube.com/watch?v=9pJjtEeq-N4)
- [ ] 33 > [Plasma in ETH]()
- [ ] 34 > [RollUp's](https://www.youtube.com/watch?v=6_nOYsvXMsE)
- [ ] 35 > [Channels]()

### Other Consensus Algo 

- [ ] 36 > [Proof of Elapsed Time]()
- [ ] 37 > [Proof of  Burn]()
- [ ] 38 > [Proof of Capacity]()
- [ ] 39 > [Proof of History] (https://solana.com/solana-whitepaper.pdf)
- [ ] 40 > [Monero](https://www.youtube.com/watch?v=B7sLnmlZ-kU)
> Very Very Private
- [ ] 41 > [Ripple](https://www.youtube.com/watch?v=dlxYUQIMzqo)
> 100 B coins deflationary
- [ ] 42 > [Shibba Inu](https://www.youtube.com/watch?v=jGjmOjD_F-o)
- [ ] 42 > [Polygon Matic](https://www.youtube.com/watch?v=GWUwFDFOipo)
> Layer 2 chain


### Scaling BCT Network

- [ ] 43 > [Casper](https://www.youtube.com/watch?v=GAywmwGToUI)
- [ ] 44 > [Hydra with Cardano](https://iohk.io/en/research/library/papers/hydrafast-isomorphic-state-channels/)

### Defi Knowledge

- [ ] 50 > [Defi](https://www.youtube.com/watch?v=o9ObYRjpIhs)
- [ ] 51 > [Aoutmated Market Maker in Liquidity Pool](https://www.youtube.com/watch?v=1PbZMudPP5E))
- [ ] 52 > [AAVE](https://www.youtube.com/watch?v=dTCwssZ116A)
- [ ] 53 > [Basic Attention Token]()
- [ ] 54 > [UnicakeSwap](https://www.youtube.com/watch?v=DLu35sIqVTM)
- [ ] 55 > [Defi 2.0](Defi 2.0(https://www.youtube.com/watch?v=I34lOvUWsNc)
- [ ] 56 > [DAO](https://www.youtube.com/watch?v=KHm0uUPqmVE)
- [ ] 57 > [OlympusDAO](https://www.youtube.com/watch?v=o699i_l_qy8)

### Wrapped Tokens

- [ ] 58 > [Wrapped Tokens over Solona (ERC1155)](https://www.youtube.com/watch?v=DuwQ6NuPQp4)




