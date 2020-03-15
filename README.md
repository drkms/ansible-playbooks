Ansible Playboos Repository !
==========================

These playbooks aim to help you install several basic setup in order to quickly get a comfortable desktop environment.

It can be installed inside a Vagrant machine using the Ansible provisionner :

```ruby
Vagrant.configure("2") do |config|
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "/home/vagrant/name_of_the_playbook/playbook.yml"
  end
end
```

You can also run it locally to be sure you are up to date
```shell
ansible-playbook playbook.yml --connection=local -i inventory --ask-become-pass
```

You can try it remotely using Packer or Terraform

```json
....
```

It allow you to have a perfect reflexivity on every platform.


