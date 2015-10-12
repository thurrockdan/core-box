# Core Box

## Installation

* Install the vagrant scotch-box (`https://github.com/scotch-io/scotch-box`)
* `git clone git@github.com:thurrockdan/core-box.git`
* Set your desired IP in Vagrantfile (172.16.13.13)
* Replace all instances of `core-box` to your desired repo name
* `vagrant up`
* `vagrant provision`
* `cd public`
* `bower_install`
* `cd ../`
* `bash build.sh`
* `composer install`
* Visit http://172.16.13.13 
