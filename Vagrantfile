# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.network "private_network", ip: "192.168.22.222"

  config.vm.provision "ansible" do |ansible|
      # ansible.inventory_path = "ansible/inventory"
      ansible.playbook = "ansible/playbook.yml"
      ansible.galaxy_role_file = "ansible/requirements.yml"
      ansible.sudo = true
  end
end
