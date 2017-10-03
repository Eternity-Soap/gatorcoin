As of October, the blockchain has completely stagnated and the nodes that were holding the network together with toothpics and glue failed and went offline. As such, gatorcoin is dead for all intents and purposes. If you want to play with the source code and attempt to resurrect it, feel free.

Copyright (c) 2009-2014 Bitcoin Developers Copyright (c) 2011-2014 Litecoin Developers (c) 2017 Florida Man 

# What is Gatorcoin?
Gatorcoin is a very simple clone of Litecoin, a Bitcoin derived cryptocurrency. If you don't know what a cryptocurrency is, the short description is a digital currency that uses cryptography and a special piece of technology known as the blockchain to avoid a central authority. While Gatorcoin functions pretty much identically to Litecoin, it has a completely independent blockchain and network. Gatorcoin is based off of the contemporary (v0.14.2) Litecoin client.

# [Latest Release](https://github.com/schyczewski/gatorcoin/releases/tag/v0.14.2)

# Gatorcoin Properties:
- P2P port is 1853 after year of school's founding
- Initial mining reward of 16 coins per block (one for each of UF's colleges)
- 8 minute block targets (after the 8 libraries on campus)
- Difficulty retarget every 90 blocks (about half of a day)
- Reward cut in half every 262.8k blocks, about 4 years
- Maximum coin supply will about 8146800 coins, and will be reached in 20 years
- Mined coins take 50 blocks to mature
- Addresses start with a "G"
- Probably better than an FSU equivalent

# Getting Gatorcoin

Simply go to the release page linked above download the appropriate file for your operating system and architecture. 

### Windows Users: 
If you're running an up to date version of Windows 10 and in some cases 8, Windows defender will almost certainly try to stop you from running the program. This is because I have not bought a special certificate to sign the software and make windows happy. If you like, you can point an antivirus at the thing and you should find that everything is in order. The warning can be ignored by simply clicking on the more info button on the blue window that will pop up and telling the program to run anyway. 

### Linux Users:
The release package comes only with binaries that need to be started from the command line. To run the GUI, extract the release package and run gatorcoin-qt. If you would like to compile the code yourself and create an install, instructions to do so can be found [here](doc/build-unix.md).

### OS X Users:
Upon downloading and opening the .dmg, just drag Gatorcoin-Qt.app into the Applications folder and you're good to go.

# So.. What do I do with this?
If you've ever wanted to learn more about cryptocurrencies, this one should do fine for getting some first hand experience with them. If you're like me and wanted to know what it was like to be able to solo mine one that was bitcoin derived, than go at it! Other than that though, use it for whatever you like, whether that be turning it into a meme, some sort of inside joke or a fun commodity. Use your *imagination* or something. 

Also, as an important piece of information to new users: if you connect to the network and your client seems to get stuck synchronizing (i.e. no change for more than a minute) there's a good chance that a new block hasn't been mined in a couple of hours. As soon as a new block is mined either by you or someone else on the network, you will be synchronized. 

# I like this, how can I help?
Well, you can start by telling your friends and having their friends tell their friends etc... If you're familiar with the process, you could also make a bunch of paper wallets to throw at people in Turlington. Also, a healthy network will have a large amount of peers as well as enough miners to keep a steady hashrate. If you've got a small computer or something like a raspberry pi that you are not using, you can point it at the gatorcoin pool to contribute hashing power to the network. Additionally, if you can do it, you could host a node. The process of setting one up is identical to litecoin. If you do decide to host a node, contact me and I will add it to the list of seed nodes.  

Perhaps of highest importance though is actually using it. Gatorcoins aren't doing anyone any good by being stashed away. Have fun with them by accepting/offering them as payment for mundane thing such as help with classwork and such. 

# Other Utilities

## Paper Wallet Generator

I've forked WalletGenerator.net and added Gatorcoin support for those who might want to make them. You will need to download the repository either as a zip file or with the clone command and execute the index.html file that comes with it (this can usually just be done by double clicking on it). If you are unfamiliar with the concept of a paper wallet, a cryptocurrency wallet is composed of two keys: a public key (your receiving address) and a private key (used to spend coins). A paper wallet is literally a piece of paper with this information recorded, usually also accompanied by QR codes to quickly get the keys in a digital format. To access the funds on a paper wallet, go to the debug console accessable via the help tab of the client and type the collowing command: `importprivkey yourprivatekeyhere`. Note that after this you should discard the wallet. Gatorcoin isn't the default currency (bitcoin is), so you will need to locate Gatorcoin in the list of cryptocurrencies in the lower right of the generator window.

[Wallet Generator](https://github.com/schyczewski/WalletGenerator.net).

## Blockchain Explorer

I've set up an Iquidus block explorer that works with Gatorcoin. For those who don't know, a block explorer allows you to see all of the transaction on the network, how many per block, the richest addresses on the network, etc. They can be useful for determining if a transaction you sent was properly confirmed as well as do things such as see the amount stored on a paper wallet.

[Block Explorer](http://165.227.127.93:3001/)

## Mining
If you aren't familiar with the term, mining is the process by which the network of cryptocurrencies like gatorcoin process transactions and ensure integrity. Without miners, the network will stagnate and die. The main incentive for mining is receiving newly generate Gatorcoins. As mentioned above, each block found yields 16 new coins that go the the person(s) who generated it. If you're interested in mining, I've created a guide below for you to use.   

[Mining Instructions](doc/mining.md)

[Gatorcoin Mining Pool](http://165.227.127.93/)
