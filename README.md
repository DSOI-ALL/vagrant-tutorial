vagrant-tutorial
================

As mentioned in our [Vagrant Post](http://blog.sei.cmu.edu/post.cfm/devops-technologies-vagrant-345), [Vagrant](https://www.vagrantup.com/) is a tool to generate virtualized and provisioned environments based on a single, declarative script. Our tutorials will always include a Vagrantfile (the script that defines the virtual machine in which our tutorials will run).

To use Vagrant with our tutorials, follow the below steps:

1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
2. Install [Vagrant](https://www.vagrantup.com/downloads.html)
3. Download a zip container of a tutorial. In this case, we will use the [SLS Vagrant Tutorial](https://github.com/SLS-ALL/vagrant-tutorial)
4. From your command line, navigate to the extracted tutorial folder.
5. From within the tutorial folder run `vagrant up`.
6. Once the script has finished running, run `vagrant ssh`.

At this point you will be logged in to a running virtual machine that will have the same environment we are developing our tutorials in. This way, you will be able to follow the tutorials and get the anticipated results. Enjoy the tutorial!

When you are finished with the tutorial, and you want to discard the vagrant virtual machine, there are a few more steps to take.

1. From within the vagrant session, run `exit`. This command ends your session in the virtual machine and you will exit back to the tutorial directory.
2. From within the tutorial directory, run `vagrant halt`. This will shutdown the virtual machine.
3. Finally, run `vagrant destroy`. This command destroys the virtual machine used to run the tutorial.
