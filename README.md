# vagrant-puppet-jenkins-server-demo

This is a demonstration of how to configure a Jenkins server using [Vagrant](https://www.vagrantup.com/) and [Puppet](https://puppet.com/) for provisioning.

## Onward to victory!

Server Specs:

Ubuntu 16.04 LTS

Jenkins 2.121.1

#### Warning! Jenkins is running without security with this build. This build does not attempt to address all security concerns that would need to occur in a production environment.

The server OS could be changed to your personal liking in the Vagrantfile:

```
config.vm.box = "puppetlabs/ubuntu-16.04-64-puppet"
```

... and the Puppet manifest would need to change to reflect installation options offered in your particular OS of choice but, these things are possible.

#### \<\-\- Do not skip reading this! \-\-\>

First, please use the latest version of [Vagrant](https://www.vagrantup.com/). At the time of this writing I am using 2.1.1. I have not tried this with older versions, it might work or it might not.

Second, I am on macOs Sierra Version 10.12.6. Therefore my instructions will be tailored towards using a terminal in a \*nix environment.

### Let's begin..

Open a terminal and navigate to where you would like a new directory to live. I personally keep all my repos and those I clone in a symlinked directory under my home directory called repos, very funny... I mean practical, I know but, I am not one to tell you how to organize your life/computer(computer life?). Ok, time for some fun stuff!

1. Clone this repo:

... [or learn about cloning repos](https://help.github.com/articles/cloning-a-repository/)

git clone https://github.com/jlmoody/effective-goggles.git

2. Change directory:

cd effective-goggles

3. Do the thing:

vagrant up

Now sit back, sip your favorite beverage and let the magic happen... oh we're done. This process takes less than a minute on my machine, hopefully on yours too.

Navigate to your new install of [Jenkins](https://jenkins.io/):

http://127.0.0.1:8080/

Note: Jenkins has been configured to run on port 8000, Vagrant is port forwarding on 8080 to avoid collisions.

Party!