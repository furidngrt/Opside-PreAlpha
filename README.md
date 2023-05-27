# Install Incentivized Pre-alpha Testnet

Opside is a decentralized ZK-Rollup-as-a-Service (ZK-RaaS) network, founded on the modular blockchain concept. By developing a sophisticated three-layer blockchain architecture, Opside combines the strengths of Proof-of-Stake (PoS) and Proof-of-Work (PoW) consensus mechanisms. This innovative design offers Web3 developers a robust and feature-rich zkEVM chain, which can be effortlessly generated with just a single click.


### Update 
```
sudo apt update && apt upgrade -y
```

### Install Prerequisites
```
sudo apt install pkg-config curl git build-essential libssl-dev libclang-dev cmake ufw screen
```

### Install auto-program
```
wget -c https://pre-alpha-download.opside.network/testnet-auto-install-v2.tar.gz 
```
```
tar -C ./ -xzf testnet-auto-install-v2.tar.gz
```
```
chmod +x -R ./testnet-auto-install-v2
```
```
cd ./testnet-auto-install-v2
```
### Install validator clients
```
./install-ubuntu-en-1.0.sh
```
Follow the CLI prompts to generate your keys. You will need to enter:
1. Your withdrawal Opside address(which is used to receive your validator rewards and your deposit when you exit)
2. Password(which is used to encrypt your validator signing key)
3. Repeat your withdrawal Opside address
4. Repeat your Password
Then there will be 24 mnemonic seed phrases. This is highly sensitive and should never be exposed to other people or networked hardware.

### Check the logs
```
opside-chain/show-geth-log.sh
```
```
opside-chain/show-beaconChain-log.sh
```
```
opside-chain/show-validator-log.sh
```
### Upload deposit file

If you are using MobaXTrem please download the Deposit file located at `/root/testnet-auto-install-v2/validator_keys/`
![Screenshot_2](https://github.com/furidngrt/Opside-PreAlpha/assets/63885192/e687ad8a-0e0c-40fa-88a0-88574da2e9d1)

then please upload it here https://opside.network/validator/deposit
![Screenshot_3](https://github.com/furidngrt/Opside-PreAlpha/assets/63885192/6a883979-461d-4125-b07a-b348cdcdc3d5)

### Connect wallet and confirm deposit

