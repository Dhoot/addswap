# Add swap to your VM

This Chef recipe adds swap to your VM. Particularly useful when running `npm install` or `composer udpate` of having problem which can use a lot of memory and be killed during the provisioning.

Tested on Vagrant + Ubuntu 16.04.

Source : [https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-16-04]

Add in your Berksfile

    cookbook 'addswap', git: 'git://github.com/dhoot/addswap.git'

and add recipe 'addswap' in your run list.
