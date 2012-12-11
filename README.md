# Vagrant WordPress #

Virtual machine for development with WordPress.

Installed by default:

* Apache2
* MySQL
* PHP
* Git
* Subversion
* Vim
* WordPress

## Install: ##

Clone this repo and execute:

    $ git submodule init
    $ git submodule update
    $ vagrant up

## Requirements ##

* [VirtualBox](https://www.virtualbox.org/)
* [Ruby](http://www.ruby-lang.org)
* [Vagrant](http://vagrantup.com/)
* [Git](http://git-scm.com/)

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
        subversion/
        vim/
        wordpress/

## License: ##

Licensed under the MIT license. [License text](http://opensource.org/licenses/mit-license.php).
