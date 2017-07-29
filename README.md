# Own_MongoDB_Config
# Initial Config Notes for - 

```
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ sudo apt-get install -y mongodb-org
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  mongodb-org-mongos mongodb-org-server mongodb-org-shell mongodb-org-tools
The following NEW packages will be installed:
  mongodb-org mongodb-org-mongos mongodb-org-server mongodb-org-shell mongodb-org-tools
0 upgraded, 5 newly installed, 0 to remove and 257 not upgraded.
Need to get 66.8 MB of archives.
After this operation, 270 MB of additional disk space will be used.
Get:1 http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4/multiverse amd64 mongodb-org-shell amd64 3.4.6 [7,981 kB]
Get:2 http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4/multiverse amd64 mongodb-org-server amd64 3.4.6 [14.2 MB]                            
Get:3 http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4/multiverse amd64 mongodb-org-mongos amd64 3.4.6 [8,110 kB]                           
Get:4 http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4/multiverse amd64 mongodb-org-tools amd64 3.4.6 [36.5 MB]                             
Get:5 http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4/multiverse amd64 mongodb-org amd64 3.4.6 [3,556 B]                                   
Fetched 66.8 MB in 2min 40s (417 kB/s)                                                                                                               
Selecting previously unselected package mongodb-org-shell.
(Reading database ... 576032 files and directories currently installed.)
Preparing to unpack .../mongodb-org-shell_3.4.6_amd64.deb ...
Unpacking mongodb-org-shell (3.4.6) ...
Selecting previously unselected package mongodb-org-server.
Preparing to unpack .../mongodb-org-server_3.4.6_amd64.deb ...
Unpacking mongodb-org-server (3.4.6) ...
Selecting previously unselected package mongodb-org-mongos.
Preparing to unpack .../mongodb-org-mongos_3.4.6_amd64.deb ...
Unpacking mongodb-org-mongos (3.4.6) ...
Selecting previously unselected package mongodb-org-tools.
Preparing to unpack .../mongodb-org-tools_3.4.6_amd64.deb ...
Unpacking mongodb-org-tools (3.4.6) ...
Selecting previously unselected package mongodb-org.
Preparing to unpack .../mongodb-org_3.4.6_amd64.deb ...
Unpacking mongodb-org (3.4.6) ...
Processing triggers for man-db (2.7.5-1) ...
Setting up mongodb-org-shell (3.4.6) ...
Setting up mongodb-org-server (3.4.6) ...
Adding system user `mongodb' (UID 126) ...
Adding new user `mongodb' (UID 126) with group `nogroup' ...
Not creating home directory `/home/mongodb'.
Adding group `mongodb' (GID 133) ...
Done.
Adding user `mongodb' to group `mongodb' ...
Adding user mongodb to group mongodb
Done.
Setting up mongodb-org-mongos (3.4.6) ...
Setting up mongodb-org-tools (3.4.6) ...
Setting up mongodb-org (3.4.6) ...
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ service mongod status
● mongod.service - High-performance, schema-free document-oriented database
   Loaded: loaded (/lib/systemd/system/mongod.service; disabled; vendor preset: enabled)
   Active: inactive (dead)
     Docs: https://docs.mongodb.org/manual
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ service mongod start
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ service mongod status
● mongod.service - High-performance, schema-free document-oriented database
   Loaded: loaded (/lib/systemd/system/mongod.service; disabled; vendor preset: enabled)
   Active: active (running) since Sat 2017-07-29 20:56:23 IST; 12s ago
     Docs: https://docs.mongodb.org/manual
 Main PID: 14323 (mongod)
   CGroup: /system.slice/mongod.service
           └─14323 /usr/bin/mongod --config /etc/mongod.conf

Jul 29 20:56:23 dhankar-VPCEB44EN systemd[1]: Started High-performance, schema-free document-oriented database.

dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ whereis mongod
mongod: /usr/bin/mongod /etc/mongod.conf /usr/share/man/man1/mongod.1.gz

dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ cd /var/lib/mongodb
dhankar@dhankar-VPCEB44EN:/var/lib/mongodb$ ls
collection-0--827616214542030742.wt  index-1--827616214542030742.wt  journal          sizeStorer.wt  WiredTigerLAS.wt   WiredTiger.wt
collection-2--827616214542030742.wt  index-3--827616214542030742.wt  _mdb_catalog.wt  storage.bson   WiredTiger.lock
diagnostic.data                      index-4--827616214542030742.wt  mongod.lock      WiredTiger     WiredTiger.turtle
dhankar@dhankar-VPCEB44EN:/var/lib/mongodb$ 
dhankar@dhankar-VPCEB44EN:/var/lib/mongodb$ 
```

#

#

#


#
