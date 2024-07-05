# Disk-encryption



## Requirements
Debian-based Linux OS
Ansible-core version => 2.13.9
community.crypto module (can be installed with ansible-galaxy collection install community.crypto)

## Warnings

This role implements encryption of the disk passed as a variable encrypt_disk and encryption of the disk partition passed as a variable encrypt_partition

Assumes that the encryption disk is empty. Any actions with encrypted disk are not implemented in this role.

P.S. I have no experience with encrypting disks and partitions in linux. The information I could find on encrypting the Bios Boot partition is that you can't do it, but I added a description of a partition encryption script to the role. In my opinion, such procedures (which can break the system) are better not to be left to automation, and left to the engineer's responsibility (here it is implemented as a variable).