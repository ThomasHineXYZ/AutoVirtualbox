# AutoVirtualbox

## Installation
* Add this script to `/etc/init.d/`, run `update-rc.d vmmanager defaults 99 01` as `root`.
* Change `$VBOXUSER` to the appropriate user that you are using to run VMs with.
* Create a file in `$VBOXUSER`'s home folder named `.autovms`, add just the UUIDs of the VMs that you wish to autostart
    
## Usage
### /etc/init.d/vmmanager stop
For stopping every VM from running by default, can specify VM's name(s).

### /etc/init.d/vmmanager start
Starts all of the specified VMs from /home/$VBOXUSER/.autovms by default, can specify VM's name(s)

### /etc/init.d/vmmanager status
Lists running VMs

### /etc/init.d/vmmanager list
Lists all VMs
