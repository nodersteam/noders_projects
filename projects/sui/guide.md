# Sui (prepare intensivized testnet)

Update packages
```bash
apt update && apt upgrade -y
```
Install Docker & Docker-compose
```bash
. <(wget -qO- https://raw.githubusercontent.com/SecorD0/utils/main/installers/docker.sh)
```
Download files for start docker-compose
```bash
mkdir sui && cd sui && \
wget https://raw.githubusercontent.com/MystenLabs/sui/main/docker/fullnode/docker-compose.yaml && \
wget https://github.com/MystenLabs/sui/raw/main/crates/sui-config/data/fullnode-template.yaml && \
wget https://github.com/MystenLabs/sui-genesis/raw/main/devnet/genesis.blob
```
Open ports
```bash
sed -i 's/127.0.0.1/0.0.0.0/' fullnode-template.yaml
```
Start docker-compose and check logs
```bash
docker-compose up -d && docker-compose logs -f --tail 100
```

