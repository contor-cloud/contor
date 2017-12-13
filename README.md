# Contor
## Communications Cloud
[![Join the Chat on irc.freenode.org #contor](https://img.shields.io/badge/irc-freenode:%20%23contor-blue.svg)](http://webchat.freenode.net/?channels=%23contor)
[![License: ALv2](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://opensource.org/licenses/Apache-2.0)

## :construction: WARNING - WORK IN PROGRESS :warning:
This project is a Work In Progress and not ready for deployment, yet! Please consider contributing!

## Introduction

The objective of the Contor project is to provide the user with the means to set up their own personal cloud on their web domain using only open source software, so they're in full control of their data. It aims to provide cloud-storage, email, contacts, calendar, chat and videochat capabilities, all accessible through a browser interface or synced to their favourite app. With a highly-automated setup on a Kubernetes cluster it is easily deployed to any infrastructure, be it self-hosted or cloud-provided by a third-party, and can be maintained, managed and scaled with little effort.

## Containers

Contor will be distributed as an [Ansible Playbook Bundle](https://github.com/ansibleplaybookbundle/ansible-playbook-bundle) for use on [Service Catalog](https://github.com/kubernetes-incubator/service-catalog)-enabled [Kubernetes](https://github.com/kubernetes/kubernetes) clusters. The initial focus will lie on supporting the [OpenShift](https://github.com/openshift/origin) Kubernetes distribution. Check back here later for information on installation, setup and deployment.

## Built On Top Of / With

Base Technology Stack:
* [Ansible Playbook Bundle](https://github.com/ansibleplaybookbundle/ansible-playbook-bundle) - Packaging Format of the Contor Deliverable
* [Fedora](https://getfedora.org/) - Container Base Operating System
* [Kubernetes](https://github.com/kubernetes/kubernetes) - PaaS
* [OpenShift Origin](https://github.com/openshift/origin) - Recommended Kubernetes Distribution for Contor
* [Ansible Service Broker](https://github.com/openshift/ansible-service-broker) - Implementation of the Open Service Broker API
* [Kubernetes Service Catalog](https://github.com/kubernetes-incubator/service-catalog) - Integration with the Service Broker
* [OpenShift ACME](https://github.com/tnozicka/openshift-acme) - Automatic Let's Encrypt Certificate Retrieval & Management for K8s Pods

Features planned for the initial Release:

:construction: Implementation of these services is currently a WIP :warning:
* [FreeIPA](https://github.com/freeipa/freeipa) - User Identity & Policy Management Server
* [Dovecot](https://github.com/dovecot/) - IMAP + Sieve Server
* [Postfix](http://www.postfix.org/) - SMTP Server
* [Rspamd](https://github.com/vstakhov/rspamd/) - Rapid Mail Filter
* [Clamd](https://github.com/vrtadmin/clamav-devel) - Anti Virus
* [NextCloud](https://github.com/nextcloud) - File Storage, DAV & Frontend Server
* [LibreOffice Online](https://github.com/LibreOffice/online) - Office Apps
* [Prosody](https://hg.prosody.im/) - XMPP Server

Features on the Roadmap for later Releases:
* [HomeAssistant](https://github.com/home-assistant/home-assistant) - Home Automation & IoT Hub
* [Kazoo](https://github.com/2600hz/kazoo) - PBX & SIP-Trunk
* [Coturn](https://github.com/coturn/coturn) - TURN/STUN & ICE Server

## Topology

![Contor Cloud Topology](docs/topology.svg)
Federated Kubernetes Cluster

## Contributing

Please read [CODE_OF_CONDUCT.md](https://github.com/contor-cloud/contor/blob/master/CODE_OF_CONDUCT.md) for details on our code of conduct, and [CONTRIBUTING.md](https://github.com/contor-cloud/contor/blob/master/CONTRIBUTING.md) for sending pull requests and contributing to Contor.

## Authors

* **Christian Glombek** - *Initial work* - [LorbusChris](https://github.com/LorbusChris)

See also the list of [contributors](https://github.com/contor-cloud/contor/graphs/contributors) who participated in this project.

## License

This project is licensed under the Apache License, Version 2.0, Copyright © 2017 Christian Glombek.

See [LICENSE](https://github.com/contor-cloud/contor/LICENSE) for more information.

## Acknowledgments

This project builds on a long line of earlier work by clever folks all around the world. We'd like to thank the authors and contributors of all the projects mentioned in the `Built With / On Top Of` section of this document.
