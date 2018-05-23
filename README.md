# stuff to remember

## install homebrew
+ `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

## install gpg
+ `brew install gpg`

## mount drive

+ Edit `/etc/auto_master` 
+ and add  `/nas          auto_nas`
+ then create auto_nas file and add
+ `music    storage.local:/nfs/music`
+ then `sudo automount -vc`

