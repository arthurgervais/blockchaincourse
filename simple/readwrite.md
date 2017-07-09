# Read and write access

In the following we outline which entities are eligible to post messages on the blockchain and which entities are eligible to read the blockchain.

## Read access
A decentralized blockchain allows anybody to read the written content. Any message that is posted, is therefore fully transparent and world-readable.

{%mcq ans="o2", random=true%}
{%title%} Why is it problematic if all messages on the blockchain are world-readable?
{%o1%} An entity could modify a message.
{%o2%} If a message corresponds to a financial transaction, the time, value, sender and receipient are public.
{%o3%} A coin can be spent if the identification number is known.
{%message%} Note that a message is valid only if it has been signed with the appropriate crytographic key of the coin owner. By parsing the blockchain messages, the ownership of a coin can be determined.
{%endmcq%}

## Write access
Write access, i.e. the ability to write messages to the blockchain is rule based. The rules for writing to the blockchain are enforced by other peers of the blockchain, i.e. peers only accept a message, if the message follows the write access rules.

In Bitcoin and Ethereum, peers need to prove to have performed a given amount of work in order to be eligible to write to the blockchain. Performing this work is computationally expensive, while verifying that the work has been performed is inexpensive.