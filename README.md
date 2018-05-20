# db stuff to store

## mount drive

Edit `/etc/auto_master` 
and add  `/nas          auto_nas`
then create auto_nas file and add
`music    storage.local:/nfs/music`
then `sudo automount -vc`

