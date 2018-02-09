Docker image for Provisionable Machine
======================================

This image is useful for testing provisioning scripts. It builds on top of [Alpine image][alpine-image] and adds OpenRC init system which allows managing services. In addition, _ssh_ and _sftp_ server accepts user with `root` username and `root` password.

To make a remote host known you can include any of the following keys in `~/.ssh/known_hosts`:

```shell
ssh-keyscan -p 2222 testing-machine | grep ssh-ed25519 >> ~/.ssh/known_hosts
```


[alpine-image]: https://hub.docker.com/_/alpine/
