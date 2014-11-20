Clean Laravel 4.2 install using LEMP stack. This is a Vagrant project - https://www.vagrantup.com please read the documentation https://docs.vagrantup.com/v2
You will need the hosts-updater vagrant plugin - https://github.com/cogitatio/vagrant-hostsupdater
Windows does not have a native ssh client. I recommend PuTTY - http://www.putty.org (you will need this if you want to ssh into your vm).

To get started please:

1.) Clone repo into your project folder.
2.) Edit line 36 of puphpet/config.yaml - C:\Path\to\Your\Project\www (Windows).
3.) Open an elevated command prompt (Windows) or your cli of choice - We need administrative priveleges to be able to edit the hosts file** (this is so you can navigate to laravel.dev in your browser. you must do this everytime you want to run the vm).
4.) cd into your project root - cd C:\Path\to\Your\Project (this has to be where the Vagrantfile is stored).
5.) Run "vagrant up" (no quotes).
6.) Sit back and wait for the VM to finish provisioning.
7.) Once complete you can navigate to http://laravel.dev and you should see the Laravel default page.

**In order to ssh into your VM you must run both VirtualBox and your ssh client with elevated privileges.