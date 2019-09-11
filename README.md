# ansible-xmrig
Ansible Playbook to compile XMRIG miner for Monero mining from GIT source, builds miner on all nodes and runs automatically at server boot.
XMRig is high performance Monero (XMR) CPU miner. Originally based on cpuminer-multi with heavy optimizations/rewrites and removing a lot of legacy code, since version 1.0.0 complete rewritten from scratch on C++.

Currently tested on:
* Ubuntu Disco

### 1 - Configuration

Create new hosts file using *hosts.yml.example*
Update variables:

`public_key` : SET YOUR XMR PUBLIC KEY

`mining_pool` : SET MONERO POOL (eg. mine.moneropool.com:3333)

You can find a list of available Monero pools here:
http://moneropools.com/


### 2 - Run

```
ansible-playbook playbooks/lxd-xmrig.yml
```

### 3 - Enjoy mining!

XMRIG miner starts in background mode by default
