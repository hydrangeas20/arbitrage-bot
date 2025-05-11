<h1>What Are Smart Contracts?</h1>
Smart contracts are self-executing programs stored on a blockchain that run when specific conditions are met. They automate transactions without needing a central authority or intermediary. Once deployed, smart contracts are immutable and transparent, ensuring security and trust in decentralized applications (dApps).

In this project, I used Solidity, the most popular language for writing Ethereum smart contracts, to create token swap contracts that let users convert tokens securely and automatically.

<h2>Why Use Smart Contracts in Crypto Arbitrage?</h2>
<p>Smart contracts help remove the middleman by automating multi-step crypto trades directly on the blockchain. In this project, the goal is to spot and exploit price mismatches between different cryptocurrencies — like BTC, USD (a stablecoin), and ETH.</p>

<b><i>Here's why smart contracts are ideal:</b></i>
<ul>
  
<p><li><b>Speed:</b> Prices in crypto change by the second. Smart contracts can detect opportunities and perform all three swaps (BTC → USD → ETH → BTC) instantly and automatically, before the prices change.</li></p>

<p><li><b>Atomicity (All-or-Nothing):</b> If one part of the trade fails (for example, if ETH suddenly jumps in price) the entire transaction gets reverted, and no funds are lost.</li></p>

<p><li><b>Trustless & Secure:</b> The contract handles your funds according to rules you coded in. No third parties, no exchange mishaps, onchain execution.</li></p>

<p><li><b>Automation:</b> You don't need to be by your computer all day waiting to press "swap" three times. The contract does it all in one transaction, 24/7.</li></p>

By chaining together multiple token swaps, your smart contract ensures you're always converting back to BTC.

<h2>Smart Contract Pseudocode</h2>
<ul>
  <li>1. Fetch current prices for BTC, ETH, and USD from exchange APIs.</li>
  <li>2. Calculate if a profit is possible by converting: <b>BTC → USD → ETH → BTC</b></li>
  <li>
    3. If profit > 0:
    <ul>
      <li>a) Execute trade 1: Swap BTC for USD</li>
      <li>b) Execute trade 2: Swap USD for ETH</li>
      <li>c) Execute trade 3: Swap ETH back to BTC</li>
    </ul>
  </li>
  <li>4. Log the transaction and profit.</li>
</ul>




