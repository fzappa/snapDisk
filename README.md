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

```sh
./snapDisk
Choose an option:
1. Create a snapshot
2. List and remove snapshots
Option: 1

Available datasets:
rpool/USERDATA
Enter the dataset name to create a snapshot: rpool/USERDATA

Snapshot created: rpool/USERDATA@2023-10-10_22:49:18
```

```sh
./snapDisk
Choose an option:
1. Create a snapshot
2. List and remove snapshots
Option: 2

Available snapshots:
0. rpool/USERDATA@2023-10-10_22:49:18
1. rpool/USERDATA/alan_b56lyv@2023-10-10_22:49:11

Enter the numbers of the snapshots to remove (separated by space): 0 1

Snapshot removed: rpool/USERDATA@2023-10-10_22:49:18
Snapshot removed: rpool/USERDATA/alan_b56lyv@2023-10-10_22:49:11
```
