# Archway Network Testnets

Configurations and instructions for connecting to **testnet** networks of Archway Network (Cosmos SDK).

## Quick connection

1. Clone repository
```bash
git clone https://github.com/arl-dev-py/archway-network-testnets.git
cd archway-network-testnets
Download genesis + node config

bash
# Main testnet
curl -o testnet-1/genesis.json https://testnet-1.archway.network/genesis.json
curl -o testnet-1/config.toml https://testnet-1.archway.network/config.toml

# Or all testnets at once
./download-all-testnets.sh
Run node

bash
# Install Archway binary
curl -sSfL https://raw.githubusercontent.com/archway-network/mainnet/main/install.sh | bash

# Add to PATH
export PATH=$PATH:~/.archway/bin

# Start node sync
archwayd start --home testnet-1

---

# Archway Network Testnets 

Конфигурации и инструкции для подключения к **testnet** сетям Archway Network (Cosmos SDK).

## Быстрое подключение

1. Клонировать репозиторий
git clone https://github.com/arl-dev-py/archway-network-testnets.git
cd archway-network-testnets

2. Скачать genesis + node config
# Основной testnet
curl -o testnet-1/genesis.json https://testnet-1.archway.network/genesis.json
curl -o testnet-1/config.toml https://testnet-1.archway.network/config.toml

# Или все testnets сразу
./download-all-testnets.sh

3. Запустить ноду
# Установить Archway binary
curl -sSfL https://raw.githubusercontent.com/archway-network/mainnet/main/install.sh | bash

# Добавить в PATH
export PATH=$PATH:~/.archway/bin

# Запустить синк ноды
archwayd start --home testnet-1

