opencv-env
======
Configuration Environment for opencv  at https://github.com/opencv/opencv


## Requirements
* cmake 

## Rules

One can install lmfit with the following orders:

```
lmfit-env$ make init
lmfit-env$ make build
lmfit-env$ make install
```


For CentOS, one should run the following also

```
lmfit-env$ make setup
```

All files are installed in /usr/local/


## Steps

### Check the Release Tag

* Edit configure/CONFIG_MODULE
```
MODULE_TAG:=tags/3.4.2
```


### make init
* Download the main opencv from  https://github.com/opencv/opencv
* Switch to Release number selected in CONFIG_MODULE


### make build

* Prepare cmake environment
* Build 

### make install
* Install all files into /usr/local (default)

### make distclean
* Delete downloaded source file (opencv directory under opencv-env)

### make setup
* Create ld.conf for opencv target directory (/usr/local/lib)