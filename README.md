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

Clone this repository and build the docker image using:

```shell
docker build -t anexia-it:drowncheck .
```

After building the image you may invoke DROWNcheck like this:

```shell
docker run --rm=true -t -i anexia-it:drowncheck 10.0.0.2 443
```