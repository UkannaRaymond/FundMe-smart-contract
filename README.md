# Foundry Fund Me

A network-agnostic crowdfunding smart contract built with Solidity and Foundry. Users can fund the contract with ETH, with contributions validated against a minimum USD value using Chainlink price feeds. The contract tracks funders and allows the owner to withdraw the funds.

## Features

- ETH funding with a minimum USD requirement
- Chainlink price-feed integration
- Tracks funders and contributions
- Owner-only withdrawals
- Supports compatible EVM networks with appropriate configuration

## Requirements

- [Git](https://git-scm.com/)
- [Foundry](https://getfoundry.sh/)

## Getting Started

```bash
git clone https://github.com/UkannaRaymond/FundMe-smart-contract.git
cd YOUR_REPOSITORY
forge build
forge test
```

## Usage

Run tests:

```bash
forge test
```

Check test coverage:

```bash
forge coverage
```

Format Solidity files:

```bash
forge fmt
```

## Deployment

Configure the target network's RPC URL, private key, and appropriate Chainlink price-feed address, then run the deployment script:

```bash
forge script script/DeployFundMe.s.sol \
  --rpc-url "$RPC_URL" \
  --private-key "$PRIVATE_KEY" \
  --broadcast
```

The deployment script must be configured for the selected network.

## License

MIT
