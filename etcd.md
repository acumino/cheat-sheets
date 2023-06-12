**Connecting to the etcd Cluster:**
- `etcdctl --endpoints=<endpoint1>,<endpoint2>,... <command>`: Connect to the etcd cluster.

**Key-Value Operations:**
- `etcdctl put <key> <value>`: Set a key-value pair.
- `etcdctl get <key>`: Get the value of a key.
- `etcdctl get --prefix <prefix>`: List keys with a prefix.
- `etcdctl del <key>`: Delete a key.
- `etcdctl del --prefix <key>`: Delete a key and its associated range.
- `etcdctl put --lease=<lease_id> <key> <value>`: Set a key-value pair with a lease.
- `etcdctl txn --interactive`: Set a key-value pair with a transaction.
- `etcdctl watch <key> [--prefix]`: Watch for changes on a key or prefix.

**Directory Operations:**
- `etcdctl mkdir <directory>`: Create a directory.
- `etcdctl ls <directory>`: List all keys under a directory.
- `etcdctl rmdir <directory>`: Delete a directory and all its contents.

**Lease Operations:**
- `etcdctl lease grant <ttl>`: Create a lease.
- `etcdctl lease revoke <lease_id>`: Revoke a lease.
- `etcdctl lease keep-alive <lease_id>`: Keep a lease alive.

**Cluster Operations:**
- `etcdctl cluster-health`: Get the status of the etcd cluster.
- `etcdctl endpoint health`: Check the health of the cluster.
- `etcdctl member list`: List all members in the cluster.
- `etcdctl member add <name> --peer-urls=<peer_urls>`: Add a new member to the cluster.
- `etcdctl member remove <member_id>`: Remove a member from the cluster.
- `etcdctl member update <member_id> --peer-urls=<new_peer_urls>`: Update a member's peer URLs.
- `etcdctl member promote <member-id>`: Promote a non-voting member to a voting member.

**Snapshot Operations:**
- `etcdctl snapshot save <filename>`: Create a snapshot.
- `etcdctl snapshot restore <filename>`: Restore a snapshot.

**Authentication and Authorization:**
- `etcdctl auth enable`: Enable authentication.
- `etcdctl auth disable`: Disable authentication.
- `etcdctl user add <user>`: Add a user.
- `etcdctl user delete <user>`: Delete a user.
- `etcdctl user grant-role <user> <role>`: Grant a role to a user.
- `etcdctl user revoke-role <user> <role>`: Revoke a role from a user.
- `etcdctl user list`: List users.
- `etcdctl role add <role>`: Add a role.
- `etcdctl role delete <role>`: Delete a role.
- `etcdctl role grant-permission <role> <permission_type> <key> [--range-end=<range_end>]`: Grant a permission to a role.
- `etcdctl role revoke-permission <role> <key> [--range-end=<range_end>]`: Revoke a permission from a role.
- `etcdctl role remove <role>`: Remove a role.
- `etcdctl role list`: List roles.

**Maintenance Operations:**
- `etcdctl compact <revision>`: Compact the event history.
- `etcdctl defrag`: Defragment the storage backend.
- `etcdctl alarm list`: Check the alarm list.
- `etcdctl alarm disarm <alarm_type>`: Disarm an alarm.
- `etcdctl --endpoints=<endpoints> put /0/metadata/config/force-new-cluster true`: Set the election timeout.
- `etcdctl --endpoints=<endpoints> put /0/metadata/config/heartbeat-interval <interval>`: Set the heartbeat interval.
