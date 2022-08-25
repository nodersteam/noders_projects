# Stride's Testnet - PoolParty

This contains instructions for how to connect to Stride's testnet, PoolParty!

We've tried to keep the instructions as simple as possible, but if you have any questions, please don't hesitate to contact us over [email](mailto:hello@stridelabs.co), on [Twitter](https://twitter.com/stride_zone), or at our [Discord](https://stride.zone/discord).

Requirements for this testnet are quite minimal. You should have a 4 CPU 32 GB RAM machine. We've only tested this build on OSX and Linux machines, but we hope to support Windows soon.

## Installation

Run the following command to install PoolParty

```bash
bash -c "$(curl -sSL install.poolparty.stridelabs.co)"
echo "OK"
```

## Upgrade

If you've installed Poolparty with the standard install script, please run 

```bash
bash -c "$(curl -sSL https://raw.githubusercontent.com/stride-labs/testnet/main/poolparty/upgrade.sh)"
echo true
```
