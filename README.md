# OurToken ERC-20 Token 🪙

This repository contains the implementation of **OurToken (OT)**, a custom ERC-20 token built using the OpenZeppelin library. It uses **Foundry** for deployment and testing.

---

## Features 🚀
- **ERC-20 Standard Token**: Implements a fungible token with `name` as **OurToken** and `symbol` as **OT**.
- **Initial Supply**: The token mints the total supply to the deployer's address upon deployment.
- **Test Suite**: Includes unit tests for token balances, allowances, and transfers.

---

## How to Use 🛠️

### Deployment
The deployment script is located at `script/DeployOurToken.s.sol`. It deploys the token with an initial supply.

### Steps to Deploy:
1. **Install Foundry** (if not already installed):
   ```bash
   curl -L https://foundry.paradigm.xyz | bash
   foundryup
    ```

2. **Clone the repository**:
```bash
git clone https://github.com/your-username/OurToken.git
cd OurToken
```
3. **Install dependencies**:
```bash
forge install
```
4. **Deploy the contract**:
```bash
forge script script/DeployOurToken.s.sol:DeployOurToken --rpc-url <YOUR_RPC_URL> --broadcast
```
## Testing 🧪
This project includes comprehensive tests located in the test directory. The tests check:

1. Token balances for users.
2. Allowance functionality (e.g., approvals and transfers via a third party).

### Run the Tests:
```bash
Copy code
forge test
```

Use the -vvvv flag for detailed logs:
```bash
Copy code
forge test -vvvv
```
