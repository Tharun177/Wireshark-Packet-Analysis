# Wireshark-Packet-Analysis
## steps

- Install ubuntu and windows 10 or 11 to virtual machine
- Now go to settings and Network and select the apadter 2 option and set Internal Network for both Ubuntu and Windows
- Here we are using adapter 2 for conncecting internal network
- Now open ubuntu go to network settings then select adapter 2 settings
- Now go to IPV4 section and select manual and enter an ip address and save the settings
- Here I entered an ip of 10.0.2.50 and subnet 255.255.255.0
- Now similary opne the windows and go to network settings
- Select the adapter 2 settings right click and select the proporties
- select the IPV4 then properties
- Then select use the following IP address option and enter the ip address that relates the previous ip entered in ubuntu
- Here I entered 10.0.2.25 and subnet 255.255.255.0
- Now open the command prompt in windows and try to ping the ubuntu machine be make sure that adaper 1 and adapter 2 options are similar in both cases.
- Also make sure that the firewalls are disabled.
- Next install latest versions of  Wireshark and Putty 
- And install telnet in ubuntu using command : sudo apt install telnetd
- To verify installation use command : sudo dpkg -l | grep telnetd
- Now open Wireshark and select ethernet2 and start
- Next open Putty and select Telnet option under other give the ip address of Ubuntu and start
Now we successfully telnted to ubuntu in windows and enter the password and explore
And wireshark starts capturing the packets of all thesNow stop capturing the packets 
And apply telnet in filters
Now right click on any telnet packet and choose follow then tcpstream
Here we can see the data we entered in putty like passwords and etc.

