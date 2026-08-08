🌐 Multi-Network Drainer 

<p align="center">
  <b>A lightweight, responsive Web3 interface for legitimate multi-chain USDT transfers.</b>
</p><p align="center">
  <a href="https://github.com/xepel">GitHub</a> •
  <a href="https://t.me/angraaj">Telegram</a>
</p>---

📖 Overview

Multi-Network USDT Transfer is a lightweight Web3 interface designed for sending USDT across supported blockchain networks.

The interface provides a simple network selector and wallet connection flow, allowing users to select a supported network and initiate a transaction through their own Web3 wallet.

The project focuses on:

- Clean and responsive UI
- Multi-chain support
- Wallet-based transaction signing
- Simple configuration
- Minimal dependencies
- Easy integration into existing Web3 projects

«Important: Users must always be able to clearly see and verify the destination address, token, network, and transaction details before signing.»

---

✨ Features

🌐 Multi-Network Support

Designed to support multiple EVM-compatible networks, including:

- BNB Smart Chain
- Ethereum
- Polygon
- Arbitrum

Additional networks can be added through the network configuration.

🔗 Web3 Wallet Integration

Connect using compatible wallets such as:

- MetaMask
- Brave Wallet
- Other EIP-1193 compatible Web3 wallets

⚡ Network Switching

The application can request the user's wallet to switch to the selected blockchain network when required.

💰 USDT Transfer

Users can enter the amount of USDT they want to transfer and initiate the transaction directly through their wallet.

🧮 Amount Helper

The interface can display an approximate USD value while the user enters an amount.

📱 Responsive Design

The interface is designed to work across:

- Desktop
- Tablet
- Mobile
- Web3-enabled browsers

🎨 Minimal UI

A lightweight, borderless interface with minimal visual elements makes the application easy to integrate into other projects.

---

🛡️ Security & Transparency

This project is intended for legitimate user-authorized transactions.

The application should never:

- Hide the recipient address
- Use deceptive recipient addresses
- Request unnecessary wallet permissions
- Automatically transfer assets without explicit user authorization
- Attempt to bypass wallet confirmation
- Store private keys or seed phrases

Always display the following information clearly before a transaction is signed:

Network
Token
Recipient Address
Amount
Estimated Network Fee
Transaction Type

Users should independently verify the transaction details in their wallet before confirming.

---

🚀 Getting Started

1. Clone the Repository

git clone https://github.com/xepel/usdt-multi-transfer.git
cd usdt-multi-transfer

2. Open the Application

For a quick test, open:

index.html

in a Web3-compatible browser.

For development, a local HTTP server is recommended:

python3 -m http.server 8080

Then open:

http://localhost:8080

3. Connect Your Wallet

1. Select the desired network.
2. Connect your Web3 wallet.
3. Enter the recipient address.
4. Enter the USDT amount.
5. Review the transaction details.
6. Confirm the transaction from your wallet.

---

⚙️ Configuration

Network Configuration

Networks can be configured through the "NETWORKS" object in the JavaScript section.

Example:

{
  name: "Network Name",
  chainId: "0x...",
  rpc: "https://...",
  usdt: "0x...",
  nativeCurrency: {
    name: "Native Token",
    symbol: "TOKEN",
    decimals: 18
  },
  explorer: "https://...",
  icon: "https://..."
}

Recipient Address

The recipient address should be provided transparently through the application's UI rather than hidden inside the application.

Example:

const recipient = document.getElementById("recipient").value;

Before signing, the application should display the complete recipient address to the user.

---

🧩 Supported Network Configuration

Network| Chain Type| Token
BNB Smart Chain| EVM| USDT
Ethereum| EVM| USDT
Polygon| EVM| USDT
Arbitrum| EVM| USDT

«Always verify token contract addresses from official network/token sources before deploying a production application.»

---

🔐 Best Practices

Before deploying the application publicly:

- Validate Ethereum/EVM addresses.
- Validate token amounts.
- Display transaction details before signing.
- Handle rejected wallet transactions gracefully.
- Handle incorrect-network errors.
- Never request seed phrases or private keys.
- Never store private keys in frontend code.
- Use HTTPS in production.
- Use verified token contract addresses.
- Test on testnets before using real funds.
- Keep dependencies updated.



🤝 Contributing

Contributions are welcome.

Development workflow

git clone https://github.com/xepel/usdt-multi-transfer.git
cd usdt-multi-transfer

Create a feature branch:

git checkout -b feature/my-feature

Commit your changes:

git add .
git commit -m "Add my feature"

Push the branch:

git push origin feature/my-feature

Then open a Pull Request.

---

📬 Contact

MR.NIGHT

<p>
  <a href="https://github.com/xepel">
    <img src="https://img.shields.io/badge/GitHub-Xepel-181717?style=for-the-badge&logo=github" alt="GitHub">
  </a>
  <a href="https://t.me/angraaj">
    <img src="https://img.shields.io/badge/Telegram-@angraaj-26A5E4?style=for-the-badge&logo=telegram" alt="Telegram">
  </a>
</p>GitHub: "Xepel" (https://github.com/xepel)

Telegram: "@angraaj" (https://t.me/angraaj)

---

⚠️ Disclaimer

This project is provided for educational and legitimate Web3 development purposes.

Users are responsible for verifying transaction details before signing any blockchain transaction.

The developers and contributors are not responsible for losses resulting from:

- Incorrect recipient addresses
- Incorrect network selection
- Incorrect token contracts
- User error
- Wallet compromise
- Third-party services
- Gas or network fees

Never share your seed phrase or private key with anyone or any website.

---

📄 License

This project is released under the MIT License.

See "LICENSE" for the complete license text.

---

<p align="center">Made with ❤️ by MR.NIGHT

<a href="https://t.me/angraaj">Telegram</a> •
<a href="https://github.com/xepel">GitHub</a>

</p>
