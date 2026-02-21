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

