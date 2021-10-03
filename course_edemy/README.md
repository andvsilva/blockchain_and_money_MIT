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
XXXXXXXXX - - [03/Oct/2021 12:21:17] "GET /get_main HTTP/1.1" 404 -
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

#### Resources

- [The Meaning of Decentralization](https://medium.com/@VitalikButerin/the-meaning-of-decentralization-a0c92b76a274)