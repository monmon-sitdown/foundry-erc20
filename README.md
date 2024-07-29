# OurToken Project

This project implements a simple ERC20 token named "OurToken" using Solidity and the OpenZeppelin library. It includes the token contract, deployment script, and test file.

## Project Structure

- `src/OurToken.sol`: The main token contract
- `script/DeployOurToken.s.sol`: Deployment script for the token
- `test/OurTokenTest.t.sol`: Test file for the token contract

## Features

- ERC20 compliant token
- Initial supply of 99 tokens (considering 18 decimal places)
- Deployment script for easy token deployment
- Comprehensive test suite

## Prerequisites

- Solidity 0.8.19
- Foundry (for deployment and testing)
- OpenZeppelin contracts

## Installation

1. Clone this repository
2. Install dependencies:
   ```
   forge install
   ```
   This will install the required dependencies (forge-std and OpenZeppelin) in the lib/ directory.

## Dependency Management

This project uses Foundry for dependency management. The dependencies are specified in the foundry.toml file and are installed in the lib/ directory. These directories are ignored by git .

## Deployment

To deploy the token:

```
forge script script/DeployOurToken.s.sol:DeployOurToken --rpc-url <your_rpc_url> --private-key <your_private_key>
```

Replace `<your_rpc_url>` and `<your_private_key>` with your actual RPC URL and private key.

## Testing

Run the tests using Foundry:

```
forge test
```

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
