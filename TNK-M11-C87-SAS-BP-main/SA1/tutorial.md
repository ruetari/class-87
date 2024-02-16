SA1

Create a Genesis Block
======================


In this activity, you will learn to create a new blockchain, beginning with a genesis block, and print the information within the chain.




<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10642051/SA1.gif" width = "480" height = "320">




Follow the given steps to complete this activity.
1. Create a genesis block


* Open the file blockchain.py.


* Create a Block chain class and a list object variable.

    `class BlockChain:
        def __init__(self):
            self.chain = []`


* Define a method to create a genesis block. Create a new object of the class Block with index=0, timestamp, an empty transaction, and the previous hash. Add a message to inform the user that the previous hash will not be present as this is the genesis block.


    `def createGenesisBlock(self):`
    `genesisBlock = Block(0, time(), [], "No Previous Hash Present. Since this is the first block.")`


* Append the genesis block to the block chain list.


    `self.chain.append(genesisBlock)`

* Print the information of all the blocks by looping through the chain.

    `for block in self.chain:
                print("Block Index", block.index)
                print("Timestamp", block.timestamp)
                print("Transaction", block.transaction)
                print( "Previous Hash",block.previousHash)
                print( "Current Hash",block.currentHash)
                print("*" * 100 , "\n")`


* Create a new chain and call the methods to create a genesis block and print the block chain.

    `chain = BlockChain()`
    `chain.createGenesisBlock()`
    `chain.printChain()`

* Save and run the code to check the output.
