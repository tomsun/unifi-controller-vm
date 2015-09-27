unifi-controller-vm
===================

A Vagrantfile for running [Unifi Controller](https://www.ubnt.com/download/unifi/)
in a VM, so that you don't have to install a JRE and MongoDB on your main OS.

The VM uses a bridged network adapter, to simplify access to other devices on the network.
(Assumes the targeted network is VirtualBox's default interface and assumes DHCP - for
finer-grained control, see the [Vagrant documentation](http://docs.vagrantup.com/v2/networking/public_network.html))

### Usage

- Install [Vagrant](https://www.vagrantup.com/downloads.html) and
  [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

- Run `vagrant up` in the `unifi-controller-vm` directory

- Open https://`vm-ip`:8443 in a web browser

```bash
$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Importing base box 'ubuntu-14.04'...
.
.
.
==> default: Unifi Controller v4.7.5 is now listening at
==> default: https://10.0.2.15:8443
==> default: https://192.168.0.21:8443
```
