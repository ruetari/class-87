AA2

Add the Current Hash of the Genesis Block
================================================


In this activity, you will learn to create the current hash of the genesis block.




<video src= "https://s3.amazonaws.com/media-p.slid.es/videos/1525749/EVpcfxt-/sa3.mp4" width = "480" height = "320"></video>




Follow the given steps to complete this activity.
1. Calculate the current hash of the genesis block


* Open file blockchain.py.


* Define the hash method.


    `def calculateHash(self):`


* Create the blockString variable by concatenating index, timestamp, and previousHash as string.


    `blockString = str(self.index) + str(self.timestamp) + str(self.previousHash)`


* Generate the hash using the generateHash() function and pass the blockstring to it, and then return the result.


    `return generateHash(blockString)`


* Call the calculatehash() method to add the current hash of the genesis block.
 
    `self.currentHash = self.calculateHash()`


* Save and run the code to check the output.