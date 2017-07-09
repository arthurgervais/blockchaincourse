# Node Types
Due to the variety of different entities that can participate in an open and decentralized blockchain such as Bitcoin, multiple nodes types emerged.

## Miner
Miners perform the Proof of Work to find and broadcast blocks in the Bitcoin network. Their operations consist mainly in quickly retrieving information about the newest blocks, validating transactions that are included in new blocks, operate dedicated mining hardware to perform as many hash operations as possible, and to efficiently spread found blocks to the whole network.

Every discovered Bitcoin block provides a monetary reward, for example, 12.5 bitcoins to the respective miner. Because a block, however, is found on average only every 10 minutes, the time until a miner receives a payout can be significant. Miners therefore typically organize themselves into groups of miners, commonly referred to as mining pools. Because of its higher overall hashing power, a mining pool has a higher chance to find a block, and mining pool members can consequently receive payouts more periodically than an independent miner.

## Full node
We define a full Bitcoin node as a node that (i) maintains the full copy of the blockchain, (ii) validates incoming transactions and blocks, and (iii) forwards transactions and blocks to its peers. In addition to providing validation services to the Bitcoin network, a full node might provide an open TCP port (Bitcoin uses the TCP port 8333), where other Bitcoin peers can connect to.

## Lightweight Clients
Lightweight clients are clients that do not maintain the full Bitcoin blockchain, but rather follow the Simple Payment Verification (SPV) scheme. This scheme allows the lightweight client to verify that a transaction has been included in the blockchain, by only receiving the block headers. Besides, lightweight clients do not receive transactions that are irrelevant to their operation, do not need to perform transaction or block validation and consequently require significantly fewer resources to operate than full nodes or miners.

# Information Dissimination

## Peer-to-Peer Overlay Network

Bitcoin's Peer-to-Peer overlay network enables peer discovery and provides broadcast information propagation. The network is loosely and by default randomly connected. A fraction of all Bitcoin peers provide incoming TCP connections on port 8333 (typically full Bitcoin nodes) to which other peers can connect to. SPV clients, in particular, do not provide direct services to the P2P overlay network and only listen for information relevant to their respective operation.
