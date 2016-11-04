# CSE1110-Headless-RPi-setup-assignment
Assignment for CSE1110 for setting up a headless Raspberry Pi (connected with Ethernet cable to Windows 10 laptop).

To complete this assignment you have to follow the described steps and check off all the steps you have completed succesfully (check them off using markdown, see https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments for how to do this). When you have completed the assignment show your running headless RPi to your teacher to have it marked. 

# Step 1: Set up RPi by connecting it to an existing screen
Before you are able to connect to your RPi from a Windows computer you need update the system and enable SSH and VNC on the RPi by connecting it to an external monitor, ethernet, keyboard and mouse. Start up your RPi and open a terminal. 

- [ ] Start by updating your RPi by running the following commands from the terminal:
```
sudo apt-get update
sudo apt-get upgrade
```
Check default values when prompted (just press enter).

- [ ] Enable SSH and VNC by running the following command in the terminal: ```sudo raspi-config```

When the menu appears  Select the advanced option -> VNC -> Enable VNC and Select the advanced option -> SSH -> Enable SSH 

- [ ] Exit ```raspi-config``` (using the tab key to move the cursor between menu items)
- [ ] Shutdown your RPi by running the following command in the terminal: ```sudo shutdown -h now```
- [ ] Unplug the Ethernet cable and power cable
- [ ] Reboot your RPi by plugging in the power cable
- [ ] Once you RPi has booted connect it to the EPS Internet Only Wifi network
- [ ] Shut down your RPi by running sudo shutdown -h now and unplug the power cable

# Step 2: Setup Windows computer for connecting to RPi
- Download and install the following software on a windows computer (laptop)
  - [ ] Bonjour Windows Print Services Using Apple: https://support.apple.com/kb/DL999?locale=en_GB
  - [ ] Bonjour Browser: http://hobbyistsoftware.com/bonjourbrowser
  - [ ] Install Putty: http://www.putty.org/
  - [ ] Install the VNC Viewer for Google Chrome App from the Chrome Web Store

# Step 3: Connecting remotely to the RPi from laptop (VNC mode)
Establishing a VNC connection between Windows and RPi by following these steps:
- [ ] Connect RPi with an Ethernet cable to the ethernet port of a Windows laptop
- [ ] Boot RPi by plugging it in (it will not not need a keyboard, mouse or monitor. Only the power cord and the Ethernet cable should be plugged into the RPi).
- [ ] Launch the BonjourBrowser on the Windows computer and click the refresh button until you see the RPi being detected
- [ ] Select the RPi VNC server and copy the IP number
- [ ] Open VNC Viewer for Google Chrome App through Chrome paste in the IP address when prompted
- [ ] Press connect… wait for the terminal window to appear.
- [ ] Log into your RPi.
