# Extra Information to consider

This file is for mentioning things that are not implemented in the scripts

## To disable IP forwarding, use the following command as root:

```shell
sysctl -w net.ipv4.ip_forward=0
```

## Firewall Rules:

Here, the scripts to revert the nftables or iptables rules have also not been
implemented. The reason is that doing so might mess up with the rules that are
pre-configured by the user. So, the firewall rules created by the scripts using
either nftables or iptables should be removed or altered manually if required.
