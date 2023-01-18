# HomeLab
HomeLab Setup running k3s with security monitoring features


### Basic Idea
- k3s nodes and master are Ubuntu VMs running under Proxmox
  - Looked at running in LXC container but has too many issues to implement
- Set up useful services for my home network 
  - Nextcloud
  - FreshRSS
  - Gitlab
  - Restic backup service
  - Ceph storage to NAS
  - Monica (Personal CRM) 
  - ... and more
- Set up additional security services 
  - Antrea CNI with Suricatta NID/PS or Security Onion
  - Falco container monitoring (basically container intrusion detection)
  - Authentik central Oath and SAML authentication
  - Grafana's Loki as a SIEM solution for all the logs 
  - ... and more  

### Why?
- Learning more about Kubernetes and containerization
  - Linux kernel mechanisms used for systems like docker/containerd
  - Still need to see stuff on RBAC and policies in k8s
- I get a playground for testing out open source software, security, and monitoring systems
  - See what projects people are creating
  - Find what gives me more visibility into the cluster network
  - Can learn how to set up and manage my own CA for k8s
- Improving my day to day function with some home services
  - Monica is a cool project that lets you manage information about the people you know
  - Home Wiki for managing information/documenting
  - Backups for my devices!!!
  - Get off using services that steal my information
- This is all doable with my one proxmox machine
  - I am poor college student who can't aquire the $20000 setups you see people have on r/homelab
  - Though, I this is far from redundant and I could lose everything in a blink of an eye
  
  
