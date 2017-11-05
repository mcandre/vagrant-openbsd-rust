# vagrant-openbsd-rust: a Vagrant box for building Rust binaries for OpenBSD

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-openbsd-rust

# EXAMPLE

```console
$ vagrant up
$ vagrant ssh -c "cd /vagrant && rustc hello.rs && ./hello"
Hello World!
```

# REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* A VM provider, such as [VirtualBox](https://www.virtualbox.org), [VMware](https://www.vmware.com), or [libvirt](https://libvirt.org)

# EXPORT

```console
$ vagrant package --output vagrant-openbsd-rust.box
```
