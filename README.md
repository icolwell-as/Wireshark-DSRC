# Wireshark-DSRC
**Wireshark custom build with DSRC (IEEE 802.11p, WSMP and 1609.2) support and SAE J2735 Dissector**

1. Wireshark 3.0.0 added support for WSMP and 1609.2
2. Including EU ETSI ITS support.
3. IEEE 1609.3 and 1609.4 are not supported yet.

Builds are based on latest Wireshark development release, in this case 3.1.0.  Compiled and built for 64-bits only!

**Linux (Debian/Ubuntu) Packages**
1. dpkg -i *.deb
2. apt-get -f install

**Windows Installer** (don't install over existing production release)
1. Run install.bat to combine split files and run installer

**I cannot release additional sources as the ASN.1 for SAE J2735 is copyrighted material!**
