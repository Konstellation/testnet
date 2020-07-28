# Konstellation Testnets

This repo collects the genesis and configuration files for the various Konstellation
testnets. It exists so the [Konstellation](https://github.com/konstellation/konstellation)
repo does not get bogged down with large genesis files and status updates.

## Getting Started

To get started with the latest testnet, see the
[docs](https://github.com/Konstellation/konstellation#to-join-testnet-follow-this-steps).

## Testnet Status

⚠️ Latest testnet: [knstlhub-1](./knstlhub-1) ⚠️

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