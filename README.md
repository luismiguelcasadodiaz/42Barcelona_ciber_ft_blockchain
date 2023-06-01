# Blockchain with proof of work

## Blockchain implementation based on Proof of work algorithm.

1.-Add transaction to block
2.-Mine the block
3.-Add block to chain

### Simple proof -of-work-algoritm:
    1.-Guest number
    2.-Concatenate wiht previuos
    3. Hash cincatenated string
    4.-Hash must end 4242


### Non persistent chain of blocks
Implemented in memory. Not saved to any database.


## Mining
1.-Calculate proof of work
2.-Reward miners (create the rewarding transacion)
3.- Create new block and add it ti the chain


## Server to operate wiht the blockchain.
HTTP request on a Text-based API
[POST]/transaction/new ==> Post a new transaction to add ti the next block
[GET]/mine             ==> Execute proof of work and create new block
[GET]/chain            ==> Returns infromation about the full blockchain

Network timestaps each 

```
block =
{   
    'index': 4,
    'timestamp': 1644045050.00042,
    'transactions':[
                        {
                        'sender': '4c6e7e2a9f2f7f7ff8e7d3d6c8b7c6e8e23a7',
                        'recipient': 'b3c6e7e2a9f2f7f7ff8e7d3d6c8b7c6e8e23a7',
                        'amount': 42,
                        }
                    ],
    'proof': 324984774000,
    'previous_hash': '084c799cd551dd1d8d5c5f9a5d593b2e931f5e36122ee5c793c1d08a19839cc0',
}   
```
BONUS
Dynamical adjustmen of proof of work dificculty in funciton of elapsed time or mined blocks....
Implement a decentralized network of nodes that communicate between them
Implement a consensus algoritm to verify the goodness of the chain.
Implement a Proof of Stake as an alternative to the proof of work

SUPPORT DOCS
[Consensus Algorithm](https://en.wikipedia.org/wiki/Consensus_(computer_science))