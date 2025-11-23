# Blockchain
- Centralized = one party controls everything
- Decentralized but Permissioned = fixed list of parties (hyperledger)
- Fully Permissionless = everyone can participate (bitcoin...)
## Centralized anonymous cash
- bank can't find details of received money
## Decentralizazion in 80s
- no single bank - multiple banks are computing

## Bitcoin consensu
- consensus in permissionless setting is impossible
  + fake identities can be created freely to control the majority of the system -> consensus is impossible
- instead the "voting" is done using resources - for bitcoin it is computing power (the more power, the more control)
  + so even if someone creates more identities, they cant create more computing power freely

## Proof of Work
- How do I prove, that computing power has been used? (e.g. that I computed H 10^9 times)
- Bob chooses c (bitstring), Bob then has to find input value \pie, so that H(\pie) = c // check if this is correct
- computing for transactions result in appending a block to the blockchain

## Why is Bitcoin secure?
- most will try to continue the main chain, if someone malicious tries to fork it, it will practically always be less computing power, thus the fork is shorter, making it recognsiable as a fork

## Consensus Layer
- Protocol that controls the ever growing blockchain

## Application Layer
- how is the data of each block interpreted (Bitcoin: UTXA/transactions, Ethereum: Smart Contracts (write contracts in turing complete language))

## Sustainability
- environmental
  + energy, hardware
- technological
  + postquantum security
  + scalability bottlenecks
- social
  + concentration of mining/staking
- economic
  + block rewards security vs inflation (idk why)

## Technological
- Scalability wise, VISA e.g. can manage 24000 transactions per second, bitcoin only 7, eth only 20, litecoin 56, paypal 193
- Ideas:
  + create bigger blocks
  + increase block creation rate
  + sharding: you maintain multiple blockchains for one blockchain
  + Layer 2 Solutions (a layer above the low level blockchain):
    - rollups: powerful cryptographic tools to 
    - payment networks (lightning for bitcoin), so most transactions happen off-chain

## Environmental
+ originally the idea was to use spare cpu cycles for mining
+ however, this transitioned to GPUs and later specialised hardware (ASICs) to compute the hash function
+ Single Bitcoin transaction:
  - 450 kgCO2
  - 830 kWh

## Is there are more environmentally friendly?
+ replace proof of work with alternatives
+ => Proof of Stake (ETH, ALGO)
+ ETH transitioning from Proof of Work to Proof of Stake reduced Energy consumption by ~99.95%

## Issues with Proof of Stake
+ Implementation is harder than proof of work
  - pos has less convergence to one chain
  - potential attacks
+ you get more money by having more money (less decentralisation)

## Alternative?
+ Use disk storage over computing power (many people have left over disk storage)

## Proof of Space
+ how do I prove that i store a terabyte of data?
  - naive: e.g. bob asks random index, alice confirms data at that location - but too much network use - slow
+ instead, pebbling: compute hashes of parents to prove space

## Proof of Time
- Verifieable Delay functions

## Combinations
- combination of Proof of Space and Proof of Time
- chia
- ! however, some people found a way to compress the data (factor of 2) (so use computing power to store more)
  + => so they all go double the rewards

## Decentralizazion
- Nakamoto coefficient
  + = min. number of entties, so that they can together control the system (break consesnus, integrity..)
- see graph in presentation

## DePIN 
- decentralised physical infrastructure network
- filecoin, uses Proof of Space
