Terraform OpenStack Provider
============================

- Website: https://www.terraform.io
- [![Gitter chat](https://badges.gitter.im/hashicorp-terraform/Lobby.png)](https://gitter.im/hashicorp-terraform/Lobby)
- Mailing list: [Google Groups](http://groups.google.com/group/terraform-tool)

<img src="https://cdn.rawgit.com/hashicorp/terraform-website/master/content/source/assets/images/logo-hashicorp.svg" width="600px">

Maintainers
-----------

This provider plugin is maintained by:

* Andrei Ozerov ([@ozerovandrei](https://github.com/ozerovandrei))
* Gavin Williams ([@fatmcgav](https://github.com/fatmcgav))
* Joe Topjian ([@jtopjian](https://github.com/jtopjian))

Requirements
------------

-	[Terraform](https://www.terraform.io/downloads.html) 0.11.x
-	[Go](https://golang.org/doc/install) 1.11 (to build the provider plugin)

Building The Provider
---------------------

Clone repository to: `$GOPATH/src/github.com/terraform-providers/terraform-provider-openstack`

```sh
$ mkdir -p $GOPATH/src/github.com/terraform-providers; cd $GOPATH/src/github.com/terraform-providers
$ git clone https://github.com/terraform-providers/terraform-provider-openstack
```

Enter the provider directory and build the provider

```sh
$ cd $GOPATH/src/github.com/terraform-providers/terraform-provider-openstack
$ make build
```

Using the provider
----------------------
Please see the documentation at [terraform.io](https://www.terraform.io/docs/providers/openstack/index.html).

Or you can browse the documentation within this repo [here](https://github.com/terraform-providers/terraform-provider-openstack/tree/master/website/docs).

Developing the Provider
---------------------------

If you wish to work on the provider, you'll first need [Go](https://golang.org) installed on your machine (version 1.11+ is *required*). You'll also need to correctly setup a [GOPATH](https://golang.org/doc/code.html#GOPATH), as well as adding `$GOPATH/bin` to your `$PATH`.

To compile the provider, run `make build`. This will build the provider and put the provider binary in the `$GOPATH/bin` directory.


```sh
For Linux
$ make build
---
For Windows
$ go build -o terraform-provider-openstack
$ go install github.com/terraform-providers/terraform-provider-openstack
...
$ $GOPATH/bin/terraform-provider-openstack
...
```

For further details on how to work on this provider, please see the [Testing and Development](https://www.terraform.io/docs/providers/openstack/index.html#testing-and-development) documentation.

Thank You
---------

We'd like to extend special thanks and appreciation to the following:

### OpenLab

<a href="http://openlabtesting.org/"><img src="assets/openlab.png" width="600px"></a>

OpenLab is providing a full CI environment to test each PR and merge for a variety of OpenStack releases.

### VEXXHOST

<a href="https://vexxhost.com/"><img src="assets/vexxhost.png" width="600px"></a>

VEXXHOST is providing their services to assist with the development and testing of this provider.


