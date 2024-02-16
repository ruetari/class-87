AA1

Create a separate class
=====================


In this activity, you will learn to create a separate class for creating the genesis block.




<video src= "https://s3.amazonaws.com/media-p.slid.es/videos/1525749/EVpcfxt-/sa3.mp4" width = "480" height = "320"></video>




Follow the given steps to complete this activity.
1. Create a separate class for creating the genesis block.


* Open the file blockchain.py.


* Create the genesis class.


    `class Genesis:`


* Define the __init__ method.


    `def __init__(self):`


* Pass the block's transaction information to toggelInfoSection() function, that is - sender, receiver, and amount.


    `,'{{block.transaction['sender']}}',		'{{block.transaction['receiver']}}',		'{{block.transaction['amount']}}'`


* Set index, transaction, timestamp, previousHash, and currentHash object variables.
 
    `self.index = 0
    self.transaction = []
    self.timestamp = time()
    self.previousHash = "No Previous Hash Present. Since this is the     
                        first block."
    self.currentHash = ""`


* Call the genesis class from the createGenesisBlock() function to create a genesis block. Replace genesisBlock = Block(0, time(), [], "No Previous Hash Present. Since this is the first block.") with the code given below:


    `genesisBlock = Genesis()`


* Save and run the code to check the output.