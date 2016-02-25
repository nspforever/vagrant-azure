# Vagrant Azure Provider
Vagrant plugin that adds an Azure provider to Vagrant, allowing Vagrant to control and provision virtual machines in Azure


## Features
1. Supports provision Linux VM in Azure
2. Supports provision Windows VM in Azure
3. Supports SSH into Linux VM from Windows/Liunx/Mac
4. Supports SSH into Windows VM from Windows/Liunx/Mac
5. Supports doing more stuff against Azure(will put more details after the above 4 features got implemented)

## Where to start
1. Get to know what is Vagrant at [here][1]
2. Get to know how to develop a Vagrant plugin at [here][2]
3. Take the vagrant-aws plugin as an example:
> - [plugin.rb][3] defines the plugin
> - [provider.rb][4] implements the provider
> - [config.rb][5] implements the config
4. SSH solution
> - [Win32-OpenSSH][6] will be used as the SSH client for windows client
> - [Win32-OpenSSH][6] will be used as the SSH server for windows VM in Azure
> - [Cgwin][7] is an alternative if Win32-OpenSSH is not ready
> - [Putty and pscp][8] is another alternative


    
    
    
[1]: https://www.vagrantup.com/docs/getting-started/
[2]: https://www.vagrantup.com/docs/plugins/development-basics.html
[3]: https://github.com/mitchellh/vagrant-aws/blob/master/lib/vagrant-aws/plugin.rb
[4]: https://github.com/mitchellh/vagrant-aws/blob/master/lib/vagrant-aws/provider.rb
[5]: https://github.com/mitchellh/vagrant-aws/blob/master/lib/vagrant-aws/config.rb
[6]: https://github.com/PowerShell/Win32-OpenSSH/wiki/Install-Win32-OpenSSH
[7]: https://www.cygwin.com/
[8]: http://www.putty.org/