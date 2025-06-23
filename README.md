# SRC Motion Capture System
OptiTrack Documentation: [link](https://docs.optitrack.com/)

Motion Capture Licenses: As of 3/4/2025, we have 2 Unlimited and 4 Tracker licenses (Features for each license: [link](https://optitrack.com/software/motive/pricing.html)). The Unlimited licenses are in the Dance Studio and Field & Construction. Please ask SRC staff about upgrading licenses if needed.

Login/Auth for SRC MoCap Computers: Please ask SRC staff (Zen / Matt) for login / authorization.

Each MoCap Room has a KVM that allows a user to control the MoCap computer remotely via web interface if connected to the local network (Ex: SRC, eduroam, Stanford, Stanford Visitor). To connect, enter the public domain name (i.e. ```SRC-KVM-Dance.stanford.edu```) into a web browser. Accept the security risk by clicking ```Advanced```, and ```Accept the Risk and Continue```.
![pic](/images/security.png "Security")
![pic](/images/tiny_pilot.png "Tiny Pilot")

Open the ```Motive``` application to access the MoCap system.
![pic](/images/motive_1.png "Motive 1")

## Steaming data
Ideally, it is best to stream data over the ```SRC``` network instead of directly connecting via ethernet to Optitrack computers to avoid others from losing the ability to stream data. It would be best to send a Wifi MAC address for your laptop/device that would like to stream Optitrack data to Zen. We can then request the network manager in EE to assign static IP addresses for your devices to be on ```SRC``` network. 

Note that the above only works if the device is registered with Stanford.

### Obtaining Wifi MAC address
Definition of MAC address:
```
A MAC address is a unique 12-digit hexadecimal number that identifies a network interface controller (NIC) for communication on a computer network.
It's typically represented in the format XX:XX:XX:XX:XX:XX or XX-XX-XX-XX-XX-XX, where XX represents a two-digit hexadecimal number.
For example, a MAC address might look like 00:1A:2B:3C:4D:5E or 00-1A-2B-3C-4D-5E
```
To obtain your wifi MAC address, one can go into Network settings and go into Details to find their wifi MAC address. For example, for Apple devices, click ```Settings```, click ```Details``` and there should be an associated MAC address. Please make sure to turn off ```Rotating``` on Private Wifi address since assigning a static IP requires a static MAC address.

One can also find their wifi MAC address by running ```ifconfig``` in a terminal and knowing which network interface matches wifi.

### Setting up a Sample Client
To stream data to a sample client, download the NatNet 4.3 SDK from Optitrack: [Link to Ubuntu / Fedora / Windows](https://optitrack.com/support/downloads/developer-tools.html)

For Ubuntu Linux, once installed, set the environment variable ```LD_LIBRARY_PATH``` by running ```export LD_LIBRARY_PATH=~/Downloads/NatNet_SDK_4.3_ubuntu/lib/```, while making sure that is the correct file path to the ```NatNet_SDK_4.3_ubuntu/lib/``` directory. Then navigate to the ```NatNet_SDK_4.3_ubuntu/samples/SampleClient/build``` directory and run the Sample Client: ```./SampleClient```. If the computer is connected to SRC wifi, there should be available IP addreses to stream from:
![pic](/images/sampleclientstream1.png "SampleClient Stream")

One can select the correct stream by pressing the corresponding key/number in brackets next to the corresponding IP address to stream from.

## OceanWalk
License: Motive Tracker\
Public Domain: SRC-KVM-HRI.stanford.edu

## Dance Studio
License: Motive Unlimited\
Public Domain: SRC-KVM-Dance.stanford.edu

For dance studio, the Optitrack IP address you would like to stream over would be ```172.24.68.67``` if the ethernet cable is connected correctly to the switch. The correct settings for this configuration should have the Optitrack computer with wifi turned off and ```Ethernet 2``` (i.e. the network adapter) set to DHCP.

Once your device is assigned a static IP, one should be able to stream data from the Optitrack computer at ```172.24.68.67``` when connected to the ```SRC``` network.

## Domestic Suite
License: Motive Tracker\
Public Domain: SRC-KVM-Domestic.stanford.edu

## Kitchen
License: Motive Tracker\
Public Domain: SRC-KVM-Kitchen.stanford.edu

For the kitchen, the Optitrack IP address you would like to stream over would be ```172.24.69.102``` if the ethernet cable is connected correctly to the switch. The correct settings for this configuration should have the Optitrack computer with wifi turned off and ```Ethernet 2``` (i.e. the network adapter) set to DHCP.

Once your device is assigned a static IP, one should be able to stream data from the Optitrack computer at ```172.24.69.102``` when connected to the ```SRC``` network.


## Field & Construction
License: Motive Unlimited\
Public Domain: SRC-KVM-Fieldbay.stanford.edu

For the field bay, the Optitrack IP address you would like to stream over would be ```172.24.68.77``` if the ethernet cable is connected correctly to the switch.

## Logistics & Manufacturing
License: Motive Tracker\
Public Domain: SRC-KVM-Warehouse.stanford.edu
