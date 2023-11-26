Due to the requirements of the homework found in Karvinen (2023), this is what I could have executed: 

# X) Summaries
### *Nakamoto 2008: Bitcoin: A Peer-to-Peer Electronic Cash System*

1. Nakamoto (2008), discussed how online payments work, which are quite dependable on middlemen and for that, he suggested a computational transaction that is more secure and prevents reversals, making it more difficult to hack; 
2. The proposed electronic coin system uses a chain of digital signatures for ownership. Since the main challenge is preventing double-spending, the suggested solution is to publicly announce transactions and have participants collectively agree on their order; 
3. The transaction begins with a timestamp server that proves that the information existed at that specific time, which strengthens the previous ones by including them in its code;
4. In order to make sure everyone agrees on the order of the transactions, the proof-of-work method is used like a puzzle in which computers get to decide the order of transactions, ensuring fairness and security in the system;
5. Thus, whenever someone wants to make a transaction in the network, they tell everyone and computers group these transactions into blocks;
6. Then in this system, the first transaction in a block creates a new coin for the block`s creator, motivating nodes to support the network. This process, compared to gold miners adding gold to circulation, uses CPU time and electricity, and as more coins circulate, the incentive can shift to transaction fees. 


# a) Wallet. Creation of a BitCoin testnet wallet.

For the creation of the Bitcoin testnet wallet I followed the tips provided by Karvinen (2023). The procedure in the Debian terminal was the following: 

<img width="370" alt="Testnet 1" src="https://github.com/Student20231/Hello/assets/149126670/7b0f259b-3b77-4ce2-922f-8a696b2f753b">
<img width="368" alt="Testnet 2" src="https://github.com/Student20231/Hello/assets/149126670/1d2c5169-ab3d-4f28-82dd-74b873d92c17">
<img width="422" alt="Testnet wallet" src="https://github.com/Student20231/Hello/assets/149126670/80b71f17-84bf-486c-ad4d-62e340c44b26">

# b) Faucet. Getting worthless fake money from a testnet Bitcoin faucet.

At first, I tried some faucets by accessing them from my main computer. However, after consulting the 'history' tab in my electrum wallet and noticing that no transfer had ocurred, I tried to access those faucets from the Debian VM. I deleted all the addresses requested from the 'Receive' tab and created a new one as shown below: 

<img width="960" alt="Creation of address" src="https://github.com/Student20231/Hello/assets/149126670/ba0a101f-f4f5-4025-9408-77a0dd97e20f">

Then, I copied the adress and inserted in the first faucet: 

<img width="671" alt="Attempt 1" src="https://github.com/Student20231/Hello/assets/149126670/67044f79-9ec9-451a-9650-26b74965687c">

Since I didn`t notice any change in my wallet I proceeded to attempt 2:

<img width="510" alt="Attempt 2" src="https://github.com/Student20231/Hello/assets/149126670/cdf168a0-8693-4bb8-b630-c89c32d28bcc">

In here, the author referred that the transaction would be manual and it could take days to do, which for me it is a bit suspicious. 

Therefore, I went for attempt 3: 

<img width="574" alt="Attempt 3" src="https://github.com/Student20231/Hello/assets/149126670/4f406eb0-a399-4b73-9775-ebd69d3a8afc">

I wonder if the faucet cannot read this address, thus being necessary another kind of address request from the electrum wallet. 

# c) Giveway. Moving money to another Bitcoin wallet. Choosing an amount where the last two digits are 42.

I understand that by going to the 'Send' tab in the electrum wallet, I will be able to transfer any given amount to a certain recipient but since I didn`t receive any, I`m able to send either. 

<img width="419" alt="Sending coins" src="https://github.com/Student20231/Hello/assets/149126670/5643eb51-83ec-410f-a3fe-d8a2f8736c38">


# d)  Explorer. Using a block explorer to analyze a block on the real Bitcoin blockchain.

