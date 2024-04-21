### Synology models that officially support data deduplication

https://kb.synology.com/en-global/DSM/tutorial/Which_models_support_data_deduplication

**Which Synology NAS models support data deduplication?**
- FS6400, FS3600, FS3410, FS3400, FS2500
- HD6500
- SA6400, SA3610, SA3600, SA3410, SA3400
- RS4021xs+, RS3621xs+, RS3621RPxs

**Requirements:**

- Data deduplication is only supported on Synology SSDs and Btrfs volumes. You need to create a storage pool consisting entirely of Synology SSDs and then create at least one Btrfs volume.
- Data deduplication can only run when the volume status is Healthy.
- Data deduplication requires you to Enable usage detail analysis for the Btrfs volume.

**Notes:**

- RS3621xs+/RS3621RPxs and FS2500 need at least 16 GB of memory to enable data deduplication.

<br>

**Configure Data Deduplication:**

https://kb.synology.com/en-global/DSM/help/DSM/StorageManager/volume_btrfs_dedup?version=7

<br>

**Configure Snapshot Replication and Data Deduplication:**

https://kb.synology.com/en-global/DSM/tutorial/Configure_snapshot_replication_and_data_deduplication

<br>

***

### Undocumented models that support data deduplication

DiskStation models that support Tiny Btrfs Data Deduplication in DSM 7.2.1

- DS1522+, DS1621+, DS1621xs+, DS1821+, DS1823xs+, DS423+, DS723+ and DS923+.

These models have "tiny btrfs data deduplication" enabled and only need 4GB of memory or more.

In my test on a DS720+ with only 2GB of memory I got a message saying at 4GB of system memory was needed.
https://www.reddit.com/r/synology/comments/18oyu21/data_deduplication_only_needs_4gb_of_memory/

<br>
