# Supported tags and respective `Dockerfile` links

-	[`0.1.7-beta`, `latest` (*0.1/Dockerfile*)](https://github.com/nexocrew/docker_3nigm4_ishtmserver/0.1/Dockerfile)

# What is 3nigm4 "If Something Happens To Me" service?
The Ishtm service will let any user upload sensible data references (encrypted using PGP using the recipient’s keys and referring to files using the previously described storage service) and to deliver it, to pre-defined recipients, if the legitimate data owner do not ping the system after a specific amount of time.

# How to use this image

## start a authserver instance

The following example links to a mongodb container from the official [MongoDb image](https://hub.docker.com/_/mongo/).

```console
$ docker run -d --name ishtm-service -p 443:443 --link mongodb:mongodb nexo/3n4ishtm
```
