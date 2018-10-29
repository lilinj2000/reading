Chapter 4. Notification Chains

- 4.1 Reasons for Notification Chains

- 4.2 Overview

- 4.3 Defining a Chain
  struct notifier_block
  {
  int (*notifier_call)(struct notifier_block *self, unsigned long, void *);
  struct notifier_block *next;
  int priority;
  };

- 4.4 Registering with a Chain

- 4.5 Notifying Events on a Chain

- 4.6 Notification Chains for the Networking Subsystems

  inetaddr_chain/inet6addr_chain
  netdev_chain​
  ​

  - 4.6.1 Wrappers
  - 4.6.2 Examples

- 4.7 Tuning via /proc Filesystem

- 4.8 Functions and Variables Featured in This Chapter

  - notifier_chain_register + wrappers
  - notifier_chain_unregister + wrappers
  - struct notifier_block

- 4.9 Files and Directories Featured in This Chapter