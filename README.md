# token-vesting
This is a sample application for ERC20 token vesting. It is an example of a properly configured environment, featuring everything that is needed to get up and running quickly, such as comprehensive documentation, robust testing, and a comprehensive development setup. All of these features come together to ensure that the project is well organized, easily maintainable and above all efficient to audit. 

# Specifications
### Project Overview
This GitHub repository houses an Ethereum-based ERC20 token vesting project. The primary purpose of this project is to enable token owners to establish various payment plans and deposit tokens, enabling users to receive these funds according to predefined criteria.

The vesting smart contract facilitates user-defined settings such as start dates, end dates, and token quantities to be released over the vesting period. This feature empowers users to structure a systematic release schedule for their tokens, ensuring a consistent distribution over a specified timeframe.

Additionally, the contract offers the capability to set a "cliff period," during which no tokens will be released. This feature ensures that users must remain committed to the project for a defined duration before receiving any tokens, fostering a vested interest in the project's success.

### Functional, Technical Requirements
Functional and Technical Requirements can be found in the [Requirements.pdf](./docs/Requirements.pdf) document

# Getting Started
Recommended Node version is 16.0.0 and above.

### Available commands

```bash
# install dependencies
$ npm install

# build for production
$ npm run build

# clean, build, run tests
$ npm run rebuild

# run tests
$ npm run test

# compute tests coverage
$ npm run coverage

# eslint automatically fix problems
$ npm run lint

# run pretty-quick on .ts , .tsx files
$ npm run lint-quick
```

# Project Structure
This a template hardhat typescript project composed of contracts, tests, and deploy instructions that provides a great starting point for developers to quickly get up and running and deploying smart contracts on the Ethereum blockchain.

## Tests

Tests are found in the `./test/` folder. `./test/shared/` contains various test helpers. No additional keys are required to run the tests.

Both positive and negative cases are covered, and test coverage is 100%.

## Contracts

Solidity smart contracts are found in `./contracts/`

`./contracts/mocks` folder contains contracts mocks that are used for testing purposes.

## Deploy
Deploy script can be found in the `deploy.ts` folder.

Rename `./.env.example` to `./.env` in the project root.
To add the private key of a deployer account, assign the following variables
```
PRIVATE_KEY=...
ETHERSCAN_API_KEY=...
ALCHEMY_API_KEY=...
```
example:
```bash
$ npm run deploy -- mumbai
```
