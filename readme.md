# Konstellation Testnets

This repo collects the genesis and configuration files for the various Konstellation
testnets. It exists so the [Konstellation](https://github.com/konstellation/konstellation)
repo does not get bogged down with large genesis files and status updates.

## Getting Started

To get started with the testnet, build from code or install binaries of konstellation with version that corresponds to testnet info

### Build from code

This assumes that you're running Linux or MacOS and have installed [Go 1.14+](https://golang.org/dl/).  This guide helps you:

* build and install Konstellation
* allow you to name your node
* download config file of add seeds to your config file
* download genesis state
* start your node
* use konstellation to check the status of your node.

Build, Install, and Name your Node
```bash
# Clone Konstellation from the release found here: https://github.com/konstellation/konstellation/releases
git clone -b <release> https://github.com/konstellation/konstellation
# Enter the folder Konstellation was cloned into
cd konstellation
# Compile and install Konstellation
make install
```

### Using binaries
# linux
wget [linux](https://gist.github.com/Konstellation/b9168ec665bf8991a1cd20fd999452fa/raw/2c53c4c2fa0d90e7a10a6b7f2b5e28c35bec73d2/linux_amd64.tar.gz)

# macos
wget [macos](https://gist.github.com/Konstellation/b9168ec665bf8991a1cd20fd999452fa/raw/2c53c4c2fa0d90e7a10a6b7f2b5e28c35bec73d2/darwin_amd64.tar.gz)

# win
wget [windows](https://gist.github.com/Konstellation/b9168ec665bf8991a1cd20fd999452fa/raw/2c53c4c2fa0d90e7a10a6b7f2b5e28c35bec73d2/windows_amd64.tar.gz)


### To join mainnet follow this steps
Download Genesis, Start your Node, Check your Node Status
```bash
# Initialize data and folders
# konstellation init {MONIKER} --chain-id {CHAIN_ID}
konstellation unsafe-reset-all
# Download genesis.json
wget -O $HOME/.konstellation/config/genesis.json https://raw.githubusercontent.com/konstellation/testnet/darchub-1/genesis.json
wget -O $HOME/.konstellation/config/config.toml https://raw.githubusercontent.com/konstellation/testnet/darchub-1/config.toml
# Alternatively enter seeds to config.toml provided below.
nano ~/.konstellation/config/config.toml
# Scroll down to seeds in `config.toml`, and add some of these seeds as a comma-separated list:
ba3bacc714817218562f743178228f23678b2873@goz.konstellation.tech:26656
1e63e84945837b026f596ed8ae68708783d04ad4@node1.konstellation.tech:26656
d2d452e7c9c43fa5ef017552688de60a5c0053ee@node2.konstellation.tech:26656
dd36969b56c740bb40bb8badd4d4c6facc35dc24@node3.konstellation.tech:26656

# Name your node
konstellation config set moniker {MONIKER}
# Start Konstellation
konstellation start
# Check your node's status with konstellationcli
konstellationcli status
```