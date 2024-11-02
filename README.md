Project Name: IMPLEMENTATION OF FTP CLIENT AND SERVER

This zip file holds a repository that implements the FTP Server and Client.

Problem Statement:

Implement a simple version of client/server software. It consists of two programs: FTPClient and FTPServer. 
First, FTPServer is started on a computer. It  listens  on  a  certain  TCP  port  (such  as  5106).  
Then,  FTPClient  is  executed  on  the  same computer;  the  server’s  port  number  are  supplied in the 
command line,  for  example, “ftpclient  5106”.    The  user  can  issue  a  command  at  the  client  side:  “get  <filename>”, 
which is to retrieve a file from the server, or “upload < filename>”, which is to upload a file to the server.
Because the file could be arbitrarily large, you are required to split the file into chunks of 1K bytes and use
a loop to send the chunks, each time one chunk.

Execution:

Compilation steps in cmd:

1. Server -->  javac FTPServer.java
2. Client --> javac FTPClient.java

Running program in cmd:

1. Server --> java FTPServer.java
2. Client --> java FTPClient.java

Test Case1:

Start server
Start client
Enter command: ftpclient 5100 (5100 is the port number. You can try entering invalid commands here)
From the Menu options select 1. Send File 2. Receive File 3. Exit
i. Send file will prompt the user to enter the file name to be uploaded to the server. Enter valid file name to be uploaded here.
ii. Receive file will prompth the user to engter the file name to be downloaded from the server. Enter valid file name to be downloaded here.
iii. Terminate the program.

Note: The files to be uploaded and downloaded should be in the same folder as in the FTPServer and FTPClient java programs. 