Vagrant.configure("2") do |config|
    config.vm.provider "virtualbox"
    config.vm.box = "ubuntu/bionic64"
    config.vm.synced_folder "src/", "/var/www/html/", id: "vagrant-root", :owner => "www-data", :group => "www-data"
    config.vm.network :forwarded_port, guest: 80, host: 80
end