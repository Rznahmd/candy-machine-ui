# Candy Machine User Interface Configuration Guide

## Introduction
This document serves as a detailed guide for setting up the user interface (UI) of your Candy Machine for NFT minting operations. The UI enables the minting of NFTs with an SPL token, with transactions conducted through users' Phantom wallets.

## Prerequisites
Before starting, ensure you have the following:

- A Candy Machine configured with specific parameters in the `config.json` file, such as price, quantity, symbol, seller fee basis points, SPL token account, SPL token, activation date, and creator information.
- An operational Phantom wallet set for minting purposes.
- An SPL token created for this process.

## Configuration Steps

### Step 1: Setting Up Your SPL Token
Create an SPL token following the instructions in Lesson Three if you haven't already. Note the address of your newly created SPL token.

### Step 2: Candy Machine Configuration Update
Modify the `config.json` file of your Candy Machine by updating these fields:

- `splTokenAccount`: Enter the address of the SPL token account you've created.
- `splToken`: Input the address of your SPL token.

### Step 3: User Interface Setup
Follow the instructions in the "Quick Node: Set Up a Minting Site" guide to develop a UI for your Candy Machine. This interface allows users to link their Phantom wallets and use the SPL token to mint NFTs.

### Step 4: Modify Minting Logic
Alter the minting logic within your project (as outlined in Lesson Three) to either mint NFTs directly to the user's Phantom wallet address or adjust the transfer function to send minted NFTs to your Phantom wallet.

### Step 5: Conduct Testing
Test the entire system thoroughly by sending or minting your SPL token to a Phantom wallet. Ensure that the UI facilitates smooth NFT minting for users who pay with the specified SPL token.

## Conclusion

Following this guide should enable you to successfully set up the user interface for your Candy Machine, allowing for efficient NFT minting with an SPL token via Phantom wallets.
