# Perfrom front-running attack

## Technology Stack & Dependencies

- Solidity (Writing Smart Contract)
- Javascript (Game interaction)
- [NodeJS](https://nodejs.org/en/) To create hardhat project and install dependencies using npm


### 1. Clone/Download the Repository

### 2. Install Dependencies:
```
npm install
```

### 3. Perfrom the attack by running the test
```
npx hardhat test
```

## Mitigating Front Running
Instead of using the `create2` opcode, use a hash of `msg.sender + nonce`. This is because `msg.sender` is hard-coded and cannot be front-run.