I`ve chosen the blockchain.com (blockchain.com , 2023), and more specifically the block 818,534 to analyse details about it in a real blockchain. Besides the initial description shown in the site "A total of 3,491.58 BTC ($131,908,970) were sent in the block with the average transaction being 0.8152 BTC ($30,797.55). ViaBTC earned a total reward of 6.25 BTC $236,119. The reward consisted of a base reward of 6.25 BTC $236,119 with an additional 0.5324 BTC ($20,113.61) reward paid as fees of the 4,283 transactions which were included in the block.", I thought it was interesting to point out the following:
1. The difficulty to find a valid block hash is 67,957,790,298,897.88 showing an increased competition to mine the block and being recommended to join a mining pool to combine computer power (Cleartax, 2022).;
2. In this case, there is a mining pool called "ViaBTC" that is responsible for confirming the transactions in the block. 
Other details that have been supported by information retrieved from Bitcoin wiki (2019,2023), Cryptopedia (2023), Frankenfield (2022), Javatpoint (2023), and Reserve Bank of Australia (2023):
1. Hash - Identifier for the block and initial 0s indicate a proof-of-work requirement;
2. Capacity - 177.2% shows the block space utilization and since it is over 100%, it means that the block is congested ;
3. Distance - Shows the time that the previous block was mined, thus indicating distance between blocks;
4. BTC - how much BTC was transacted in the block (3,491.5831);
5. Value - Same as point 4 but in USD ($131,908,970);
6. Value today - estimated current value in USD;
7. Average value - average value of individual transactions;
8. Median value - median value of individual transactions;
9. Input value - the total value of BTC used as input in the transactions;
10. Output value - the total value of BTC received as output in the transactions within the block;
11. Transactions - number of transactions in the block;
12. witness Tx`s - number of transactions using the Witness protocol to improve BTC scalability;
13. Inputs - number of inputs used in the transaction within the block;
14. Outputs - number of BTC addresses receiving funds;
15. Fees - total fees paid by users;
16. Fees kb - fee per kilobyte of block space;
17. Fees kwu - fee per kiloweight unit;
18. Depth - number of blocks on top of this one;
19. Size - size of the block in bytes;
20. version - protocol version of the block;
21. Merkle root - hash of all the transaction hashes;
22. Difficulty - computation effort to find a valid hash;
23. Nonce - value that miners adjust during the mining process;
24. Bits - compact form of the target difficulty;
25. Weight - the block weight accounting for the size and complexity of transactions;
26. Minted - base reward given to the miner for mining successfully the block;
27. Reward - total reward including the base reward and additional fees paid by users;
28. Mined - timestamp indicated when the block was mined;
29. Height -position in the blockchain;
30. Confirmations - number of confirmations received by the block;
31. Fee range - range of fees per virtual byte in the block;
32. Average fee - the average fee per transaction in the block;
33. Median fee - median fee per transaction in the block;
34. Miner - The mining pool responsible for confirming the transactions in the block.

## References

Bitcoin testnet faucet, 2023. URL: https://bitcoinfaucet.uo1.net/

Cleartax, 2022. Mining Difficulty: What Is It And Benefits URL: https://cleartax.in/s/mining-difficulty#:~:text=This%20difficulty%20is%20known%20as,algorithm%20to%20regulate%20this%20adjustment.

Coinfaucet, 2023. URL:https://coinfaucet.eu/en/btc-testnet/

Bitcoin wiki, 2019. Block. URL: https://en.bitcoin.it/wiki/Block

Bitcoin wiki, 2023. Transaction. URL: https://en.bitcoin.it/wiki/Transaction

Blockchain.com, 2023. URL: https://www.blockchain.com/explorer/blocks/btc/818534

Cryptopedia, 2023. How a Block in the Bitcoin Blockchain Works. URL: https://www.gemini.com/cryptopedia/what-is-block-in-blockchain-bitcoin-block-size

Frankenfield 2022, What Is a Block in the Crypto Blockchain, and How Does It Work?. URL: https://www.investopedia.com/terms/b/block-bitcoin-block.asp

Javatpoint 2023, Blockchain block hashing. URL: https://www.javatpoint.com/blockchain-block-hashing

Karvinen, 2023. Trust to Blockchain 2023 autumn. URL: https://terokarvinen.com/2023/trust-to-blockchain/

Kuttler, 2023. URL: https://kuttler.eu/en/bitcoin/btc/faucet/success/

Nakamoto, 2008. Bitcoin: A Peer-to-Peer Electronic Cash System. URL: https://bitcoin.org/bitcoin.pdf

Reserve bank of Australia, 2023. Digital Currencies. URL: https://www.rba.gov.au/education/resources/explainers/cryptocurrencies.html
