# docker_fetch_from_registry
A python script which help you to pull docker images from a private registry using Docker Registry API.

This project is a fork from https://github.com/NotSoSecure/docker_fetch/ with adding authentication param.


## Examples:

```
$ python docker_fetch_from_registry.py -u http://docker.registry.ip -a "Basic YWRtaW46YWRtaW4="
```

In this example the creds for the docker registry is (admin:admin), so the "YWRtaW46YWRtaW4=" represent the base64 encoded string "admin:admin"

```
$ echo "YWRtaW46YWRtaW4=" | base64 -d                                                                       
admin:admin
``` 


