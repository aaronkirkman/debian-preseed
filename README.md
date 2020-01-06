Scripts for configuring [preseed files](https://wiki.debian.org/DebianInstaller/Preseed) for Debian Linux and incorporating `preseed.cfg` into a Debian iso image as part of initrd.
As of this commit, these instructions are for Debian 10 ("buster").
See [Appendix B: Automating the installation using preseeding](https://www.debian.org/releases/buster/amd64/apb.en.html) for more details.

Available configurations:

- [default/preseed.cfg](default/preseed.cfg)
   - Default configuration that uses `https` for `/etc/apt/sources.list` and installs Git

- [mediawiki/preseed.cfg](mediawiki/preseed.cfg)
   - Includes default configuration and also installs necessary packages for a [SQLite-based Mediawiki](https://www.mediawiki.org/wiki/Manual:SQLite) installation
