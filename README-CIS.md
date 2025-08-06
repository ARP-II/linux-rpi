# Case-insensitive filesystem patch

The following kernel files clashes when using a case-insensitive filesystem.
This patch renames or deletes the conflicting files.

```
include/uapi/linux/netfilter_ipv4/ipt_ECN.h
include/uapi/linux/netfilter_ipv4/ipt_TTL.h
include/uapi/linux/netfilter_ipv6/ip6t_HL.h
include/uapi/linux/netfilter/xt_CONNMARK.h
include/uapi/linux/netfilter/xt_DSCP.h
include/uapi/linux/netfilter/xt_MARK.h
include/uapi/linux/netfilter/xt_RATEEST.h
include/uapi/linux/netfilter/xt_TCPMSS.h
net/netfilter/xt_DSCP.c
net/netfilter/xt_HL.c
net/netfilter/xt_RATEEST.c
net/netfilter/xt_TCPMSS.c
tools/memory-model/litmus-tests/Z6.0+pooncelock+poonceLock+pombonce.litmus
```
