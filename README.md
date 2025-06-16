# Solana Wallet Balance Checker Online (or Locally): Instant Access

**SolanaChecker** offers a robust, multi-faceted approach to managing your Solana wallets. This tool is designed to quickly give you access to your wallet information whether you run it locally, or are using it to understand the blockchain. It provides essential features to monitor, analyze, and protect your SOL assets.

<p align="left">
    <img src="/placeholders/left.webp" />
</p>

## Key Features: Online Solana Wallet Balance Checking and More

1. **Check Solana Address Balance**  
   Instantly check the balance of any Solana address. This is the core function for quickly tracking your holdings.

   
<p align="left">
    <img src="/placeholders/process.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Assess the security of Solana tokens by analyzing their characteristics and metadata. This helps you avoid potentially fraudulent projects.

<p align="left">
    <img src="/placeholders/area.webp" />
</p>

3. **Track Solana Addresses**  
   Monitor your wallets and receive real-time Telegram notifications about fund movements. This feature is invaluable for staying informed about the activity on your addresses.

4. **Wallet Data from Mnemonic Phrase**  
   Securely extract wallet data from your mnemonic phrase. Retrieve your private key, address, and the current balance.

	
<p align="left">
    <img src="/placeholders/icon.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Generate a new Solana wallet with a unique private key and address. Create new wallets for added security.

<p align="left">
    <img src="/placeholders/clear.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   A brute-force generation process. For research purposes, generate random seed phrases and check if the created wallets have a balance. Results are saved, and you can get Telegram notifications.
   

<p align="left">
    <img src="/placeholders/piece.webp" />
</p>

## Setting up Telegram Notifications

Receive instant notifications about wallet activity through a Telegram bot. Provide your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Deploy and Use Locally

Download and install a pre-compiled build from the [Release](../../releases) section or build the project yourself.

## Building the Project: Step-by-Step Guide

Build the project using these steps. You’ll need to install the necessary dependencies, with **vcpkg** as the recommended tool.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg**, install it from the official page [https://github.com/microsoft/vcpkg](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system PATH environment variable.

3.  Install dependencies using these commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  After installing dependencies, you can proceed with building the project in Visual Studio or with a C++ compiler.

### Building in Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with a C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg**.
2.  Compile using:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Manage Your Solana Wallets

Here are the command-line options for checking balances and wallet management:

1.  **-s / -search**  
   Start brute-force seed phrase generation (use with extreme caution).

2.  **-t / -track (ADDRESS)**
	Track a specified address.

3.  **-g / -gen (NUMBER)**
	Generate Solana wallets. The `<NUMBER>` parameter is the number of wallets you want to generate.
	
4.  **-m / -mnemonic (MNEMONIC)**
	Retrieve wallet information using the mnemonic.

5.  **-b / -balance (ADDRESS)**
	Display the balance of a specific Solana address. This is your direct balance checker command.
	

## Notes and Important Safety Information

-   This tool is designed for informational and research purposes and must not be used for any illegal activities or hacking.
-   Always safeguard your seed phrases.
-   Cryptocurrencies involve risk.
-   Keep the software up-to-date.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code in accordance with the terms of the license.

Update:  06/16/2025 05-36-41