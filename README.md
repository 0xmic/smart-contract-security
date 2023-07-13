# Smart Contract Security

Below are notes pertaining to best practices for developing smart contract on Ethereum and other EVM blockchains.

## Development Best Practices
1. CEI - Checks, Effects, Interactions
2. Pull over Push
3. `msg.sender` over `tx.origin`
4. `call{value: <amount>}("")` with CEI or ReentrancyGuard over `transfer()` or `send()`
5. Chainlink VRF over `block.timestamp`

## Auditing Process
1. Developer writes smart contract code
2. Developer write tests for smart contracts
3. Static analysis tools are used to detect vulnerabilities in an automated fashion
4. Contracts are deployed and tested on a test network
5. A professional audit is conducted
6. Audit report is provided detailing vulnerabilities and how to patch
6. Vulnerabilities are patched prior to deploying to mainnet

## Auditing Contracts
The [auditing-contracts](./auditing-contracts/) repo details 5 common pitfalls when coding in solidity.
1. Missing input or precondition check
2. Phishing vulnerability with tx.origin
3. Incorrect calculation of output token amount
4. Timestamp manipulation
5. Block gas limit vulnerabilities

## Tools
* [Slither](./tools/slither-echidna/): Solidity Static Analysis
* [Echidna](./tools/slither-echidna/): Smart Contract Fuzzer

## Attacks
1. [Oracle Manipulation (Uniswap V2)](./attacks/oracle-manipulation/)
2. [Front Running](./attacks/front-running/)

## Additional Resources
* [Web3Sec - Top 20 Smart Contract Security Best Practices](https://blog.web3sec.news/posts/top-20-smart-contract-security-best-practices-checklist/)