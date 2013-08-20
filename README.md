# Drawing Biennial

## Dev

We use Vagrant as a lightweight manager for virtual environments. Download and install the latest version from [http://downloads.vagrantup.com/tags/v1.2.7](http://downloads.vagrantup.com/tags/v1.2.7).

Next, run the bootstrap sequence:

```bash
$ git submodule init
$ git submodule update
$ vagrant up
```

This might take some time since it needs to fetch the VM binaries and provision the machine.
