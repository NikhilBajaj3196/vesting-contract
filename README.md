# Token Vesting Contracts

## Overview

On-Chain vesting scheme enabled by smart contracts.

`TokenVesting` contract can release its token balance gradually like a typical vesting scheme, with a cliff and vesting period.
The vesting schedules are optionally revocable by the owner.

## 🎭🧑‍💻 Security audits

This repository is compatible with both Forge and Hardhat.
Forge needs to be ran (install and build) before Hardhat is used in order to load dependency contracts.
You can find the specific instructions for each tool below.

### Forge

#### 📦 Installation

```console
forge install
```

#### ⛏️ Compile

```console
forge build
```

#### 🌡️ Testing

```console
$ forge test
```

### Hardhat

#### 📦 Installation

```console
$ yarn
```

#### ⛏️ Compile

```console
$ yarn compile
```

This task will compile all smart contracts in the `contracts` directory.
ABI files will be automatically exported in `build/abi` directory.

#### 📚 Documentation

Documentation is auto-generated after each build in `docs` directory.

The generated output is a static website containing smart contract documentation.

#### 🌡️ Testing

Note: make sure to have ran forge build and compile before you run tests.

```console
$ yarn test
```

#### 📊 Code coverage

```console
$ yarn coverage
```

The report will be printed in the console and a static website containing full report will be generated in `coverage` directory.

#### ✨ Code style

```console
$ yarn prettier
```

#### 🐱‍💻 Verify & Publish contract source code

```console
$ npx hardhat  verify --network mainnet $CONTRACT_ADDRESS $CONSTRUCTOR_ARGUMENTS
```