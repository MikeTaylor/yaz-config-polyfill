# yaz-config-polyfill

Polyfill for the `yaz-config` script on pkg-config-based systems that omit it

For some reason, the religious convictions of the Debian package maintainer for YAZ have resulted in [`yaz-config`](https://software.indexdata.com/yaz/doc/yaz-config.html) being removed from the package, which means that it is no longer possible to build Perl packages such as [`Net::Z3950::ZOOM`](https://metacpan.org/pod/Net::Z3950::ZOOM) that rely on this script. For those of us who have to actually get work done, here is simple polyfill that reimplements `yaz-config` in terms of the `pkg-config` script that Debian prefers.

