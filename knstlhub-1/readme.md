# Knstlhub-1

- Go version: [v1.13+](https://golang.org/dl/)
- Konstellation version: [v0.1.30](https://github.com/konstellation/konstellation/releases)

Download the genesis here: [genesis](https://raw.githubusercontent.com/Konstellation/testnet/master/knstlhub-1/genesis.json)
Download the config here: [config](https://raw.githubusercontent.com/Konstellation/testnet/master/knstlhub-1/config.toml)

```bash
$ shasum -a 256 genesis.json
726e0c03ad96afd012af7161af8ed753348e157464951a76830733e7eb49879e  -
```

Persistent peers:

```
1f00c4302bcd6d9240102ce3c6444469e48f176c@node3.konstellation.tech:26656
7e565fdcc27f581abd637e68750664073112081e@node1.konstellation.tech:26656
bf1f16c89dd3cc07e69201e4f7a24a70df556c0c@node2.konstellation.tech:26656
```
```
CHAIN_ID=knstlhub-1
RELEASE=v0.1.30
KONSTELLATION_VERSION=v0.1.30
```

# How to finish tasks in Konstellation testnet

You need to use keybase to generate your own [pgp fingerprint](https://github.com/Konstellation/testnet/blob/master/How%20to%20use%20keybase.md) first. This ID is used to identify yourself in Kontellation incentivized  testnet game. 

You have to fill in this [form](https://forms.gle/L1n9bacVSxEJm8GF9) to complete your sign-up process. 

The instructions are the following: 
For more information, please visit [doc](https://docs.google.com/document/d/1_oAd4pj3v7yyU9akJtTQ9tZQKmgCtDETBHnTU27fEFo/edit?usp=sharing).

## Tasks for knstlhub-1


 | No   | Name                                           | Details                                                      | Criteria                                                     | Reward  |
  | ---- | ---------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------- |
  | 1    | Make a tx between your wallets | Create two wallets. The first *wallet_1* using https://wallet.konstellation.tech and the second one **wallet_2** using `konstellationcli keys add <name>` in the terminal (command line). Export *wallet2* with keystore using `konstellationcli keys export-keystore <name_of_your_key>` in the terminal. Import the *wallet 2* to the http://wallet.konstellation.tech/recover/key/text. Run `send` tx between *wallet_1* and *wallet_2* with your `name-pgpid` as memo | Submit two addresses, tx hash | 50 darc |
  | 2   | Setup a Full node and create a validator                             | set up a full node and use `name-pgp-fingerprint` as `moniker` | Submit your IP and the team could check the configuration of your node | 50 darc |
  | 3   | Withdraw earnings from staking          | Wait until you get the desirable number of tokens and do a withdraw    | Run `withdraw`  transaction with your `name-pgpid` as memo. Submit tx hash and the team could verify the details of transaction | 50 darc |
  | 4   | Unjail your validator      | Shutdown your node and wait until it will be jailed.                            | Run `unjail` transaction with your `name-pgpid` as memo. Submit your transaction hash | 50 darc |
  | 5   | Withdraw earnings #2          | Wait until you get the desirable number of tokens and do a withdraw    | Run `withdraw`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  | 6   | Delegate some **darc** to your validator      | Complete an delegate transaction                           | Run `delegate`transaction with your `name-pgpid` as memo. Submit your transaction hash | 50 iris |  
  | 7   | Withdraw earnings #3          | Wait until you get the desirable number of tokens and do a withdraw    | Run `withdraw`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  | 8   | Redelegate some **darc** from your validator *validator_1* to another *validator_2*           |  Complete an redelegate transaction          | Run `redelegate begin`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  | 9   | Withdraw earnings #5          | Wait until you get the desirable number of tokens and do a withdraw    | Run `withdraw`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  | 10  | Undelegate some **darc** from *validator_2*           |  Complete an undelegate transaction          | Run `begin_unbond`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |*           |  Complete an redelegate transaction          | Run `redelegate begin`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  | 11   | Withdraw earnings #6          | Wait until you get the desirable number of tokens and do a withdraw    | Run `withdraw`  transaction with your `name-pgpid` as memo. Submit tx hash | 50 darc |
  
### How to submit evidence

You could submit the transaction Hash to prove you have finished the tasks above by replying this [issue](https://github.com/konstellation/testnet/issues/1):

```
GitHub ID: XXXX
pgp ID: XXX
Link to your PR
Node URL
Task 3: Hash
Task 4: Hash
...
```
