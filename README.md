# snapDisk - ZFS Snapshot Management Script

This is a Bash script for managing ZFS snapshots. It allows you to create and remove snapshots easily.

## Prerequisites

- Linux with ZFS installed.
- Sufficient permissions to run `zfs` commands with `sudo`.

## Usage

1. Clone or download this repository.

2. Make the script executable:

   ```bash
   chmod +x snapDisk
   ```

### Create Snapshot

```sh
$ ./snapDisk -c | --create
```

### List Snapshots

```sh
$ ./snapDisk -l | --list

Available snapshots:
0. rpool/USERDATA@2023-10-10_22:49:18
1. rpool/USERDATA/username_b56lyv@2023-10-10_22:49:11
```

### Remove Snapshot

```sh
$ ./snapDisk -r | --remove 0 1

Snapshot removed: rpool/USERDATA@2023-10-10_22:49:18
Snapshot removed: rpool/USERDATA/username_b56lyv@2023-10-10_22:49:11
```
