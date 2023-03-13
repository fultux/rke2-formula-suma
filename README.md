# rke2-formula-suma
Formula to install rke2 server with SUSE Manager.
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


After that point you shoud be able to see the formula available on your SUSE Manager under the Kubernetes section in formulas. 
![image](https://user-images.githubusercontent.com/68954556/224348201-f9c00554-d753-4190-b071-d361fc24751e.png)

After being enabled you can fill the formular to fit your preferences. 
![image](https://user-images.githubusercontent.com/68954556/224348457-6298a40d-2135-4d2e-8e16-850a139187d0.png)

Now after applying the highstates it will install rke2-server on your client. 



## Future improvments to add
- Add more configurations options: At the moment you can only configure the CNI, version, tls-san. 
- Be able to manage an air-gapped installation and private registries.
 



