Chef Workstation
==================================

Chef Workstation installs everything you need to get started using Chef on Windows, Mac and Linux; and is currently focused around performing ad-hoc tasks on your server.

## Getting Started

1. Download Chef Workstation

   * [Download Chef Workstation for Mac](http://artifactory.chef.co/omnibus-current-local/com/getchef/chef-workstation/0.1.99/mac_os_x/10.13/chef-workstation-0.1.99-1.dmg)

   * [Download Chef Workstation for Windows](http://artifactory.chef.co/omnibus-current-local/com/getchef/chef-workstation/0.1.99/windows/2016/chef-workstation-0.1.99-1-x64.msi)

   * [Download Chef Workstation for Debian](http://artifactory.chef.co/omnibus-current-local/com/getchef/chef-workstation/0.1.99/ubuntu/16.04/chef-workstation_0.1.99-1_amd64.deb)

   * [Download Chef Workstation for Enterprise Linux](http://artifactory.chef.co/omnibus-current-local/com/getchef/chef-workstation/0.1.99/el/7/chef-workstation-0.1.99-1.el6.x86_64.rpm)

    ***Note:*** These links are internal and require Chef VPN.

2. Double-click the `.dmg` or `.msi` file to start the install process. Or install
   the Linux package for your platform.

3. Open a command-line terminal, and try out some chef-cli commands

   * Run `chef -h` to view the available commands

   * Want to perform an ad-hoc task? Try

    `chef target converge <Target host|IP|SSH|WinRM> <Resource> <Resource Name> [properties] [flags]`

    `chef target converge user@hostname user timmy`

    `chef target converge winrm://user@hostname:port user timmy`


## Building Chef-Workstation Packages
We use Omnibus to describe our packaging. Please review [chef-workstation/omnibus/README.MD](https://github.com/chef/chef-workstation/tree/master/omnibus) for further details.

## Questions or concerns?
Please join us in the *#chef-workstation* channel on Slack!

## Copyright and License
Copyright 2008-2018, Chef Software, Inc.

**Note:** We are currently not open source. The plan is to make Chef Workstation open source at some point in the future.
