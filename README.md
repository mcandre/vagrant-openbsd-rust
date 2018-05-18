# vagrant-openbsd-rust: a Vagrant box for building Rust binaries for OpenBSD

# WARNING

Rustup does not yet offer a port for OpenBSD, so Rust nightly is difficult to setup on these hosts.

# VAGRANT CLOUD

* https://app.vagrantup.com/mcandre/boxes/vagrant-openbsd-rust-amd64
* https://app.vagrantup.com/mcandre/boxes/vagrant-openbsd-rust-i386

# EXAMPLE

```console
$ cd amd64/test
$ vagrant up
$ vagrant ssh -c "cd /vagrant && rustc hello.rs && ./hello"
Hello World!
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ sh -c "cd amd64 && make vagrant-openbsd-rust-amd64.box"
$ sh -c "cd i386 && make vagrant-openbsd-rust-i386.box"
```
