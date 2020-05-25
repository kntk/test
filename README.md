# Demo repository

Various samples for testing software with Vagrant.

# SSH Config

`192.168.0.0/23` is used for Management Segment in this repository.
Vagrantfile adds private_network for ssh login without `vagrant ssh`.
My `~/.ssh/config` sample is following:

```
Host 192.168.0.* 192.168.1.*
    User                    vagrant
    StrictHostKeyChecking   no
    UserKnownHostsFile      /dev/null
    IdentitiesOnly          yes
    IdentityFile            ~/.ssh/id_ecdsa_vagrant.key
```

