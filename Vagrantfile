# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "scotch/box"
    config.vm.network "private_network", ip: "172.16.13.13"
    config.vm.hostname = "scotchbox"
    config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]
    
    
    # Optional NFS. Make sure to remove other synced_folder line too
    #config.vm.synced_folder ".", "/var/www", :nfs => { :mount_options => ["dmode=777","fmode=666"] }
	
    config.ssh.username = "vagrant"
	config.ssh.password = "vagrant"

    #Fix for 'stdin: is not a tty'
    config.ssh.shell = "bash -c 'BASH_ENV=/etc/profile exec bash'"

    config.vm.provision "shell", inline: <<-SHELL
        # Shell commands here...
        #cd ./
        #grunt sass
        #echo 'grunt sass complete...'

    SHELL

end