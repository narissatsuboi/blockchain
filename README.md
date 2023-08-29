# blockchain
# Bitcoin Block Integrity Demonstration

This program showcases the integrity of Bitcoin blocks by connecting to the P2P Bitcoin network, retrieving an old block, simulating changes to transaction data, and demonstrating how the network detects and rejects such changes.

## Requirements

- Connects to a peer in the P2P Bitcoin network and retrieves a block based on your SU ID number modulo 10,000.
- Optionally, displays transactions within the retrieved block.
- Optionally, manipulates a transaction's output account, corrects the block's data, and ensures consistent merkle-tree hashes.
- Generates a report highlighting changes in the block's hash and how the modified block would be rejected by peers in the network.
- Developed using Python 3 with no use of publicly available Bitcoin libraries (except makeseeds as shown below).
- Uses TCP/IP to communicate with a full node in the Bitcoin network.

## Getting Connected

1. Obtain a list of Bitcoin nodes using makeseeds (install dnspython with `pip3 install dnspython`).
2. Fetch nodes from `nodes_main.txt` that are not onion nodes and choose one working node.

## Usage

1. Connect to the Bitcoin network and retrieve a block based on your SU ID number.
2. Display transactions within the block (optional).
3. Simulate changes to a transaction's output account and ensure merkle-tree hashes are updated (optional).
4. Generate a report demonstrating how the hash of the block changes and how the modified block would be rejected.

## Example Usage

```bash
python3 blockchain.py

## Resources

Explore these valuable resources to deepen your understanding of Bitcoin and blockchain technology:

- [Bitcoin Official Website](https://bitcoin.org)
- [Bitcoin Developer Guide - P2P Network](https://developer.bitcoin.org/devguide/p2p_network.html)
- [Bitcoin Wiki](https://en.bitcoin.it/wiki/Main_Page)
- [Bitcoin Improvement Proposals (BIPs)](https://github.com/bitcoin/bips)


