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

You will now have a working Wordpress installation running on a virtual machine. Access it through [http://localhost:8080/wordpress](http://localhost:8080). The admin interface is on [http://localhost:8080/wordpress/wp-admin](http://localhost:8080/wordpress/wp-admin) and has initial credentials user: `admin` and password: `vagrant`.
