# Auditing with security tools slither and echinda
This repo showcases an example contract that has 10 vulnerabilities. We can observe the smart contract's security gaps using Slither and Echidna.

Documentation:
* [Slither](https://github.com/crytic/slither)
* [Echidna](https://github.com/crytic/echidna)

## Technology Stack & Dependencies

- Solidity (Writing Smart Contract)
- [NodeJS](https://nodejs.org/en/) To create hardhat project and install dependencies using npm


### 1. Clone/Download the Repository

### 2. Install Dependencies:
```
npm install
```

### 3. Install Slither
- Install the solc compiler first then slither
```
brew tap ethereum/ethereum
```
```
brew install solidity
```
```
git clone https://github.com/crytic/slither.git && cd slither
```
```
sudo python3 setup.py install
```
```
slither .
```
### 4. Install and use echinda
- Install the solc compiler first then slither
```
docker pull trailofbits/eth-security-toolbox
```
```
docker run -it trailofbits/eth-security-toolbox
```
