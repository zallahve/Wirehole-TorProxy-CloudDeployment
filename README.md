# PiVPN-PiHole-Unbound-TorProxy 

## Abstract:



## Initial Set-up

1. Download the latest (lite) version of Rasbian from here - https://www.raspberrypi.org/downloads/raspbian/
2. Flash this to your SD card using a tool like Etcher (https://www.balena.io/etcher/)
3. Insert the flashed SD card into the Raspberry Pi - and for this intial bit of setup you’ll also need it connected to a monitor and keyboard as well.
4.Boot the device and login with the default credentials (Username: pi) (Password: raspberry). It’s best practice to now set a custom password. Run the      passwd command to set your own password.
5. Next we need to enabled SSH access so we can work on the Pi remotely. Run the command sudo raspi-config to open the configurator tool.
Selection option (5) ‘INTERFACE OPTIONS’ and select ‘P2 SSH’ from the list to enable SSH access to the Raspberry Pi.
6. Enter the command ifconfig to reveal network information - an ‘inet’ value will be shown your connected network adapters - make note of the relevant number - you’ll need this to connect remotely to the Raspberry Pi.
Ideally, you’ll want to set this as a reserved (fixed) IP for this machine via your router configuration page.
7. Download a tool like Putty (https://putty.org/) and connect to the Raspberry Pi from your desktop / laptop PC using the IP address from the step above - the username ‘pi’ and the password you specified in step 4.
8. Once you’ve logged into your Raspberry Pi, it’s best practice to ensure all packages are up to date. Run sudo apt-get update && sudo apt-get upgrade -y to check for new packages and install any updates.


## Installing Pi-Hole



## Setting-up Unbound



## Installing Wireguard VPN




## Creating Tor Proxy




## Auto Deployment in the Cloud
