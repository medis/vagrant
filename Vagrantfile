# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
		
	config.vm.define :var do |var_config|
		var_config.vm.network "forwarded_port", guest: 80, host: 80
		var_config.vm.box = "ubuntu/xenial64"
		var_config.vm.network "public_network"
		var_config.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
	
	config.vm.define :sol do |sol_config|
		sol_config.vm.network "forwarded_port", guest: 8983, host: 8983
		sol_config.vm.box = "ubuntu/xenial64"
		sol_config.vm.network "public_network"
		sol_config.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
	
	config.vm.define :db1 do |db1|
		db1.vm.network "forwarded_port", guest: 3306, host: 3306
		db1.vm.box = "ubuntu/xenial64"
		db1.vm.network "public_network"
		db1.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
	
	config.vm.define :db2 do |db2|
		db2.vm.network "forwarded_port", guest: 3306, host: 3307
		db2.vm.box = "ubuntu/xenial64"
		db2.vm.network "public_network"
		db2.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
	
	config.vm.define :web1 do |web1|
		web1.vm.network "forwarded_port", guest: 80, host: 81
		web1.vm.box = "ubuntu/xenial64"
		web1.vm.network "public_network"
		web1.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
	
	config.vm.define :web2 do |web2|
		web2.vm.network "forwarded_port", guest: 80, host: 82
		web2.vm.box = "ubuntu/xenial64"
		web2.vm.network "public_network"
		web2.vm.provider "virtualbox" do |vb|
			# Customize the amount of memory on the VM:
			vb.memory = "1024"
		end
	end
end
