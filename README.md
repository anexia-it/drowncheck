# drowncheck
DROWN SSL attack checker


Important
---------
This script should be executed in an environment where SSLv2 is enabled.

Usage
-----

```shell
./DROWNcheck.sh 10.0.0.2 443
./DROWNcheck.sh 10.0.0.2 993
```

Simple usage using custom docker container
------------------------------------------

Either build this image yourself using the Dockerfile in this repository,
or use the image available from Docker hub:

```shell
docker pull anexia/drowncheck:latest
```

```shell
docker run --rm=true -t -i anexia/drowncheck:latest 10.0.0.2 443
docker run --rm=true -t -i anexia/drowncheck:latest 10.0.0.2 993
```