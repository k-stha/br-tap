# br-tap

Create bridge and tap interfaces easily

These are the scripts that could be used for creating and removing bridge and
tap interfaces, and enable NAT on a Unix-like machine.

## Table of Contents

- [Dependencies](#dependancies)
- [Scripts](#scripts)
- [Contributing Guidelines](#contributing-guidelines)

## Dependencies

- iproute2
- nftables or iptables (nftables recommended)
- dnsmasq-base or dnsmasq (optional)

## Scripts:

- create-br - Creates a bridge interface, and optionally runs a DHCP server on
  the interface using dnsmasq
- create-nat - Enables IP forwarding and creates firewall rules using either
  nftables or iptables
- create-tap - Creates tap interfaces for the specified bridge interface for
  the specified user
- del-br - Delete one or more bridge interfaces
- del-tap - Delete one or mote tap interfaces

**NOTE**: There is a file called 'extra.md', which contains information about
disabling IP forwarding, along with other critical information, such as why
some (obvious) things are not implemented. So, please read it before running
the scripts.

## Contributing Guidelines

See [CONTRIBUTING.md](CONTRIBUTING.md)
