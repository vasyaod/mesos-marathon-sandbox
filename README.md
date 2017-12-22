# Mesos and Marathon Vagrant sandbox with configured CNI bridge

## Requirements

* [Vagrant][1]
* [Ansible 2.x][2]

## How to start the sandbox?

`git clone` the project on your machine and run `vagrant up` in the project root.
Mesos master should be available on `10.10.10.10:5050` and Marathon on 
`10.10.10.10:8080`.

## See also

* [Mesos CNI documentation][3]
* [Marathon networking documentation][4]

[1]: https://www.vagrantup.com/
[2]: https://www.ansible.com/
[3]: https://mesos.apache.org/documentation/latest/cni/
[4]: https://mesosphere.github.io/marathon/docs/networking.html