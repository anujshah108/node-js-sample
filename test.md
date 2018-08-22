## Explaining Gas

### The EVM

The Ethereum Virtual Machine (EVM) is a part of the software running the Ethereum protocol. This EVM is what executes smart contracts on every node in the network. This execution is not free for the miners/nodes - they spend a lot of electricity to do this. Therefore for each transaction, a small amount of "gas" is needed to compensate the miners. 

### Gas
Gas is the unit of cost to successfuly execute a transaciton onto the Ethereum blockchain. 

For example:

- To simply send one transaction ($ from A to B) it costs 21000 gas
- To compare two integers it costs 3 gas
- To create a new contract it costs 32,000 gas
- To save 1 MB to storage (31250 256-bit words) it costs 625000000 gas!

It is also important to note the units of Ether. The smallest unit of either is Wei, where 1000000000000000000 equals 1 Ether. 

Gas cost varies with the traffic of the network. Currently at the time of writing this (8/22/18) - the current gas cost is 3.7 Gwei. Where 1 Gwei is one billionth of 1 Ether. So for example to send one example at 21000 gas where each gas cost 3.7 Gwei, at the current ether price of $277 - the transaction costs roughly $0.21. 

### Altering Gas Limit

The gas cost of a transaction, referencing again the tranaction we used above ($ from A to B), is automatically estimated in tools like MetaMask. 

<img src="https://cl.ly/f2bc771786cc"
     alt="Markdown Monster icon"
     style="float: left; margin-right: 10px;" />

We have the option to send less gas than the estimate but if the gas provided is less than what is actually needed, we lose the gas we gave and the transaction fails. 

If we send more has than what is needed in the transaction - the remainder it is refunded to us.

We can increase the gas limit like so:

https://cl.ly/653cadfcc03d

We can see in the above images how increasing the gas limit increases the transaction fee. In this case anything unused will be refunded back to us. That is not the case when altering gas price. 

#### Altering Gas Cost

For the most part if we are not in a rush to process our transaction we can usually leave the gas price at the amount that was estimated. 

https://cl.ly/1c7313c34767

But say for example we are in a rush because we are trying to send money to a website to buy tickets before anybody else.

In this case we can increase the gas price we are willing to pay. In this case the amount of gas used will remain the same but the amount you pay for it will increase. This higher transaction cost ultimately persuades miners to execute your transaction before others on the network and therefore increasing the speed of the transaction. In this case the extra money spent goes to the miner and is not refunded to the user. 

Example here:

https://cl.ly/6baa42192d53


 
