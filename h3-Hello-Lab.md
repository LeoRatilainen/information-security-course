# x)
The first link is guide on installing debian version of linux on a virtualbox and common issues with the process solved. Also shows you a few helpful steps like how to get sudo apt-get updates installed.

The second link is terminal commands which the most useful ones for normal use will be the the moving and looking around section and file manipulation.
# a)
When pinging a web address without internet line "icmp_seq=1 Destination Net Unreachable" the output lines mean.

-"icmp_seq=1" is the number of the ICMP packet which in thi case is stuck at one since without a network it can't proceed.

-"Destionation net Unreachable" means jsut simply that the network that's being pinged can't be found.

When pinging the same web server with connection the line "64 bytes from 1.1.1.1: icmp_seq=1 ttl=225 time=37.6 ms" in this the output lines mean.

-"64 bytes from 1.1.1.1" the size of the ICMP pack and where it came from.

-"icmp_seq=1" this is the sequence number of the ping request my example shows 1 but this will keep going up the each request sent.

-"ttl=225" Time to live. Each router hop it took the get here this is also variable.

-"time=37.6 ms" this is how long it took between your machine and the destionation or other word latency.

# b)
port scanning is used to check ports which are virtual endpoints for communication a port scanner sends packages to a range of ports and based on the responses it it shows open ports, closed ports and filtered ports.

-Open ports means a service is actively listening.

-closed port means no service is listening but it replied nothing here.

-flitered port means a firewall blocked the probe and no message was received.

When i portscan my localhost it shows you alot of information most of what i do not understand what it means, but to me the device
type section looks very interesting it shows operating system information including kernel level info.
# c)
If portscanned again with apache installed the section that changes is in PORT STATE SERVICE VERSION 
it opens port 80/tcp where it runs that port and it's added to the scan.
# d)

level 0

This level is solved with the line ssh bandit0@bandit.labs.overthewire.org -p 2220 what these mean is ssh is secure shell bandit0 is the username we are logging in with bandit.labs.overthewire.org is the address and -p 2220 is port 2220 being used. Then a password is asked which is bandit0. you can the search the directories with ls which shows a readme file that can be accessed with cat readme that'll give you the password for the next level.

level 1

You then use the password from the previous level to access the next level where with ls you'll find a directory called - you can read this with cat ./- which will give you the password to the next game.

level 2

With this level you do everything from before but you access the directory with cat spaces\ in\ this\ filename which tells it that there's spaces in the filename this will give you the next password.

level 3

in this level you need to find the password in a hidden directory this can be found with cd inhere and the then ls you can find a file called .hidden which can be accessed with cat .hidden.

# sources 
https://terokarvinen.com/2021/install-debian-on-virtualbox/

https://terokarvinen.com/2020/command-line-basics-revisited/
