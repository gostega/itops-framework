# Proxmox - Can't remove unused VM disk

## Symptoms:

- Have detached several unneeded disks from an existing running VM
- The disks no longer show up in the VM hardware pane
- The disks still exist in the storage under Content
- When clicking Remove on the disk, you get "Cannot remove image, a guest with VMID '107' exists! You can delete the image from the guest's hardware pane"
- Command `qm rescan` doesn't do anything

## Cause

Unknown. Bug?

## Workaround

- Ran command `pvesm free $storagename:$VMID/$vmdiskname.$extension`
- i.e. the command was: `pvesm free TOULA-ZFS-Storage:107/vm-107-disk-1.raw`
- Result was `"Removed volume 'TOULA-ZFS-Storage:vm-107-disk-1'"`
  > Note: recently I went to do this again and the command appeared to be `TOULA-ZFS-Storage:vm-105-disk-1`, no `105/` required.

## Solution

- Update to PVE 7.x
