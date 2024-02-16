SA2
Add a New Block
===============


In this activity, you will learn to create a new block and attach it to the blockchain.




<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10642088/SA2.gif?raw=true" width = "480" height = "320">




Follow the given steps to complete this activity.
1. Create a new block


* Open the file blockchain.py.


* Create a new block.


    `def addBlock(self, newBlock):`


* Create a genesis block if the chain is new.


    `if(len(self.chain) == 0):` 
    `self.createGenesisBlock()`


* Set the previous hash in the new block.
Get the currentHash of the last block of the chain and use it as previousHash in newBlock.


    `newBlock.previousHash = self.chain[-1].currentHash`


* Calculate the Hash of the newBlock and save it in the currentHash of the newBlock.


    `newBlock.currentHash = newBlock.calculateHash()`


* Append the newBlock to the chain.


    `self.chain.append(newBlock)`


* Replace creation of the genesis block chain.createGenesisBlock() with adding newBlock in the blockchain.


    `chain.addBlock(newBlock)`


* Save and run the code to check the output.