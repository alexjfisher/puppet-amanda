# Changelog

## 2017-02-11 Release 2.1.0

This is the last release with Puppet3 support!
* Fix several markdown issues
* Add missing badges
* Set min version_requirement for Puppet + deps

## 2016-08-18 Release 2.0.0

  * First release in the Vox Pupuli namespace
  * Drop of ruby1.8.7 Support
  * Set type UNLISTED for amandaidx and amidxtape in xinetd
  * Correctly handle /tmp/amanda
  * Add option for manage_dle to server
  * Add option to enable ssh host key imports


## 2013-10-02 Release 1.0.2

Summary:

Revert set type unlisted in xinetd config

This change was not ready to be merged

Backwards-incompatible changes:
  - Set type unlisted in xinetd config


## 2013-10-02 Release 1.0.1

Summary:

Fix amanda::disklist::dle export bug

Bugs:

  - Fix amanda::disklist::dle export bug
  - Set proper ownership on disklist file
  - Set type unlisted in xinetd config


## 2013-09-29 Release 1.0.0

Summary:

Add disklist support for Amanda

Backwards-incompatible changes:

  - Changed dependency on ripienaar/concat to puppetlabs/concat
  - Added dependency on stdlib

## 2013-08-01 Release 0.1.7

  547a444 Update dependencies to use puppetlabs/xinetd
  18d3e8a Contributors list in readme now in list format.
  c1cb18c Made Readme nice looking for GitHub formatting
  755c742 add amanda_files which is similar to amanda_directories, it contains files that need to be chowned to the amanda user.
  6aad38c Add /opt/csw/var/amanda/gnutar-lists to list of directories to chown for Solaris

## 2013-05-19 Release 0.1.6

  c6074ab adding arch test to the amandad executable as well since the /usr/sbin/amandad symlink doesn't exist on CentOS 5
  b9eddba Set the correct location of the amanda binaries on CentOS and added an architecture check on it as well since the binaries are in different pl
  92c7906 (#6) Fix server package not defined on rhel


## 2013-03-19 Release 0.1.5

  e9c5e3c Merge pull request #4 from cdelston/master
  4cee13a Fix whitespace in 10fdface15c549430463
  10fdfac Ignore .svn directory when recursing remote config
  ac3d6b1 Add rhel6 support to amanda module
  37b3da1 Add redhat params and support

## 2012-05-19 Release 0.1.4

  * Update CHANGELOG for 0.1.4 patch
  bbaabd4 Use built-in file features for config define

## 2012-05-13 Release 0.1.3

  341a7dg Update CHeNGELOG for 0.1.3 patch
  a1230bf Add smoke test "demo", which includes a config
  1060449 Fix logic bug in amanda::config
  231a5e9 Add smoke tests


## 2012-05-12 Release 0.1.2

  cf93c7e Udate CHANGELOG for 0.1.2 patch
  4e3437a Fix style violations and README syntax
  8365d8b Fix bad default logic for configs_directory param


## 2012-05-11 Release 0.1.1

  4cf6223 Update CHANGELOG for 0.1.1 release
  cb217bf Update README file
  9c96e28 Clean up puppet-lint style errors


## 2012-05-09 Release 0.1.0

  6146b82 Update CHANGELOG for 0.1.0 release
  229ce32 Switch Debian params from zmanda packages to dist
  0883ee6 Massively refactor module, redo how configs work


## 2012-05-02 Release 0.0.3

  1daec40 Update CHANGELOG for 0.0.3 release
  9349442 Update xinetd resources (changed param name)
  e82cdbc Add version number of released concat module


## 2012-04-26 Release 0.0.2

  0001044 Reverting "version number as date"
  fffdec8 The log directory should be created on debian
  13402ed Update Modulefile for release to moduleforge
  9f4e5b2 Switch from blastwave provider to pkgutil
  e6335f6 Merge pull request #3 from deadpoint/master
  285a26f Add support for SuSE distributions
  cfe129e Fix dependency problem with xinetd client/server
  ebe6048 Merge pull request #2 from blkperl/test_blkperl_release2
  5c001f6 Fixing typo in LICENSE file
  44a275d Merge pull request #1 from blkperl/test_blkperl_release
  28b003f Adding an Apache LICENSE file and modulefile
  08f79bf Updating group params for freebsd < 8.2
  07f9117 Fixing amanda package "before" param
  f07500a Adding user dependency to file resources
  5067a01 Adding user shell definition
  9ae41b5 Tweaking config so concat works on solaris
  b160b6e Seperating out ssh_authorized_key into define
  2bd73f2 Adding a boolean xinetd parameter
  8e158df Fixing -auth tyop/bug
  49b819d Cleaning up the concact stuff in amanda module
  2086878 Adding concat management of .amandahosts
  2924c8e Adding amanda index xinetd entries


## 2011-12-15 Release 0.0.1

  40b896f Adding the amanda user on ubuntu to tape group
  6a8a494 Fixing $genericpackage bug
  6db6cdb README update, since it needed it
  1d549f5 Sanitizing defaults
  b9f5f40 Adding example configs
  4404d82 Simplifying amanda_config_files function
  919681b fixing array index bug
  486306d Bug fixes
  1f49e18 Use files/server/ as root instead of files/
  a8b96cf Updating README
  f341eb7 Updating readme
  fa085e9 diversifying amanda_config_files function
  fa1b634 modifying treatment of complexity in amanda module
  3126aa9 Adding amanda module from production to theverse
