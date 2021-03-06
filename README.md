# coursera_BitcoinAndCryptocurrency
Coursera course which teaches the fundamentals of cryptocurrencies.
https://www.coursera.org/learn/cryptocurrency/

There are three assignments in Java which implement a [transaction handler](https://github.com/adagiox/coursera_BitcoinAndCryptocurrency/blob/master/Assignment1/TxHandler.java), a [compliant node](https://github.com/adagiox/coursera_BitcoinAndCryptocurrency/blob/master/Assignment2/CompliantNode.java), and a [blockchain full node](https://github.com/adagiox/coursera_BitcoinAndCryptocurrency/blob/master/Assignment3/BlockChain.java) which handles the blockchain data structure. Each assignemnt contains some starter code.


<p1><b>Assignment 1:</b></p1>
The goal of Assignment 1 is to implement a transaction handler class which will take an array of incoming transactions and return an array of valid transactions of maximal size. To validate incoming transactions in our bitcoin-like model, we must check that for each input there exists a UTXO (unspent transaction output) in the current UTXO pool, validate the signatures on each input of the transaction, make sure each UTXO is only claimed once, and validate the input and output values (bitcoins) of each of the transactions inputs and outputs. 


<p1><b>Assignment 2:</b></p1>
The goal of Assignment 2 is to implement a CompliantNode class for a distributed consensus simulation in a bitcoin-like directed random graph environment. The simulation constructs a network consisting of either malicious nodes or compliant nodes based on a specified probability. The compliant nodes should (attempt to) come into consensus regardless of the network topology, number of malicious nodes, and distribution of transactions across the initial state of the network before propagation. 


<p1><b>Assignment 3:</b></p1>
Assignment 3 builds off of the concepts of the previous assignment to construct a functional node in our blockchain network. The node will store the blockchain and be able to update its blockchain, transaction pool, and unspent transaction pool as new blocks are announced to the network. The design of the class efficiently stores blocks, creates an easily traversable and verifiably blockchain, handles forking, and easily adds the coinbase transaction to newly mined blocks. 
