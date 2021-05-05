# -*- mode: ruby -*-
# vim: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "centos/8"
  config.vm.box_check_update = true
    
  config.vm.define "dynweb", primary: true do |w|
    w.vm.hostname = 'dynweb'
    w.vm.network "public_network", ip: "192.168.1.8"
	w.vm.provider :virtualbox do |v|
		v.name = "dynweb"
		v.customize ["modifyvm", :id, "--cpus", 4, "--memory", "2048"]

    end

	w.vm.provision "ansible" do |ansible|
        ansible.playbook = "dynweb.yml"
		
	end
	
  end


  
end

