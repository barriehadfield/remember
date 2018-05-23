# Setting up a new mac

## install homebrew
+ `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

## install gpg
+ `brew install gpg`

## install rvm
+ `gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB`
+ `\curl -sSL https://get.rvm.io | bash -s stable`

## install nvm
+ `brew install nvm`

## install npm
+ `brew install npm`

## install postgres
+ `brew install postgresql`
+ `brew services start postgresql`

### install redis
+ `brew install redis`
+ `brew services start redis`
