# Ubiq-Mining-Rig
/*-------- THIS IS A WORK IN PROGRESS PLEASE USE AT YOUR OWN RISK ---------------*/

Informational Guide on how to get a Ubiq/ Eth Mining rig up and runing on Linux's Distro Ubuntu. I will include fan settings as well overclocking settings.

So to properly start using this press ctrl+Alt+T this will open a terminal window
Inside that window you want to type 

sudo apt-get install git

this will install github onto your linux machine.

The next thing you want to do is to clone this repository onto your machine.

Select the location for this repo from github where it says "Clone or Download"

you will type in the terminal:      git clone https://github.com/ventureproz/Ubiq-Mining-Rig.git

This will create the files on your hard drive.

Commands you should know when working with linux Terminal:

ls al         (Lists all items in folder)
cd            (Change Directory allows you to move from one folder to another) Example: cd Desktop/NewFolder   
sudo          (Gives your permissions to install a file with your password) Example: sudo apt-get install git

To run a basic file goto actual file location and right-click and select Open Terminal this will save you the time having to use ls al and change directory terminal commands

type ls al to see that the newly opened terminal now shows all the files you where looking for.
if this is the case the first file I would run is the install_dependencies.sh file.
to do this type:

./install_dependencies.sh

if this does not run properly cause you need root permissions type the following

sudo ./install_dependencies.sh

the next thing we want to do is to open the FanControl-UnderClock.sh file.

This controls our fans and power of our GPU's  (I've used this with both GTX 1070's and GTX 1080's please refer to your gpu's best settings before you begin with this step.)

if you right click the file and open it with gedit you will need to edit the following information:

To add more GPU's just label from 0 - 6+  notice in the line of code [gpu:1]/GPUFanControlState=1 where it says  [gpu:1]  the 1 is marking the second GPU in your system. If add another gpu it will look like this: 
sudo nvidia-settings -a [gpu:2]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90
sudo nvidia-settings -a [gpu:3]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90
sudo nvidia-settings -a [gpu4]/GPUFanControlState=1 -a [fan:1]/GPUTargetFanSpeed=90

If you need to change the fan speed 

-a [fan:1]/GPUTargetFanSpeed=70  Notice I changed 90 to 70 this will make the fan slower please make sure to moniter the heat of your GPU when doing this. I prefer to keep my GPU's around 40-48 degrees Celsius. Please refer to your GPU's best temperature settings and set fan speeds accordingly

















