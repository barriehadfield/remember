# Setting up a new mac

## Nas automount
+ In `/etc/auto_master` add `/mnt    auto_mnt`
+ Then create `auto_mnt` and add `music     10.0.1.35:/c/music`
+ `sudo automount -vc`

## bash profile prompt (~/.bash_profile)
+ `export PS1="\w "`

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

## install redis
+ `brew install redis`
+ `brew services start redis`

## install java 8
+ `brew install caskroom/versions/java8`

## install neo4j (in app folder)
+ `rake neo4j:install[community-latest,development]`
+ `rake neo4j:install[community-latest,test]`
+ `rake neo4j:config[test,7475]`

## install bundler
`gem install bundler`

## install yarn
+ `brew install yarn`

# Working with Neo4j

## Start Neo4j
+ `rake neo4j:start[development]`
+ `rake neo4j:start[test]`

## Migrate Ne04j
+ `rake neo4j:migrate` to migrate development
+ `RAILS_ENV=test rake neo4j:migrate:all` to migrate test

## Reset the Neo4j database
+ `rake neo4j:reset_yes_i_am_sure[development]`
+ `rake neo4j:reset_yes_i_am_sure[test]`

