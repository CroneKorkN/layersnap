layersnap
=========

overlay(fs)- and rsync-based simple snapshots

# API

`layersnap [-r|--restore <snapshot-id>] [-m|--merge] [<target-directory>]`

## without parameters

show status of current working directory

## only directory given

create new snapshot of given directory

## -r or --restore <snapshot-id>

restore given snapshot

## -m or --merge

merge with parent layer
