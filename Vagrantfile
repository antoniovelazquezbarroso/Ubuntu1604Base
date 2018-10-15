# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.provider :virtualbox do |v|
    v.memory = 512
    v.cpus = 1
  end

  config.vm.box = "geerlingguy/ubuntu1604"

  config.vm.hostname = "Ubuntu1604Base"

#  config.vm.network :private_network, ip: "192.168.2.88"
  config.vm.network :public_network, ip: "192.168.1.15", bridge: "en0: Ethernet"

  config.ssh.insert_key = false
#  config.vm.synced_folder '.', '/vagrant', disabled: true

#  # Ansible provisioning.
#  config.vm.provision "ansible" do |ansible|
#    ansible.playbook = "playbooks/nginx_install.yml"
#    ansible.sudo = true
#  end

end
