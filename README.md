[Aleo](https://www.aleo.org) is a new layer-1 blockchain platform for creating scalable and private applications applying zero-knowledge cryptography. Aleo uses a hybrid consensus architecture named AleoBFT, which leverages PoS to achieve instant finality for block confirmation, and leverages PoW “coinbase puzzle” that rewards the development of faster techniques for proof generation.

Mining rewards will be settled daily as credits, according to the payout scheme of PPLNS, and then accrue in your zkfab account. Adding of wallets and reward withdrawals are currently not supported, we will send payouts according to Aleo’s follow-up post about the details of the incentives. Please stay tuned for our further announcement.

Please follow the steps below for detial tutorial.

### **1. Obtain suitable hardware and software**

Aleo can be efficiently mined with NVIDIA GPUs. For each GPU, you may get the following ready:
- GPU: NVIDIA GPU with driver version 515 or above.
- CPU: 8-core CPU
- Memory: 8 GB
- SSD storage: 128 GB
You need to get the Ubuntu 18.04-20.04 (version for servers, without GUI) operation system ready, and install this mining software (download).
Minging Software: https://github.com/zkfab

### **2. Sign up for an zkfab account**

You will need to create an zkfab account before mining Aleo on its testnet 3. If you do not have one yet, please click [here](https://zkfab.io/#/usr/reg) to register.
After logging in to the account, you can configure mining parameters in Profile >  Worker Configuration.

### **3. Configure mining software**

#### 1)Upload mining software to the servers
Use a file transfer tool such as xftp to transfer the minging software to the specified directory of the server device (such as the **/opt** directory)

#### 2)Unzip the software installation package
```
cd /opt
tar -xvmf aleo_prover--version.tar.gz
```

#### 3)Change the config.yaml configuration file
```
cd /opt/aleo_prover/conf
ls 
vim config.yaml
```
**Note:**
1) The API Key can be obtained from the "Profile>Worker Configuration" of the zkfab.
2) Operator address is the Domain Name or IP address provided by zkfab. The default port is to 41326, and it does not need to be modified.
3) Execute "install.sh" script
```
cd /opt/aleo_prover
chmod +x install.sh
./install.sh
```
Now the deployment is completed!

### **4. Start Mining**

Your machines are now ready to mine! You can monitor your hashrate, rewards and so on in zkfab.\
To stay updated with the latest Aleo news and developments, follow us on [Twitter](https://twitter.com/zkfab)!\
Happy mining!
