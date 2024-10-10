
# Connect Wallet with AppKit

This project demonstrates how to connect a cryptocurrency wallet using Reown's AppKit with support for multiple networks, leveraging the Ethers.js library for Ethereum interactions. The example features wallet connection, network selection, and an integration of Web3Modal (rebranded from WalletConnect).

### Requirements

- Basic understanding of HTML, JavaScript, and web development.
- A Reown Cloud account with an active Project ID.
- Familiarity with Ethers.js and wallet integration.

### Files

- `index.html`: The main HTML file with JavaScript embedded to handle wallet and network modals using AppKit.

### Features

- Wallet connection using a modal popup.
- Network selection with supported chains (e.g., Ethereum Mainnet and Arbitrum).
- Simple buttons to open the connection and network modals.
- Integration with Ethers.js for managing blockchain interactions.

### Usage Instructions

1. **Clone or Download the Project**
Download or clone the project repository to your local environment.
2. **Configure the Project ID**
    - In the provided code, replace `'Your Project Id'` with your actual Project ID from Reown Cloud:
        
        ```jsx
        
        const projectId = 'Your Project Id';
        
        ```
        
3. **Supported Networks**
    - Define the blockchain networks you want to support. This example supports Ethereum mainnet and Arbitrum:
        
        ```jsx
        
        const networks = [window.AppKit.networks.mainnet, window.AppKit.networks.arbitrum];
        
        ```
        
4. **Optional Metadata**
    - If desired, add metadata for your app, such as the name, description, and logo. This is optional and can be uncommented in the code if needed.
5. **Run the Project**
    - Open the `index.html` file in a web browser.
    - Click on the "Open Modal" button to trigger the wallet connection modal, or "Open Networks" to select a network.

### External Libraries

- **Ethers.js**: A library for interacting with Ethereum wallets and contracts. The script is included from a CDN:
    
    ```html
    
    <script type="module" src="https://cdn.jsdelivr.net/npm/ethers/dist/ethers.min.js"></script>
    
    ```
    
- **AppKit**: The core library for connecting and interacting with wallets through Reown's services. The script should be updated to point to the correct local or hosted path
    
    ```html
    
    <script type="module" src="./appkit/dist/appkit.js"></script>
    
    ```
