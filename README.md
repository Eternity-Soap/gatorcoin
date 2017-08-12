Copyright (c) 2009-2014 Bitcoin Developers Copyright (c) 2011-2014 Litecoin Developers (c) 2017 Florida Man

# What is Gatorcoin?
Gatorcoin is a very simple clone of Litecoin v0.8.7.5. While it functions almost identically to Litecoin, its network and blockchain are completely independent. It came into being when I decided to make a cryptocurrency clone to see if I could and made it UF themed because why not. 

# [Latest Release](https://github.com/schyczewski/gatorcoin/releases/tag/v0.1)

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

## Windows
Simply download the zip file on the release page and run the installer. Upon first launch the program will likely take a minute or two to link up to the network by itself seeing as how there is only one node at the moment. 

**WINDOWS 10 AND 8 USERS:** because I didn't buy a certificate and go through the codesigning process to make windows happy, Windows Defender will almost certainly try to stop you from running the program. You can ignore it by simply clicking the more info button on the blue window that pops up and running anyway. If it puts your mind at ease, you can aggressively scan the thing with your antivirus and you should turn up nothing. 

## OS X 
Because Litecoin v0.8.7.5 was the version in use 4 years ago, most of the dependency versions that I would need to make an OS X release are dated and it would be more trouble than it's worth to try and make one. However, if you are on OS X and will still like to use this, [WineBottler](http://winebottler.kronenberg.org/) works well with Gatorcoin. When you start it up, go to the "advanced" tab and select the Gatorcoin windows executable. If you don't already have Wine on your system, you'll need to check the box that includes Wine binaries. Everything else can be ignored. 

## Linux
Because the Ubuntu suite that I would need to successfully make Linux binaries has reached EOL, I don't have any nice and easy installer for you to run. However, you are a Linux user, no? You practically live to compile your own software. Instructions to compile Gatorcoin can be found [here](doc/build-unix.md). Trust me, it's not that tricky. 

# So.. What do I do with this?
If you've ever wanted to learn more about cryptocurrencies, this one outta do fine for getting some first hand experience with them. If you're like me and wanted to know what it was like to be able to solo mine one that was bitcoin derived, than go at it! Other than that though, use it for whatever you like, whether that be turning it into a meme, some sort of inside joke or a fun commodity. Use your *imagination* or something. 

Also, as an important piece of information to new users: if you connect to the network and your client seems to get stuck catching up (i.e. no change for more than a minute) there's a good chance that a new block hasn't been mined in a couple of hours. As soon as a new block is mined either by you or someone else on the network, you will be synchronized. 

# I like this, how can I help?
Well, you can start by telling your friends and having their friends tell their friends etc... A healthy network will have a large amount of peers as well as enough miners to keep a steady hashrate. Perhaps of equal importance however would be node hosting. Without plenty of nodes, clients will have a hard time connecting to the network. As of this writing there are only one or two, and if they go down new clients will not be able to connect to the network automatically. If you have an old computer or something like a raspberry pi you can host a node quite easily on a windows or linux system. Setting up a Gatorcoin node is the same for bitcoin/litecoin, so if you need help a google search should do the trick. Just remember what version of litecoin Gatorcoin is based off of and that you will need to open port 1853 on your network. If you do decide to host a node, contact me and I'll hardcode it into the software so that new clients can connect to it. 

## Mining
Before I go any further: In case it needs to be said, DO NOT abuse the poor CISE equipment to mine this. 

[Mining Instructions](doc/mining.md)
