Gatorcoin can be mined in the same ways as any other bitcoin based scrypt coin. If you know how to mine Litecoin, than you are all set. If you don't know, than prepare to learn. 

## CPU Mining
Because of the truly enormous hash rates present on the networks of noteworthy cryptocurrencies, CPU mining won't get you very far with them. With Gatorcoin, however, CPU mining can yield new blocks just fine. The best cpu mining software by a longshot is pooler's [cpuminer](https://sourceforge.net/projects/cpuminer/files/). It is available on Windows, OS X, and Linux. As a heads up, many antivirus programs will think that mining programs are trojan viruses (including avast for students using it). This is probably due to the fact that in the age of cryptocurrency many viruses have been created to use the host computer as a miner. Anyway, cpuminer is used via the command line. To use it, navigate to the directory where the program is stored in the terminal/command prompt. For a list of options, you can use `miner -h`, where "miner" is the name of the program. On linux and mac this will just be "minerd" whereas on windows it will be "minerd.exe".

## GPU Mining
In the very early days of Bitcoin and up until just recently with most scrypt coins, mining with a rig made of gaming GPUs was the way to do it. Thanks to the development of machines specifically built to mine however, it has been impractical to mine Bitcoin at home for quite some time even with your own ASIC, and lately ASICs built for scrypt have been bringing the same thing to Litecoin. However, given the Gatorcoin network difficulty as of this writing GPUs should work great. You will need to find mining software that is compatable with your GPU and operating system. In the case of NVIDIA GPUs, I recommend this incarnation of [ccminer](https://github.com/tpruvot/ccminer/releases). It is almost identical to cpuminer in terms of use, and as a matter of fact you can follow the below example down to the command line arguments to get started. 

### Example: Pool mining with cpuminer/ccminer
Just for fun, I've launched a pretty basic uNOMP mining pool that supports Gatorcoin. The pool's webpage can be seen [here](http://165.227.127.93/). It is quite simple to use. Once you've got your choice of miner, you will need to get an address for the reward to be sent to once the blocks are all locked in and the pool decides that it is time to pay out. Just fire up your client and go to the receive tab. I recommend entering a label such as "Gator pool payout" or something similar so you can keep track of it. Leave the other fields blank and press the request button. A window will pop up. From there press the copy address button and you've got a receiving address you can use. Now it's time to start the miner. First, navigate to the directory where the executable is installed. On all three operating systems this can be done by going into the command interface, typing "cd" and then dragging the folder with the executable in it over the terminal window and then pressing enter.


In order to solo mine, you will first need to configure your client correctly. In order to do this, you will need to create a file name "gatorcoin.conf" in the application data directory. On Ubuntu, this is a hidden folder called .gatorcoin in your home directory. On windows, this is a folder called Gatorcoin located in the %appdata% directory. Create gatorcoin.conf and add the following:

```
server=1
rpcuser=someusername
rpcpassword=yourrpcpass
rpcport=14300
rpcallowip=127.0.0.1
```
Remember those login credentials, as you will need them for the miner. After you've done that and restarted your wallet, you're ready to mine. Navigate to the cpuminer directory in your terminal and enter the following:

`miner -a scrypt -o 127.0.0.1:14300 -O someusername:yourrpcpass`

Executing that command will fire up the miner and starting using all available cpu threads to mine. If you like, you can specificy the amount of threads you'd like to use by appending `-t <threads>` to the command. When you've had enough, simply use control-C while in the terminal window to terminate the program. 
