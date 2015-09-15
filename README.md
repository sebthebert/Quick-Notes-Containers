# Quick-Notes-Containers

## What is a container ?

It's chroot on steroids.

It's not quite like a VM: 
  * uses the host kernel 
  * can't boot a different OS 
  * can't have its own modules 
  * doesn't need init as PID 1 
  * doesn't need syslogd, cron... 

It's just a bunch of processes visible on the host machine (contrast with VMs which are opaque)


Cgroups = limits how much you can use

Namespaces = limits what you can see (and therefore use)

Sources: 

[Anatomy of a Container: Namespaces, cgroups & Some Filesystem Magic](http://www.slideshare.net/jpetazzo/anatomy-of-a-container-namespaces-cgroups-some-filesystem-magic-linuxcon)

[Deep dive into docker storage drivers](https://github.com/jpetazzo/jpetazzo.github.io/blob/master/assets/2015-07-01-deep-dive-into-docker-storage-drivers.html)

[Containers, Docker, and Security: State Of The Union](http://www.slideshare.net/jpetazzo/containers-docker-and-security-state-of-the-union-linuxcon-and-containercon-2015)


TO READ:
http://www.slideshare.net/jpetazzo/docker-linux-containers-lxc-and-security
