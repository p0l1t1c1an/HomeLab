
# Setup

(No detailed notes here as it is fairly basic)

### Hardware
- Dell Poweredge R710 w/ 32 GB ram
- 5 2TB drives

### Operating Systems
- Proxmox running as the hypervisor
    - Installed on zfs mirror setup with 2 disks
- Ubuntu images for virtual machines


### Creating Virtual machines
- Through Proxmox, create a base ubuntu VM 
    - Follow prompts on the terminal display in browser
    - Make sure to enable and install ssh server
    - Create sudo user w/ simple password 
        - Can't copy pw from password store soltion to this
- Clone vm 3 times creating 1 kubernetes master and 2 nodes 
    - Ssh into vm and change passwords 
    - Store passwords into password store
- In proxmox, create lvm storage for each additional disk
    - 1 will be for each k8s node/master
    - Name them accordingly and add them to the VM with the full storage


This prepares the vm nodes to be setup for installing k3s and then ceph/rook.

Other pages will be more detailed showing exact commands with secrets removed.

