# Kickstart
Linux Installer Kickstart files

These are my Kicksart installers for automated installations of particular tasks.

I use these in my IPXE enviroment by chainloading a custom IPXE undionly.kpxe.
Though these Kickstarts should work on ISO installs or any other type of install with little modification.

The main nessisary modification is to change the root password hash you can do this with

	openssl passwd -1 “MyAwesomePassword”

The Installer Should be pretty universal.

Things to Note:
  * These Installs are Basicly core only installs unless specified otherwise.
  * There may be Issues or incompatabilitys with some setups.
  * This list will likely grow.
  * Due to an issue i was having with my openstack nodes networking i have added some networking templates to bond its two interfaces you can use them if you have 2 nics or comment them out.

The Goal here is to use these with my puppet learning to find new ways of auto provisioning in the cloud enviroment as well as simple ways of provisioning the infrastructure that drives the cloud.

Archlinux Kickstart.
This is essentialy just a bash script and can be run as ./archlinux-kickstart after you make it exacutable.
this can also be run by adding:

	script=http://example.com/archlinux-kickstart

to the kernel line in /boot/grub/grub.cfg or on the Grub command line from the boot image.

(Note i have not Tested this since the Deprication of AIF and am unsure if this method still works these days and am still testing this guy)
