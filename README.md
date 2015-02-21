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
  * THis list will likely grow.

The Goal here is to use these with my puppet learning to find new ways of auto provisioning in the cloud enviroment as well as simple ways of provisioning the infrastructure that drives the cloud.
