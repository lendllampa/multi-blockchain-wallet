# Unit 19: Multi-Blockchain Wallet in Python
---
This wallet uses BIP44 to give users the ability to send multiple coins using only **one** mnemonic phrase. You can derive multiple addresses and their corresponding Public and Private Keys by using the ```derive_wallet()``` function and passing in a ```mnemonic phrase```, ```coin```, and a ```numderive```, for the number of derived addresses you would like. 


### Test Transactions
---
##### ETHEREUM
``` send_tx(ETH, priv_key_to_account(ETH,coins[ETH][0]['privkey']), priv_key_to_account(ETH,coins[ETH][1]['privkey']), 1) ```

![mycrypto_txhash](Screenshots/mycrypto_txhash.png)
The following photo is a screenshot from the local Ethereum Node that states the txhash and recipient
![node1_txhash](Screenshots/node1_txhash.png)

##### BTCTEST
``` send_tx(BTCTEST, priv_key_to_account(BTCTEST,coins[BTCTEST][0]['privkey']), priv_key_to_account(BTCTEST,coins[BTCTEST][1]['privkey']), 0.000001) ```

![btctest_tx](Screenshots/btctest_tx.png)
Transaction hash from the bottom photo matches the hash from the BitcoinTest Explorer
![btctest_ipynb_output](Screenshots/btctest_ipynb_output.png)

