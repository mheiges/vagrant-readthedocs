Vagrant.configure(2) do |config|

  config.vm.box = "ebrc/centos-7.1-64-nocm"
  config.vm.box_url = 'http://software.apidb.org/vagrant/centos-7.1-64-nocm.json'


  if Vagrant.has_plugin?('landrush')
   config.landrush.enabled = true
   config.landrush.tld = 'vm'
  end

  config.vm.hostname = 'rtfd.vm'

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
