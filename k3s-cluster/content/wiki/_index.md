---
linkTitle: Documentation
title: Introduction
cascade:
  type: docs
---

The documentation is presented as a learning tool, allowing the end-user to understand all configuration and deployment aspects of a bare-metal based K3s cluster.

<!--more-->

## Cluster Hardware

The following hardware was used to deploy the cluster:

- 8 x Raspberry Pi 4 Model B with 8GB RAM
- 8 x GeeekPi [Isolated PoE HAT](https://www.amazon.com/gp/product/B08CVDQWXF/) for Raspberry Pi 4 Model B
- 8 x Samsung PM883 240GB SSD, connected to same USB port
- 8 x SLK Tech [Sata to USB](https://www.amazon.com/gp/product/B07S9CKV7X/) cable
- UniFi [UDM-SE](https://store.ui.com/us/en/collections/unifi-dream-machine/products/udm-se) cloud gateway, for dedicated network management
- UniFi [USW-Pro-24-POE](https://store.ui.com/us/en/collections/unifi-switching-pro-power-over-ethernet/products/usw-pro-24-poe) switch, powering the Raspberry Pi's

## Network

Prior starting the cluster configuration, the end-user must determine if the [network](/k3s-cluster/tutorials/handbook/network) configuration can support **load balancing** with [external IP addresses](https://kubernetes.io/docs/tutorials/stateless-application/expose-external-ip-address) assigned from a load balancer [IP pool](https://docs.cilium.io/en/stable/network/lb-ipam). Some retail routers do not have this capability.

## Next

Dive right into the following section, to get started:

{{< cards >}}
  {{< card icon="adjustments" link="getting-started" title="Getting Started" subtitle="Set the local deployment environment." >}}
{{< /cards >}}
