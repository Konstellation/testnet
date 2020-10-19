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

# How to use keybase

The `keybase ID` is a 16-digit string that is generated with a keybase.io account. It's a cryptographically secure method of verifying your identity across multiple online networks. The Keybase API allows us to retrieve your Keybase avatar. This is how you can add a logo to your validator profile

1. Go to https://keybase.io/
2. Click `login`，then` Join Keybase` and finish the sign up process
3. Click `add a PGP key`，then choose `I need a public key`，then click `Ok，got it`。
4. After filling the form, you should click on `Let the math begin`，then you could get your own key, then the whole registration process is finished. 

# How to finish tasks in Konstellation testnet

You need to use keybase to generate your own [pgp fingerprint](https://github.com/Konstellation/testnet/blob/master/How%20to%20use%20keybase.md) first. 

You have to fill in this [form](https://forms.gle/L1n9bacVSxEJm8GF9) to complete your sign-up process. 

The instructions are the following: 

## Tasks for knstlhub-1

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
