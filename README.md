### Mtprotoproxy ansible role

Will clone [mtprotoproxy](https://github.com/alexbers/mtprotoproxy) from git (stable branch by default), generate config from vars and install systemd service file  
Also installs dependencies based on system (uvloop is available in ubuntu but not in debian)  
Tested on Debian 9 and Ubuntu 18.04 LTS. Should work with any system if you adjust vars for operating system.

Vars example (host/group vars):
```
mtprotoproxy_branch: master
mtprotoproxy_port: 31812
mtprotoproxy_ad_tag: 00000000000000000000000000000000
mtprotoproxy_secrets:
  - [user1, 00000000000000000000000000000001]
  - [user2, 00000000000000000000000000000002]
```

