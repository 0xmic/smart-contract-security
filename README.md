# Smart Contract Security

Below are notes pertaining to best practices for developing smart contract on Ethereum and other EVM blockchains.

## Best Practices
1. CEI - Checks, Effects, Interactions
2. Pull over Push
3. `msg.sender` over `tx.origin`
4. `call{value: <amount>}("")` with CEI or ReentrancyGuard over `transfer()` or `send()`
5. Chainlink VRF over `block.timestamp`
