#
# Vagrant script for setting up a WordPress install on Nginx
#
# * "THE BEER-WARE LICENSE" (Revision 42):
# * Dustin Warren (@dustyfresh) wrote this file. As long as you retain this notice you
# * can do whatever you want with this stuff. If we meet some day, and you think
# * this stuff is worth it, you can buy me a beer in return
# * - Poul-Henning Kamp
#

Vagrant.configure("2") do |config|

## VM configuration
	config.vm.box = 'ubuntu14.04'
	config.vm.box_url = ''
	#config.vm.network 'public_network'
	
    config.vm.define :dvwa do |dvwa|
		dvwa.vm.provider :virtualbox do |v|
			v.name = "dvwa.dev"
			v.customize ["modifyvm", :id, "--memory", "1024", "--cpus", 4]
		end
		dvwa.vm.network :public_network
		dvwa.vm.hostname = "dvwa.dev"
		dvwa.vm.provision :shell, :path => "bootstrap.sh"
	end
end
