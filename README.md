# aimat-lab.github.io/package-index
Public package index for the AIMat Lab.  
To install packages you need to have an ssh key for github setup on your system. Due to 2FA it is not possible anymore to serve packages via https.  
You can install packages from here using:
```
pip install <package_name> --extra-index-url https://aimat-lab.github.io/package-index/
```


## Config File
It is also possible to create a pip config file which allows to automatically search packages from the AIMat Lab without 
adding the tag `extra-index-url` for every install.

You just have to create a file called `pip.conf` in the directory `/home/user/.config/pip` and copy the following
config:

```
[global]
  extra-index-url = https://aimat-lab.github.io/package-index/ 
[install]
  trusted-host = https://aimat-lab.github.io/package-index/
```

