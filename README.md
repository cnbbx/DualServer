# DualServer
中国百宝箱专用DCHP和DNS服务器中文美化版

##Windows Compiling 
It is not needed to recompile Dual DHCP DNS Server on windows version. 64 bit versions can also run this 32 bit executable.  However the command for compiling is: 
```bash
g++ -o DualServer.exe DualServer.cpp -lwsock32 -liphlpapi -lws2_32 
```

##Linux Compiling 
The enclosed dualserver executable file may only run on Intel Linux 32 bit version. For 64 bit Linux system, you can try:
 
```bash
#g++ dualserverd.cpp -odualserverd -lpthread
#g++ dualserverd.cpp -odualserverd -lpthread -lgcc_s 
```

Fork of https://sourceforge.net/projects/dhcp-dns-server/
