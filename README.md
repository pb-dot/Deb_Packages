# Deb_Packages
This is an Online repo for my debian packages

## How to use my FTP server and client 

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
