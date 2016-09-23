layersnap
=========

overlay(fs)- and rsync-based simple snapshots

# API

`layersnap [-s|--snapshot|-m|--merge|-r|--restore] [<target-directory>]`

## without parameters

show status of current working directory

## only directory given

show status of given directory

## -s or --snapshot [<target-directory>]

create snapshot of cwd or target, if given

## -r or --restore

restore snapshot

## -m or --merge

merge snapshot with production





layersnap FUTURE
================

overlay(fs)- and rsync-based simple snapshots

# API

`layersnap [-r|--restore <snapshot-id>] [-m|--merge] [<target-directory>]`

## without parameters

show status of current working directory

## only directory given

show status of given directory

## -s or --snapshot [<target-directory>]

create snapshot of cwd or target, if given

## -r or --restore <snapshot-id>

restore given snapshot

## -m or --merge

merge with parent layer
