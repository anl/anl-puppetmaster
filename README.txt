puppetmaster

A puppet module to bootstrap a puppetmaster; written to be run from
"puppet apply".

Example usage:

> puppet module install cprice404-inifile
> git clone https://github.com/anl/anl-puppetmaster.git
> mv anl-puppetmaster ~/.puppet/modules/puppetmaster
> sudo puppet apply --modulepath=~/.puppet/modules -e "include puppetmaster"

or 

> sudo puppet apply --modulepath=~/.puppet/modules -e "class { puppetmaster: hiera_gpg => true }"
