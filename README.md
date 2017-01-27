# AutoVirtualbox

## Installation
This script can be run on its own, but it can also work within init.d for autostarting VMs

* Add this script to `/etc/init.d/`, run `update-rc.d vmmanager defaults 99 01` as `root`.
* Change `$VBOXUSER` in the script to the appropriate user that you are using to run VMs with.
* Create a file in `$VBOXUSER`'s home folder named `.autostartvms`, add just the UUIDs (UUIDs look along the lines of this: a02b5b54-a84d-48fa-8dac-2a3fad55717e) of the VMs that you wish to autostart
    
## Usage
### /etc/init.d/vmmanager stop
For stopping every VM from running by default, can specify VM's name(s).  

### /etc/init.d/vmmanager start
Starts all of the specified VMs from /home/$VBOXUSER/.autovms by default, can specify VM's name(s)

### /etc/init.d/vmmanager status
Lists running VMs

### /etc/init.d/vmmanager list
Lists all VMs
