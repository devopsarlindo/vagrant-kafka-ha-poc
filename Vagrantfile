Vagrant.configure(2) do |config|

  config.vm.box = "bento/centos-7.2"
  config.vm.box_download_insecure = true
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
  
  config.vm.define "node1" do |node1|
      node1.vm.network "private_network", ip: "192.168.33.60"
      node1.vm.hostname = "node1"
      node1.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end
   
   config.vm.define "node2" do |node2|
      node2.vm.network "private_network", ip: "192.168.33.61"
      node2.vm.hostname = "node2"
      node2.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end

  config.vm.define "node3" do |node3|
      node3.vm.network "private_network", ip: "192.168.33.62"
      node3.vm.hostname = "node3"
      node3.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end

  config.vm.define "node4" do |node4|
      node4.vm.network "private_network", ip: "192.168.33.63"
      node4.vm.hostname = "node4"
      node4.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end
   
   config.vm.define "node5" do |node5|
      node5.vm.network "private_network", ip: "192.168.33.64"
      node5.vm.hostname = "node5"
      node5.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end

   config.vm.define "node6" do |node6|
      node6.vm.network "private_network", ip: "192.168.33.65"
      node6.vm.hostname = "node6"
      node6.vm.provider "virtualbox" do |v|
        v.customize ["modifyvm", :id, "--memory", "1024"]
	      v.customize ["modifyvm", :id, "--cpus", "1"]
        v.customize ["storagectl", :id,"--name", "SATA Controller","--hostiocache", "on"]
      end
   end

end
