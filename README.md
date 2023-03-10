# rke2-formula-suma
Formula to install a rke2 cluster with SUSE Manager.
This will install rke2-server on the targeted server. It can be installed either in standalone mode or registered to another server in the case of a Highly available installation. 

## Prerequisites
- SUSE Manager 4.3 and later
- Opensuse Leap 15.3/SUSE Linux Enterprise Linux 15 SP3 or later.

## How to
On the suse manager create the 2 following folders:

```
mkdir /srv/salt/rke2-server
mkdir /srv/formula_metadata/rke2-server
```

Either clone this repo or extract it as a zip file. 
Copy the content of the folder states in the folder  /srv/salt/rke2-server.
Copy the content of the folder formula_metadata in the folder /srv/formula_metadata/rke2-server.



