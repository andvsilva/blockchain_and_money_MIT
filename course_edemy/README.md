# Blockchain A-Z: Learn to Build your own Blockchain

### About this course

Harness the power of the most disruptive technology since the internet 
through real life examples! Master Blockchain Now!

### What you’ll learn
- Why this is important
- Understand the theory behind Blockchain
- Create a Blockchain
- Understand the theory behind Cryptocurrency's
- Understand the theory behind Cryptocurrency Transactions
- Create their own currency
- Understand the theory behind Smart Contracts
- Create their own Smart Contracts

### Are there any course requirements or prerequisites?
- Just some high school mathematics level
- To take and complete practical part of the course basic Python knowledge required

###  Who this course is for:
- Any students in college who want to start a career in Blockchain &Cryptos
- Any Blockchain, Bitcoin & Cryptos enthusiast
- Anyone interested in building their own Blockchain
- Anyone interested in Blockchain and its applications
## Table of Contents

### Blockchain intuition
- What is a blockchain?
- Understanding SHA256 Hash
- Immutable Ledger
- Distributed P2P Network
- How Mining Work: The Nonce
- How Mining Work: The Cryptographic Puzzle
- Byzantine Fault Tolerance
- Consensus Protocol: Defense Against Attackers
- Consensus Protocol: Proof-of-Work (PoW)
- Blockchain demo

### Quiz:

  - Which of these statements is correct?
    - [x] A blockchain is a decentralized ledger which is continuously growing. 
  - Which of the following is not a requirement for Hash algorithms:
    - [x] A hash algorithm has to be only one-way (cannot be reverse-engineered)
    - [x] A hash algorithm has to be deterministic (same input generates same output every time).
    - [x] A hash algorithm has to have the Avalanche effect(any minor change to inputs changes the output completely and unpredictably)
- How does the "Distributed P2P Network" property of Blockchain enhance the security of this technology?
  - [x] Every participant of the network has a copy of the full blockchain and participants are synced up. Therefore, if an attacker modifies the blockchain on one of the computers in the network, they are modifying only one simple copy of the blockchain. The network will see this, compare it to prevailing majority of versions of the blockchain in the network and very quickly override the fraudulent version.
- Which of these is an accurate description of what Bitcoin mining is?
  - [x] Mining is all about finding a ```Nonce``` value which willl generate a Hash value below a certain target threshold set by the bitcoin network.
- What is a Consensus Protocol?
  - [x] A Consensus Protocol is a process used process to achieve agreement between participants of a distributed network.

### Create a Blockchain

See the source code in python:
  - [x] [blockchain.py](/course_edemy/blockchain/blockchain.py)

#### Run

```bash
~/repo/blockchain_and_money_MIT/course_edemy/blockchain on  master! ⌚ 12:05:41
$ python blockchain.py
 * Running on all addresses.
   WARNING: This is a development server. Do not use it in a production deployment.
 * Running on http://XXXXXXXXX:5000/ (Press CTRL+C to quit)
XXXXXXXXX - - [03/Oct/2021 12:05:48] "GET /get_chain HTTP/1.1" 200 -
```

### Postman

```bash
# to install postman
$ sudo snap install postman

$ postman
```

### Get chain: Genesis Block

![Postman](/course_edemy/picture/genesis_block.png)


### Mined a Block
![Postman](/course_edemy/picture/mine_block.png)

```bash
$ python blockchain.py
 * Running on all addresses.
   WARNING: This is a development server. Do not use it in a production deployment.
 * Running on http://XXXXXXXXX:5000/ (Press CTRL+C to quit)
XXXXXXXXX - - [03/Oct/2021 12:05:48] "GET /get_chain HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:17:59] "GET /mine_block HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:21:26] "GET /get_chain HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:22:18] "GET /mine_block HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:22:22] "GET /mine_block HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:22:26] "GET /mine_block HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:22:27] "GET /mine_block HTTP/1.1" 200 -
XXXXXXXXX - - [03/Oct/2021 12:22:41] "GET /get_chain HTTP/1.1" 200 -
```

### Mining some Blocks

```bash
{
    "chain": [
        {
            "index": 1,
            "previous_hash": "0",
            "proof": 1,
            "timestamp": "2021-10-03 12:05:43.845840"
        },
        {
            "index": 2,
            "previous_hash": "e4abf40c012d738ae8d8908e2431f1954fd9ddadeb62368b5e0d18c74fdb9005",
            "proof": 533,
            "timestamp": "2021-10-03 12:17:59.016593"
        },
        {
            "index": 3,
            "previous_hash": "3a99a684da7d4a67603fce758e5cc3606588e93b9529878206662f5205e078c4",
            "proof": 45293,
            "timestamp": "2021-10-03 12:22:18.702784"
        },
        {
            "index": 4,
            "previous_hash": "57720be8cf1fe9b74a49ceaf4c4564ff7838f718b5c0ffaa681dc3a01be18af8",
            "proof": 21391,
            "timestamp": "2021-10-03 12:22:22.569101"
        },
        {
            "index": 5,
            "previous_hash": "bf494782ac47d89fe2ddd0b8ef9e4777e764a77decca4c0923071d4fbc7493c8",
            "proof": 8018,
            "timestamp": "2021-10-03 12:22:26.418960"
        },
        {
            "index": 6,
            "previous_hash": "e8e942302398ff49d8aadfa382ba9760d957ced792e74d305e2327f2b39ad24c",
            "proof": 48191,
            "timestamp": "2021-10-03 12:22:27.671972"
        }
    ],
    "length": 6
}
```

### Welcome to Part 2 - Cryptocurrency
### Welcome to Part 2!

In this Part you will:

Build up a solid Cryptocurrency Intuition
Reinforce this Intuition by understanding in depth Cryptocurrencies transactions

