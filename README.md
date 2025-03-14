# Deb_Packages
This is an Online repo which contains the following debian packages created by me
1. **Retro_X85_Emu.deb : Intel 8085A Emulator with Dark Themed Retro Style UI**
2. **fbi.deb : Linux Packet Sniffer**
3. **prithi-ftp.deb : custom FTP server client**
4. **pbChat.deb : One to One Chat App**
5. **pbShell.deb : Minimalistic Shell for Linux**

## Installation Steps : Intel 8085A Emulator with Dark Themed Retro Style UI

#### To Know What it does, its Details, its Code_Base and Features of this software <a href="https://github.com/raj-shahh/Retro-X85-Emulator">Click Here</a>

#### Download Retro_X85_Emu.deb  from this repo

#### Install & Uninstall the .deb Package :-
    sudo dpkg -i Retro_X85_Emu.deb // install
    sudo dpkg -r retro-x85-emu     // remove

#### Verify Succesfull Install of Deb pkg (check below dir structure exists):-
    /Emu_x85/
    ├── bin/
    │   └── emu
    ├── Config_Rsts/
    │   └── RST_0_1000.asm
    └── egInputs/
        ├── demo1.asm
        └── demo2.op

#### Eg Use the installed deb_pkg :-
    cd /Emu_x85
    ./bin/emu ->Enter to see usage instrction
    // Some example Runs (either do 1> or 2> )->
    1> ./bin/emu 8000 ./egInputs/demo1.asm --one_go ./Config_Rsts
    2> ./bin/emu 1000 ./egInputs/demo2.op --step_wise


## Installation Steps : Linux Packet Sniffer
#### To Know What it does, its Details, its Code_Base and Features of this software <a href="https://github.com/pb-dot/Socket_Programming/tree/main/Fbi">Click Here</a>

1. Download fbi.deb file from this repo
   
2. To install run:
   1. sudo dpkg -i fbi.deb

3. On Succesfull install U will see there is a folder created /fbi

4. Setup :
   1. cd /fbi
   2. to run  use sudo ./fbi -i [interFace Name eg wlo1]
   3. On success 3 report files will be created under /fbi as output

5. To uninstall run:
   1. sudo rm -r /fbi
   2. sudo dpkg -P fbi


## Installation Steps : custom FTP server and client 
#### To Know What it does, its Details, its Code_Base and Features of this software <a href="https://github.com/pb-dot/Socket_Programming/tree/main/FTP">Click Here</a>

1. Download prithi-ftp.deb file from this repo
   
2. To install run:
   1. sudo dpkg -i prithi-ftp.deb

3. On Succesfull install U will see there are 2 folders created /prithiFTP/SERVER and /prithiFTP/CLIENT

4. Setup of server:
   1. cd /prithiFTP/SERVER
   2. There is a file called id_passwd.txt store clients userName and Password there in the format userName/:Password
   3. Create empty dir with same name as client userName for every user u add to this id_passwd.txt file
   4. One demo entry has been kept in the file and corresponding to its userName(demoClient) the directory(demoClient) has been kept
   5. to run the server use ./server.out [serverPort].

5. Setup of client
   1. cd /prithiFTP/CLIENT
   2. run ./client.out [SERVER-IP] [Server-port]

6. To uninstall run:
   1. sudo rm -r /prithiFTP
   2. dpkg -P prithi-ftp


## Installation Steps : one to one Chat App 
#### To Know What it does, its Details, its Code_Base and Features of this software <a href="https://github.com/pb-dot/Socket_Programming/tree/main/one-to-one-Chat">Click Here</a>

   1. Download pbChat.deb file from this repo
   
   2. To install run:
      1. sudo dpkg -i pbChat.deb

   3. On Succesfull install U will see there are 2 folders created /pbChat/Server and /pbChat/Client

   4. Setup of server:
      1. cd /pbChat/Server
      2. to run the server use ./server.out [serverPort].

   5. Setup of client
      1. cd /pbChat/Client
      2. run ./client.out [SERVER-IP] [Server-port]

   6. To uninstall run:
      1. dpkg -P pbChat


## Installation Steps : Minimalistic Shell 
#### To Know What it does, its Details, its Code_Base and Features of this software <a href="https://github.com/pb-dot/pb_shell">Click Here</a>

   1. Download pbShell.deb file from this repo
   
   2. To install run:
      1. sudo dpkg -i pbShell.deb

   3. On Succesfull install pbShell exe is created under /usr/bin.
   
   4. Type pbShell in terminal to access my shell from anywhere
   
   5. To uninstall run:
      1. dpkg -P pbShell
