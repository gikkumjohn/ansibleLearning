Vagrant.configure(2) do |config|

 config.vm.define "control" do |control|
  control.vm.box = "ubuntu/trusty64"
  control.vm.network "private_network",ip:"192.168.0.10"
  control.vm.hostname = "control"
  ansible.playbook = "nginx.yml"
 end

 config.vm.define "lb1" do |h|
  h.vm.box = "ubuntu/trusty64"
  h.vm.network "private_network",ip:"192.168.0.101"
  h.vm.hostname = "lb1"
 end

 config.vm.define "app1" do |h|
  h.vm.box = "ubuntu/trusty64"
  h.vm.network "private_network",ip:"192.168.0.102"
  h.vm.hostname = "app1"
 end

 config.vm.define "app2" do |h|
  h.vm.box = "ubuntu/trusty64"
  h.vm.network "private_network",ip:"192.168.0.103"
  h.vm.hostname = "app2"
 end

 config.vm.define "db1" do |h|
  h.vm.box = "ubuntu/trusty64"
  h.vm.network "private_network",ip:"192.168.0.110"
  h.vm.hostname = "db1"
 end

end