Learn how to create a Cryptocurrency from scratch
Enjoy!

### Cryptocurrency intuition

- What is Bitcoin?
- Bitcoin's Monetary Policy
- Understanding Mining Difficulty
- Virtual tour of a Bitcoin Mine
- Mining Pools
- Nonce Range
- How Miner Pick Transactions (Part 1)
- How Miner Pick Transactions (Part 2)
- CPU's vs GPU's vs ASIC's
- How do Menpools?
- Orphaned Blocks
- The 51% Attack
- Extra: Bits to Target conversion
- Quiz 2: Cryptocurrency intuition

### Quiz:

- In which order (from top to bottom) do the three layers of Blockchain go?
  - [x] 1 - Technology(Blockchain), 
  - [x] 2 - Protocol/Coin (e.g. Bitcoin, Ethereum) and 
  - [x] 3 - Token (e.g. Power Ledger).
- What is the maximum number of Bitcoins that will ever be in circulation and when will this happen?
  - [x] 21 Million Bitcoins by 2140.
- Assuming that the current mining difficulty requires 18 leading zeros for a hash to be vaild, what is the probability that a hash selected at random will be valid?
  - [x] 0.00000000000000000002%
- What is a Mempool?
  - [x] A Mempool is a storage area where transactions are stored before they are added to a block. Every participant of the P2P distributed network has their own menpool on their computer.
- What is the 51% attack and how do the attackers benefit from it?
  - [x] The 51% attack is when a group of hidden participants with majority computational power conduct mining without announcing their version of the chain to the rest of the network. The attackers can benefit by leveraging the double-spend problem.

### Cryptocurrency Transactions Intuition

- Transactions and UTXO'S
- Where do transaction fees come from?
- How wallets work
- Signatures: Private & Public Keys
- Signatures & Keys Demo
- What is Segregated Witness (SegWit)
- Public Key and Bitcoin Address
- Hierarchically Deterministic (HD) Wallets
- Quiz 3: Cryptocurrency Transactions Intuition

### Quiz:

- What does the acronym UTXO stand for?
  - [x] Unspent Transaction Output
- Which of the following describes the difference between how transactions work in traditional banking sense and on a blockchain?
  - [x] Bank - there is concept of 'balance'. Transactions add or take away from that balance.
  - [x] Blockchain - each transaction has a life of it's own and has to start from another transaction(s) and end into other transaction(s).
  - [x] blockchain - there is no concept of 'balance'. What a cryptocurrency wallet demonstrates is simply an aggregation of all of the transactions which exist on the blockchain and include you as either a sender of receipent.
- Where do transaction fees come from?
  - [x] Fees constitute the difference between a transaction inputs and Outputs. Anything that is unused is given to the miner and that's how you can choose what fee you want to pay.
- Which of the following is not required by the Verification Function in order to verify the validity of a message (or transaction)?
  - [x] Private Key.
- What is the difference between a Public Key and an Address?
  - [x] These are almost the same. The Address is the SHA256 encrypted version of the public. This is done for additional security in case the elliptic curve is hacked.


### Create Cryptocurrency

See the source code in python:
  - [x] [freedomcoin.py](/course_edemy/blockchain/freedomcoin.py)

### Smart Contract Intuition

```bash
Definition - Smart Contract:

- "A set of promises,
- Specified in Digital Form,
- including protocols,
- within which the parties perform on these promises" Nick Szabo, 1996.
```

- What is Ethereum?
- What is a Smart Contract
- Decentralized Applications (DApps)
- Ethereum Virtual Machine & Gas
- Decentralized Autonomous Organizations (DAO)
- The DAO attack
- Soft and Hard Forks (Part 1)
- Initial Coin Offerings (ICOs)
- ICO Case Study 
- Blockchain and Web 3.0
- Quiz: Smart Contract intuition 

### Quiz:

- In a nutshell, what is Vitalik Buterin trying to build with Ethereum?
  - [x] The World's largest super-computer.
- What is a Smart Contract?
  - [x] A smart contract is the simplest form of decentralized automation, and is most easily and accurately defined as follows: a smart contract is a mechanism involving digital assets and two or more parties, where some or all of the parties put assets in and assets are automatically redistributed among those parties according to a formula based on certain data that is not known at the time the contract is initiated. [Vitalik Buterin on May 6, 2014](https://blog.ethereum.org/2014/05/06/daos-dacs-das-and-more-an-incomplete-terminology-guide/)
- What is Gas used for in Ethereum?
  - [x] Gas is used by applications to pay for running operations on user machines.
- Which statement about Forks is correct?
  - [x] A soft fork is backward compatible, a hard fork is not.
- What is the purpose of a Whitepaper in a Blockchain project?
  - [x] To describe how the project will leverage the different properties of Blockchain.
  - [x] To describe why the project needs its own token (or coin) if an ICO has been proposed. 
#### Resources

- [The Meaning of Decentralization](https://medium.com/@VitalikButerin/the-meaning-of-decentralization-a0c92b76a274)
- [DETERMINISTIC WALLETS, THEIR ADVANTAGES AND THEIR UNDERSTATED FLAWS
](https://bitcoinmagazine.com/technical/deterministic-wallets-advantages-flaw-1385450276)
- [Smart Contracts: 12 Use Cases for Business & Beyond
A Technology, Legal & Regulatory Introduction — Foreword by Nick Szabo](https://digitalchamber.org/wp-content/uploads/2018/02/Smart-Contracts-12-Use-Cases-for-Business-and-Beyond_Chamber-of-Digital-Commerce.pdf)
- [BOOK: DeFi and the FUTURE of FINANCE, Campbell R. Harvey Ashwin Ramachandran Joey Santoro]()