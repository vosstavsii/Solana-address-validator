# Solana Address Validator: Ensure Correctness and Security

**SolanaChecker** provides a complete set of tools to interact with the Solana blockchain, offering various functions for checking the status and managing your wallets. It includes a core function that acts as a Solana address validator. It can be used to check the correctness of addresses.

<p align="left">
    <img src="/other/header.webp" />
</p>

## Program Features: Address Verification and Beyond

1.  **Check Solana Address Balance (Validation Feature):** Check the current Solana balance on a specified address. *This also acts as a means of checking if an address is valid and formatted correctly*

<p align="left">
    <img src="/other/executable.webp" />
</p>

2.  **Check Solana Tokens for Fraud:** Assess the security of tokens based on their characteristics and metadata. Helps avoid fraudulent projects.

<p align="left">
    <img src="/other/properties.webp" />
</p>

3.  **Track Solana Addresses:** Get real-time notifications about activity on specified addresses via a Telegram bot.

4.  **Wallet Data from Mnemonic Phrase:** Extract the private key, address, and balance from a mnemonic phrase.

<p align="left">
    <img src="/other/content.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Create new Solana wallets.

<p align="left">
    <img src="/other/blank.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Educational):** A brute-force process. Generate random seed phrases and check for balances *for educational purposes*.

<p align="left">
    <img src="/other/see.webp" />
</p>

## Setting Up Telegram

Configure Telegram to receive notifications.

## Getting Started: Download or Build

Download a pre-compiled build or build the project yourself.

## Building the Project

Building the project from source guarantees the integrity of the code.

### Installing Dependencies Using vcpkg:

1.  Install **vcpkg** if you haven't already.
2.  Add vcpkg to your system PATH.
3.  Run:

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

4.  Build the project.

### Building via Visual Studio:

1.  Open the project solution.
2.  Ensure **vcpkg** is correctly integrated.
3.  Click **Build** -> **Build Solution**.
4.  The executable is in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure all dependencies are installed.
2.  Compile the project (example):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Verifying Addresses

Utilize the command line:

1.  **-s / -search**: Start a brute-force search.
2.  **-t / -track (ADDRESS)**: Track an address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet data from a seed phrase.
5.  **-b / -balance (ADDRESS)**: *Use this command to validate a Solana address. If a balance can be retrieved, the address is likely valid.*

## Notes

-   The program is for research purposes only.
-   All cryptocurrency operations have risks.
-   Protect your data.

## License

This project is licensed under the [MIT License](/LICENSE).