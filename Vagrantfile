# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
	config.vm.box = "00gavin/centos71"
	config.vm.box_url = "centos-71-x64-virtualbox-minimal.box"
	config.vm.provider :virtualbox do |p|
		p.customize ["modifyvm", :id, "--memory", 1024]
		p.customize ["modifyvm", :id, "--cpus", 2]
		p.customize ["modifyvm", :id, "--cpuexecutioncap", 50]
	end
	config.vm.hostname = "centos71"
	config.vm.network "forwarded_port", guest: 80, host: 8000
	#config.vm.provision :shell, path: "bootstrap.sh"
	#config.vm.provision "ansible" do |ansible|
	#	ansible.playbook = "provisioning/site.yml"
	#	ansible.host_key_checking = false
	#	ansible.raw_ssh_args = '-o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no -o PasswordAuthentication=no -o IdentitiesOnly=yes'
	#end
end
