This repository includes a Vagrant file for creating a VM
with all dependencies needed to work on Elixir in the class
installed. To use this repository you should

* Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](https://www.vagrantup.com/). We have tested this on VirtualBox
version 6.1.12 and Vagrant version 2.2.10. Installing either on macOS Catalina
(10.15) might need you to bypass security permissions. Please see 
[this Github issue](https://github.com/hashicorp/vagrant/issues/11127) to
figure out how.

* Clone this repository into an appropriate location.

* Run `vagrant up` to create the VM. This will download a VM image
  from the Internet, and then update it.

* Once the previous step has succeeded, you can use `vagrant ssh` to
  log into the VM. You will find `git` and Elixir (in particular `iex`
  and `mix`) installed. The VM is a Debian based VM, and you can
  add additional software using `apt`.

# Connecting from VSCode

You can follow the steps in this [blog post](https://medium.com/@lopezgand/connect-visual-studio-code-with-vagrant-in-your-local-machine-24903fb4a9de)
to connect from VSCode if that is your editor of choice.

When working with Elixir in VSCode we found the `vscode-elixir`
plugin to be particularly useful.
