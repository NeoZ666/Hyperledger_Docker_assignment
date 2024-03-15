# SimplyFI_assignment
1. Steps for installing and instantiating the Chain code on HLF2.2
  ![container](image.png)
  ![images](image-1.png)
  ![terminal](image-2.png)
  ![terminal2](image-3.png)
  
2. Explain Cryptogen and Configtxgen
Cryptogen and Configtxgen are two command-line tools provided by Hyperledger Fabric.

a. Cryptogen: Cryptogen is used to generate the cryptographic materials required for setting up a Hyperledger Fabric network. It generates key pairs and X.509 certificates for organizations, peers, orderers, and other network entities.
```
cryptogen generate --config=./crypto-config.yaml
```

b. Configtxgen: Configtxgen is used to generate the configuration artifacts required for creating and updating a Hyperledger Fabric network. It generates the genesis block, channel configuration transactions, and anchor peer updates.
```
configtxgen -profile MyChannel -outputCreateChannelTx ./channel-artifacts/mychannel.tx -channelID mychannel
```

### ADDING RELAVENT FILES FOR Q3
3. Develop a chaincode for storing the data in to blockchain
a. Store
b. Retrieve
c. Update
d. GetHistory
e. GetbyNonPrimaryKey (Using CouchDB Rich Queries)
