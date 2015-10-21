# WSO2 BPS 3.5.0 Dockerfile

WSO2 BPS 3.5.0 Dockerfile defines required resources for building a Docker image with WSO2 BPS 3.5.0.

## How to build

(1) Copy wso2bps-3.5.0 binary pack to the packages folder:

* [wso2bps-3.5.0.zip](http://wso2.com/products/business-process-server/)

(2) Generate template module `wso2bps-3.5.0-template-module-<PPAAS_VERSION>.zip` as described in [README.md](https://github.com/wso2/product-private-paas/tree/master/cartridges/template-module/wso2bps-3.5.0) under "Creating BPS Template Module for Private PaaS" section.


(3) Run build.sh file to build the docker image. (This will copy the plugins and template module to the docker image)
```
sh build.sh clean
```

(4) List docker images:
```
docker images
```
(5) If successfully built, docker image similar to following should display.
```
wso2/bps        3.5.0              ac57800e96c2        2 minutes ago         777.6 MB
```
## Docker environment variables
```
PPAAS_VERSION - WSO2 Private PaaS Version
PCA_HOME - Apache Stratos Python Cartridge Agent Home
JAVA_HOME - JAVA HOME
CONFIGURATOR_HOME - WSO2 Private PaaS Configurator Home
WSO2_SERVER_TYPE - WSO2 Carbon Server type
WSO2_SERVER_VERSION - WSO2 Carbon Server version
TEMPLATE_MODULE_NAME - PPaaS Carbon Server template module name
```
