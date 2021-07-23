# Build your kernel driver

In order to build any driver yourself, go on your docker host and use follwing shell commands to build it:

```
mkdir thunderbolt

cd thunderbolt

git clone https://github.com/xcp-ng/xcp-ng-build-env

git clone https://github.com/xcp-ng-rpms/thunderbolt-module

chown 1000 ./thunderbolt-module/ -R

./xcp-ng-build-env/run.py -b 8.2 --build-local thunderbolt-module/ --rm
```
