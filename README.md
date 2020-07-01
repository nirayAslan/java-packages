# Monostore

![Build Status](https://miro.medium.com/max/708/0*Q7OCXDNejTFVCPxB.jpg)

Monostore is a package of frequently used integrations and contains B2B and B2C Accelerator.

  - Based on SAP Commerce 2005

### Installation

>Monostore requires;
-SAP Commerce 2005,
-Java Development Kit 11
-Git
-Intellij Idea

* Clone Repository
```sh
$ git clone https://github.com/monotect/monostore.git
```
* Merge with SAP Commerce 2005
* Run ant clean all 
```sh
$ ant clean all
```
* Make sure that the config folder is created.
* Update /etc/hosts file with following lines:
       *"127.0.0.1 monostore.local"*
```sh
$ sudo nano /etc/hosts
```
* Move the contents of config-local/local.properties and localextensions.xml to config/
```sh
$ cd ../../config-local
$ cp localextensions.xml ../config/ && cp local.properties ../config/
```
* Ant initialize
```sh
$ ant initialize
$ ./hybrisserver.sh
```
* In order to access accelerator storefronts:
https://localhost:9002/monostorefront/?site=powertools
https://monostore.local:9002/monostorefront/?site=powertools
