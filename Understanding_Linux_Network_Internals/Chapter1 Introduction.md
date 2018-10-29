- Chapter 1. Introduction
  - 1.1 Basic Terminology
    - L2 -> Link layer (e.g., Ethernet)
    - L3 -> Network layer(e.g., IP)
    - L4 -> Transport layer (e.g., UDP/TCP/ICMP)
    - BH -> Bottom half
    - IRQ -> Interrupt
    - RX -> Reception
    - TX -> Transmission
  - 1.2 Common Coding Patterns
    - 1.2.1 Memory Caches
      - kmalloc/kfree
      - kmem_cache_create/kmem_cache_destroy
      - kmem_cache_alloc/kmem_cache_free
    - 1.2.2 Caching and Hash Tables
    - 1.2.3 Reference Counts
      - xxx_hold/xxx_release
    - 1.2.4 Garbage Collection
      - Asynchronous
      - Synchronous
    - 1.2.5 Function Pointers and Virtual Function Tables(VFTs)
      struct sock {
      ...
      void (*sk_state_change)(struct sock *sk);
      void (*sk_data_ready)(struct sock *sk, int bytes);
      ...
      };
    - 1.2.6 goto Statements
    - 1.2.7 Vector Definitions
      struct abc {
      int age;
      char *name[20];
      ...
      char placeholder[0];
      }
    - 1.2.8 Conditional Directives (#ifdef and family)
    - 1.2.9 Compile-Time Optimization for Condition Checks
      - likely
      - unlikely
    - 1.2.10 Mutual Exclusion
      - Spin locks
      - Read-write spin locks
      - Read-Copy-Update (RCU)
    - 1.2.11 Conversions Between Host and Network Order
      - htons (short)
      - htonl (long)
      - ntohs (short)
      - ntohl (long)
    - 1.2.12 Catching Bugs
      - BUG_ON (kernel error message)
      - BUG_TRAP (kernel warning message)
    - 1.2.13 Statistics
    - 1.2.14 Measuring Time
  - 1.3 User-Space Tools
    - iputils
      - ping
      - arping
      - rdisc
    - net-tools
      - ifconfig
      - route
      - netstat
      - arp
      - ipmaddr
      - iptunnel
      - ether-wake
      - netplugd
    - IPROUTE2
      - ip
      -  <http://linux-net.osdl.org/index.php/Iproute2>
    - URLs
      -  <http://lartc.org>
      - <http://www.policyrouting.org>
      - <http://www.netfilter.org>
      - The Linux Network Development List Archives (<http://oss.sgi.com/projects/netdev/archive>)
  - 1.4 Browsing the Source Code
    - 1.4.1 Dead Code
  - 1.5 When a Feature Is Offered as a Patch