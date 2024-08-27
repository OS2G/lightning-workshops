## Steps
1. Download Wireshark
2. Install the Drivers
3. Start Capturing Data
4. Open the I/O Graph

## Download Wireshark
Download the installer from [wireshark.org](https://www.wireshark.org/) and start it up. (To be fixed: find some public image of the page that's not going anywhere to insert here)

## Install the Drivers
Normally, as part of the installation process wireshark will tell you to install the specific drivers necessary for your machine (To be fixed, the specific names/screenshots from installer)

## Start Capturing Data

Start up wireshark. You will either see a Wired or Wireless connection depending how your machine gets internet. The one with the wiggly line is probably the one providing your connection. 

Double click on your interface of interest and the little shark logo at the top should turn green. The screen will also change to give you the packet view (incredibly powerful, tons to make sense of).

## Open the I/O Graph
Under the Statistics menu at the top, the previously grayed out I/O Graph option should now be available if you're actively collecting data. Click it and the graph appears!

You can add and remove graphs using the plus/minus buttons in the bottom left. Your first two visible graphs may show you the number of packets; while it's surely helpful, most people want to know how much data their wireless card actually sends.

The correct graph that will show you what you'd see on speedtest.net is `all packets` using a line graph with the y-axis set to bits. Congrats, you're done!

![image](https://github.com/user-attachments/assets/3896833d-d750-4593-920f-da8a265c204d)

### Notes
Some machines are more finicky about the drivers than others, if you're nervous google should give you lots of good forum posts about your particular machine's setup.

If you want to leave this running the background passively measuring your internet speed (very informative over extended periods of time!), you will generally want to have the graph open and minimized. 
If you have collected a large volume of data (especially ongoing for say 10+ minutes) and then try to open the I/O graph, Wireshark can sometimes struggle.
