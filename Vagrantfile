
Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu1804"
  # Install Docker
  config.vm.provision "docker" do |d|
    
  end
  #Run bash code
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.provision :docker_compose, yml: "/vagrant/docker-compose.yml", rebuild: true, run: "always"

end