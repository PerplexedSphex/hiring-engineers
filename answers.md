Your answers to the questions go here.

# Level 0

Before starting this exercise, it is necessary to download VirtualBox and Vagrant. These will allow us to create a fresh ubuntu virtual machine, which we can bring online with the following:

```
$ vagrant init hasicorp/precise64
$ vagrant up 
```

More complete instructions to using Vagrant can be found [here](https://www.vagrantup.com/docs/getting-started/).

# Level 1

Once our VM is running, we can install the Data Dog Agent.

```
$ vagrant ssh
$ bash -c "$(curl -L https://raw.githubusercontent.com/DataDog/dd-agent/master/packaging/datadog-agent/source/install_agent.sh)"
```

NOTE: For this install script to work, first set the shell variable $DD_API_KEY equal to your api key.


