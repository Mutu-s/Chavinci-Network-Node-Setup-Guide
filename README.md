# Chavinci-Network-Node-Setup-Guide
 > [Discord](https://discord.gg/nvMtb77G)

CPU: 2 CPU
RAM: 2GB
Depolama: 20-40 GB SSD
      
    wget https://github.com/chavinci-chain/chavinci-releases/releases/download/1.0.3/chavinci-linux.zip
    apt install unzip
    unzip chavinci-linux.zip
    mkdir ~/.chachain
    cd .chachain
    
    nano chachain.conf
        rpcuser=username   
        rpcpassword=password  
        daemon=1
        testnet=1
        staking=1   
    CTRL X + Y ENTER kaydet ve çık
    
     cd .. dedikten sonra ./chad.  düğümü başlat
 
  Peerleri ayarlayalım 
   
    ./cha-cli addnode 157.245.19.145:22833 add
    ./cha-cli addnode 146.190.207.106:22833 add
    ./cha-cli addnode 139.59.207.170:22833 add

 Node SYNC oldu mu kontrol et
   
    ./cha-cli getblockchaininfo
    
  Adres OLUŞTUR

    ./cha-cli getnewaddress
