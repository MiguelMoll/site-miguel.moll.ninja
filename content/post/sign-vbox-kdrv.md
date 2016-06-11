+++
date = "2016-06-06T22:23:23-04:00"
description = ""
tags = []
title = "Signing VirtualBox Kernel Drivers"
topics = []

+++

I recently came across an issue with VirtualBox and Fedora 23 that took me a good while to address. With Secure Boot enabled, the built kernel modules failed to load. Instead of disabling secure boot, I decided to tackle the problem head on. Hopefully this will be use for some, most likely my future self.

I tried installing VirtualBox via both the repos and  [website](https://www.virtualbox.org/wiki/Downloads) with no luck. And after various logs referring to `dmesg` with nothing of value, off to the interwebs I went. As this the first time I didn't disable secure boot (honestly I forgot) I didn't know as of Fedora 22 drivers need to be signed. Good to know.

Credit where credit is due: http://gorka.eguileor.com/vbox-vmware-in-secureboot-linux/

That useful blogpost really saved me. I could copy/paste the entire thing here, but sharing the link works better. It includes some extra tidbits for VMware.
