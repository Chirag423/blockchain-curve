# Creating a ERC-20 Token

1. Create an account on a crypto wallet(Meta Mask) to store your token.
2. To create a ERC-20 token you need to deploy ERC-20 smart contract, which you can either write yourself or do it with the help of [20 Lab](https://20lab.app/generate/general)
3. To mine your token it will charge you some gas fee in the form of goerli testnet.
> **Note:**
>  If you don't have Goerli Testnet, you can mine them from [here](https://goerli-faucet.pk910.de/)

After your Token is formed, you can check it on [etherscan.io](https://etherscan.io/)

![Screenshot 2023-07-01 024549](https://github.com/Chirag423/blockchain-curve/assets/118429338/c27235c2-ba4c-413b-b5de-63ccd2d5fdcc)


# Hyperledger-Fabric
To initiate Hyperledger-Fabric follow the steps:

### Prerequisites:
* Install Docker and Docker Compose on your machine.
* Install Go programming language.
* Install Node.js and npm (Node Package Manager).
* Install Hyperledger Fabric binaries and samples.

### Install Docker
```
sudo apt-get -y install docker-compose
```
### Install Golang-Go
```
sudo apt install golang-go
```
### Install jq
```
sudo apt install jq
```
### Install Node/Java
```
sudo apt install npm
npm install node
```
### Install Fabric Sample Repo
```
curl -sSLO https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/install-fabric.sh && chmod +x install-fabric.sh
```

Then you can pull docker container by running this command.
```
./install-fabric.sh d s
```
To install binaries for Fabric samples you can use the command below:
```
./install-fabric.sh binary
```

## Build your first network

### Bring up the test network

You can find the scripts to bring up the network in the test-network directory of the fabric-samples repository. Navigate to the test network directory by using the following command:
```
cd fabric-samples/test-network
```

From inside the test-network directory, run the following command to remove any containers or artifacts from any previous runs:
```
./network.sh down
```

You can then bring up the network by issuing the following command. You will experience problems if you try to run the script from another directory:
```
./network.sh up
```

