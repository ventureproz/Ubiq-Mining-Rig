# Ubiq-Mining-Rig
Informational Guide on how to get a Ubiq/ Eth Mining rig up and runing on Linux's Distro Ubuntu. I will include fan settings as well overclocking settings.

So to properly start using this press ctrl+Alt+T this will open a terminal window
Inside that window you want to type 

sudo apt-get install git

this will install github onto your linux machine.








To add more GPU's just label from 0 - 6+  notice in the line of code [gpu:1]/GPUFanControlState=1 where it says  [gpu:1]  the 1 is marking the second GPU in your system. If add another gpu it will look like this: 
sudo nvidia-settings -a [gpu:2]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90
sudo nvidia-settings -a [gpu:3]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90
sudo nvidia-settings -a [gpu4]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90




















