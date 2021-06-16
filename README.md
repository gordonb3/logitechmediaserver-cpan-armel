> #### Deprecation notice
> Logitechmediaserver 7.8.0 is pretty old now and I have upgraded to version 8.x quite some time ago. With Perl 5.32 having been marked as stable by Gentoo it is time to archive this repository as I'm no longer able to verify that it runs correctly with newly built modules after Perl 5.30.

---

# logitechmediaserver-cpan-armel

#### Description
This project contains a complete CPAN folder for logitechmediaserver 7.8.0 on armv5te with Perl 5.20 and later.


#### Installation
Download logitechmediaserver-7.8.0-noCPAN.tgz from [downloads.slimdevices.com](http://downloads.slimdevices.com/LogitechMediaServer_v7.8.0/) and unpack it in your work folder.

Unpack the master zip from this project and copy these folders over to your work folder, overwriting every file that may exist:
 - Bin
 - CPAN
 - Slim

Reference the `Tarball Notes` in Installation.txt in the work folder on how to run your copy of Logitech Media Server.


#### Special Perl 5.24 note
CPAN/arch contains two versions of architecture dependent modules for Perl 5.24.x. The second version, `5.24-pie`, was compiled with `-fPIE` for position independent execution and it is advised that you use that version if the rest of your system was compiled the same way (like in Gentoo profile 17). This requires you to swap the folder with the non-PIE `5.24` folder.

It is safe to delete any unused versions from the `arch` folder.


#### Gentoo installation
If you haven't already, use layman to add the [bubba overlay](https://github.com/gordonb3/bubba-overlay) to your system and emerge logitechmediaserver-bin
