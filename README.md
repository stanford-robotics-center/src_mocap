# SRC Motion Capture System
OptiTrack Documentation: [link](https://docs.optitrack.com/)

Motion Capture Licenses: As of 3/4/2025, we have 2 Unlimited and 4 Tracker licenses (Features for each license: [link](https://optitrack.com/software/motive/pricing.html)). The Unlimited licenses are in the Dance Studio and Field & Construction. Please ask SRC staff about upgrading licenses if needed.

Login/Auth for SRC MoCap Computers: Please ask SRC staff for login / authorization.

Each MoCap Room has a KVM that allows a user to control the MoCap computer remotely via web interface if connected to the local network (Ex: SRC, eduroam, Stanford, Stanford Visitor). To connect, enter the public domain name (i.e. ```SRC-KVM-Dance.stanford.edu```) into a web browser. Accept the security risk by clicking ```Advanced```, and ```Accept the Risk and Continue```.
![pic](/images/security.png "Security")
![pic](/images/tiny_pilot.png "Tiny Pilot")

Open the ```Motive``` application to access the MoCap system.
![pic](/images/motive_1.png "Motive 1")

## OceanWalk
License: Motive Tracker\
Public Domain: SRC-KVM-HRI.stanford.edu

## Dance Studio
License: Motive Unlimited\
Public Domain: SRC-KVM-Dance.stanford.edu

For dance studio, it would be best to send a Wifi MAC address for your laptop/device that would like to stream Optitrack data to Zen. We can then request the network manager in EE to assign static IP addresses for your devices to be on ```SRC``` network. The Optitrack IP address you would like to stream over would be ```172.24.68.67``` if the ethernet cable is connected correctly to the switch. The correct settings for this configuration should have the Optitrack computer with wifi turned off and ```Ethernet 2``` (i.e. the network adapter) set to DHCP.

Once your device is assigned a static IP, one should be able to stream data from the Optitrack computer at ```172.24.68.67``` when connected to the ```SRC``` network.

## Domestic Suite
License: Motive Tracker\
Public Domain: SRC-KVM-Domestic.stanford.edu

## Kitchen
License: Motive Tracker\
Public Domain: SRC-KVM-Kitchen.stanford.edu

## Field & Construction
License: Motive Unlimited\
Public Domain: SRC-KVM-Fieldbay.stanford.edu

## Logistics & Manufacturing
License: Motive Tracker\
Public Domain: SRC-KVM-Warehouse.stanford.edu
