# monerod-bootstrap
Monero Remote node bootstrapper

Based on the awesome guide from: https://sethforprivacy.com/guides/run-a-monero-node-advanced/

How to use
```bash
Monerod Easy Install Script for setting up remote node.
Usage: monero_remote_node.sh [-p|--profile <arg>] [-h|--help] [<action>]
        <action>: Action to perform. install or upgrade (optional) (default: 'install')
        -p, --profile: Monerod RPC profile type.  (optional) (default: 'monerod_public_restricted_pruned')
        -h, --help: Prints help
```

To install remote node with defaults use:
```
wget https://raw.githubusercontent.com/meramsey/monerod-bootstrap/main/monero_remote_node.sh
bash monero_remote_node.sh install
```

To upgrade an existing remote node installed from this script:
```
bash monero_remote_node.sh upgrade
```

### Config profile options are below:
- monerod    
- monerod_pruned    
- monerod_public_restricted    
- monerod_public_restricted_pruned      


#### To install with specific profile:
```
bash monero_remote_node.sh install --profile monerod_public_restricted
```

Features:
Auto install of monerod install/upgrade
Tor onion setup
