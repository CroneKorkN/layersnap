layersnap
=========

overlayfs- and rsync-based simple snapshots

# UI

`layersnap [-s|--snapshot|-m|--merge|-r|--restore] <target-directory>`

## without additional parameters

* show status of target-directory and mounts it if neccessary

## -s (or --snapshot) \<target-directory\>

* create snapshot of target-directory

## -r (or --restore) \<target-directory\>

* shows a list of snapshot-layers
* asks interactively for snapshot to restore
* restores given snapshot and deletes all layersnap-stuff related to target-directory

## -m (or --merge) \<target-directory\>

* merges range of layers to restore performance
* asks interactively for starting-layer and target-layer
* merges layers and remounts 

# compatibility

layersnap has two operational modes.

## legacy-mode

compatible with
* Linux kernel 3.18 and newer
* Ubuntu 12.04 and newer (at least)
* max two layers

Older overlayfs implemantations accepted only one lower-dir. But two overlayfs' can be stacked either and so does layersnap. Thus, snapshots are limited to two.


## multi-mode

compatible with
* Linux kernel 4.0 and newer
* Ubuntu 14.04 and newer (at least)

Newer overlayfs-implementations accept multiple lower-dirs and so layersnap theoretically provides an unlimited amount of snapshots.
