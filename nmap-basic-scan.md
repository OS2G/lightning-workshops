## Steps:
1. Install nmap (I like zenmap for visualizing results)
2. Starting NMAP
3. Running a basic scan
4. Reading scan results

## 1. Install Nmap/Zenmap
Nmap can be found at [nmap.org](https://nmap.org/download.html), most of the work for this tutorial is understanding how to choose the correct installer for your machine. 
Generally your best bet will be their docs (they have a section per OS). (Todo: include pictures walking through the installation)

## Starting NMAP/zenmap
(Todo: talk about adding the program to the system path so that they're both readily available)

## Basic NMAP Scanning
First, you will need to know your actual local IP address. The easiest route to figuring this out is using ipconfig/ifconfig in a terminal; there are several good ways to do this which can be found very easily.

Second, you need to know what network your IP address is on. This requires you to understand how subnetting works (explanation here). The simplest thing to try is scanning your own machine once you have this IP (this is basic vulnerability scanning.
Zenmap provides a number of prebaked scans you can execute against your IP address.

The easiest way to guess your network is to find your default gateway's IP address and subtract 1 from the last number, because the first address on a network is traditionally the default gateway (read: where internet traffic on that network comes from).
The subnet mask can be converted by converting each number of the subnet mask into binary (eg. 255.255.255.0 becomes 11111111.11111111.11111111.00000000) and counting the number of 1s before the 0s appear (alternatively, subtract how ever many 0s there are from 32).

An example Hello World scan would thus be something like
` nmap -sn -v 192.168.1.0/24`
Where -sn is the flag for an ARP scan (the simplest type of scan) and -v is for verbose (so you can actually see progress as it goes. There are many different types of scans which are fun to learn about.
The Topology tab of the main zenmap view lets you visually see all the hosts you just scanned.
(TODO: insert pictures)

## Reading scan results


### Notes

### Where to next?
