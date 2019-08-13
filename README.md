# bionic64
Packer bionic64 image for vagrant projects

# Pre-requisites
- Install [Packer](https://www.packer.io/intro/getting-started/install.html)
- Account on Vagrant [cloud](https://app.vagrantup.com/) *optional


# Usage
```bash
packer build bionic64.json
```

then you can upload created box to Vagrant [cloud](https://app.vagrantup.com/) and use it as your vagrant environment

```bash
Vagrant.configure("2") do |config|
  config.vm.box = "apopa/bionic64"
  config.vm.box_version = "0.1"
end
```
