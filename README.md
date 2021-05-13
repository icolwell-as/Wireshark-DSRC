# Wireshark-DSRC
**Wireshark custom build with DSRC (IEEE 802.11p, WSMP and 1609.2) support and SAE J2735 Dissector**

1. Wireshark 3.0.0 added support for WSMP and 1609.2 thanks to ETSI and Wireshark Devs
2. Included EU ITS support from ETSI
3. Supports the IEEE 1609.2, 1609.3-WSMP and SAE J2735-2016/2020 standards
4. IEEE 1609.3 and 1609.4 are not fully supported yet
5. Cellular is not supported
6. Wireshark builds have moved to Ubuntu 20.04
7. Now uses SAE J2735-2020
8. 64-bit only

**Releases**
1. v3.5.0-2020 Wireshark 3.5.0 with SAE J2735-2016
2. TBD

Builds are based on latest Wireshark development release, in this case 3.5.0.  Compiled and built for 64-bits only!

**Linux (Debian/Ubuntu) Packages**
1. dpkg -i *.deb
2. apt-get -f install

For DIY folks, the gory details for building Wireshark on Linux is here: https://www.wireshark.org/docs/wsdg_html_chunked/ChSrcBuildFirstTime.html#_building_on_unix

I had to build this on Ubuntu: https://github.com/BelledonneCommunications/bcg729, but I included the Debian packages in the Linux area.  This package is now included in Ubuntu 20.04.

**Windows Installer** (don't install over existing production release)
1. Run install.bat to combine split files and run installer

For DIY folks, the build for Windows is here: https://www.wireshark.org/docs/wsdg_html_chunked/ChSetupWin32.html

**Sources**
1. git clone https://code.wireshark.org/review/wireshark
2. The files under Sources go into the Wireshark root directory
3. Please diff the CMakeLists.txt files so that you don't break your build.

**Issues**
1. Does not dissect 3rd party add-on extensions to J2735

**I cannot release the ASN.1 file for SAE J2735 because it is copyrighted material!**
