# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'danmaq/openSUSE-42.1-x86_64-Android-Qt-dev-env'
  config.vm.provider 'virtualbox' do |vb|
    vb.name = 'Android video-app dev env using Qt'
    vb.gui = true
    vb.linked_clone = true
    vb.cpus = 2
    vb.memory = '1536'
    vb.customize [
      'modifyvm', :id,
      '--accelerate3d', 'off',
    ]
    # Enabling sounds on Windows / macOS.
    if (/cygwin|mswin|mingw|bccwin|wince|emx/ =~ RUBY_PLATFORM) != nil
      vb.customize [
        'modifyvm', :id,
        '--audio', 'dsound',
        '--audiocontroller', 'ac97'
      ]
    elsif (/darwin/ =~ RUBY_PLATFORM) != nil
      vb.customize [
        'modifyvm', :id,
        '--audio', 'coreaudio',
        '--audiocontroller', 'ac97'
      ]
    end
  end
  config.vm.provision 'ansible_local' do |ansible|
    ansible.playbook = 'playbook.yml'
    ansible.limit = 'all'
    ansible.verbose = false
    ansible.install = true
  end
end
