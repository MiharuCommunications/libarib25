Prepare  
install PCSC-Lite https://github.com/LudovicRousseau/PCSC  
install CCID https://github.com/LudovicRousseau/CCID  
scrambled TS file  

Usage  
At first you need to know the scramble key of the file which you would like to descramble.  
Please connect a smart card reader and a B-CAS card.  
Please execute the following command and scramble keys, ca system id and cbc init are outputted to text file (scramble_key.txt, ca_system_id.txt, cbc_init.txt).  
b25 -o 1 scrambled.ts descrambled.ts
  
Please disconnect a smart card reader and a B-CAS card.  
Please execute the following command and you can descramble without a B-CAS card.  
b25 -e 1 scrambled.ts descrambled.ts  
-e 1 means parameters which are needed by descrambling are read from text files. 