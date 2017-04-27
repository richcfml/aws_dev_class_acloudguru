## Volumes and Snapshots

### Lab

commands:

lsblk to view the volumes available
file -s /dev/xvdf to view if a volume has data. /dev/xvddf is a sample volume. If the response states volume: data it means that there is no data at all
mkfs -t ext4 /dev/xvdf this is to format the new volume as ext4 file system
mount /dev/xvdf /fileserver to mount the new formatted volume and pass the volume name and the path where it should be mounted
umount /dev/xvdf to unmount the volume from its current point


Notes:

Volumes exists on Elastic Block Storage(EBS)
	A volume is a virtual HD

Snapshots are stored on S3
Snapshots are point copies of volumens
Snapshtos are incremental, which means that only the blocks that have changes since your last snapshot are moved to S3
The first snapshot may take some time to create