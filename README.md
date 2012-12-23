# Vagrant WordPress #

Virtual machine for development with WordPress.

Installed by default:

* Apache2
* MySQL
* PHP
* phpMyAdmin
* Git
* Subversion
* Vim
* WordPress

## Requirements ##

* [VirtualBox](https://www.virtualbox.org/)
* [Ruby](http://www.ruby-lang.org)
* [Vagrant](http://vagrantup.com/)
* [Git](http://git-scm.com/)

## Install: ##

Clone this repo and execute:

    $ git submodule init
    $ git submodule update
    $ vagrant up

## Custom Instalation: ##

See the configurations that are possible via the Vagrantfile.

### WordPress config: ###

    "wordpress" => {
      "dir" => "/home/vagrant/www",
      "url" => "http://br.wordpress.org/wordpress-3.5-pt_BR.tar.gz",
      "lang" => "pt_BR",
      "debug" => "false",
      "db" => {
        "database" => "wordpressdb",
        "user" => "wordpressuser",
        "prefix" => "wp_"
      }

* **dir** - Not change, it is essential to work with the shared folder!
* **url** - WordPress tag.gz url
* **lang** - WordPress installation language.
* **debug** - WordPress debugging mode.
* **db** - WordPress MySQL database config.

### MySQL config: ###

    "mysql" => {
      "server_root_password" => "vagrant",
      "server_repl_password" => "vagrant",
      "server_debian_password" => "vagrant"
    },

All fields are for setting passwords to the MySQL users.

### Access via IP or fake domain ###

To access via IP uncomment the line below:

    # config.vm.network :hostonly, "192.168.33.10"

You can also configure your hosts file:

    192.168.33.10    www.project-name.com

## Sources: ##

### Box ###

Ubuntu Precise 32 Box by [Vagrantbox.es](http://www.vagrantbox.es/)

### Cookbooks ###

Cookbooks by [Opscode Public Cookbooks](https://github.com/opscode-cookbooks/)

    cookbooks/
        apache2/
        apt/
        build-essential/
        git/
        mysql/
        openssl/
        php/
        phpmyadmin/
        subversion/
        vim/
        wordpress/

WordPress custom cookbook: <https://github.com/claudiosmweb/wordpress-cookbook/>

## License: ##

Licensed under the [MIT license](http://opensource.org/licenses/mit-license.php).
