### Objective
To block domains using the /etc/hosts file.
***
### How
The `/etc/hosts` file contains the IP host names and addresses for the local host and other hosts in the internet network[^1]. 

This works by specifying 0.0.0.0 / 0.0.0.1 as IP address for the hostname explicitly in the /etc/hosts file.

So the resolver will use IP address specified in this file instead.
***
### Steps
1.	Open terminal and run the following command:
![42b54e09cef9ae45d7812a26bd30caa8.png](./_resources/42b54e09cef9ae45d7812a26bd30caa8.png)
![63b6d0d0ec37990d15830c8c0724ccae.png](./_resources/63b6d0d0ec37990d15830c8c0724ccae.png)

2.	Give 0.0.0.0/0.0.0.1 as IP address for domain that you want to block.
![617eaa5313356ff8fbfcd0d3914d9868.png](./_resources/617eaa5313356ff8fbfcd0d3914d9868.png)
3. Verify using dig:
![3764f06a8ddf81a7a9d978dfffb82a2b.png](./_resources/3764f06a8ddf81a7a9d978dfffb82a2b.png)
4. Restart browser if domain remains unblocked.

[^1]:https://www.ibm.com/docs/en/aix/7.2?topic=formats-hosts-file-format-tcpip
