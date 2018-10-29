Chapter 2. Critical Data Structure

- 2.1 The Socket Buffer: sk_buff Structure

  Layout
  General
  Feature-Specific
  Management functions​​​
  ​

  - 2.1.1 Networking Options and Kernel Structures
    struct sk_buff {
    ... ... ...
    \#ifdefCONFIG_NET_SCHED
    _ _u32 tc_index;
    \#ifdefCONFIG_NET_CLS_ACT
    _ _u32 tc_verd;
    _ _u32 tc_classid;
    \#endif
    \#endif
    }
    ​
  - 2.1.2 Layout Fields
  - 2.1.3 General Fields
  - 2.1.4 Feature-Specific Fields
  - 2.1.5 Management Functions
    - 2.1.5.1 Allocating memory: alloc_skb and dev_alloc_skb
    - 2.1.5.2 Freeing memory: kfree_skb and dev_kfree_skb
    - 2.1.5.3 Data reservation and alignment: skb_reserve, skb_put, skb_push, skb_pull
    - 2.1.5.4 The skb_shared_info structure and the skb_shinfo function
    - 2.1.5.5 Cloning and copying buffers
    - 2.1.5.6 List management functions

- 2.2 net_deice Structure

  - 2.2.1 Identifiers
    - int ifindex
    - int iflink
    - unsigned short dev_id
  - 2.2.2 Configuration
    - 2.2.2.1 Interface types and ports
    - 2.2.2.2 Promiscuous mode
  - 2.2.3 Statistics
  - 2.2.4 Device Status
  - 2.2.5 List Management
  - 2.2.6 Link Layer Multicast
  - 2.2.7 Trafic Management
  - 2.2.8 Feature Specific
  - 2.2.9 Generic
  - 2.2.10 Function Pointers

- 2.3 Files Mentioned in This Chapter