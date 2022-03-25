## Collectl, w/ Lustre

This repo contains the required bits to build a [`collectl`][collectl] RPM
including [Peter Piela's Lustre plugin][lustre-plugin] (and supports Lustre
2.12).

### Build

```
# yum install rpm-build rpmdevtools yum-utils
# rpmdev-setuptree
# spectool -g -R collectl.spec
# cp -R SPECS SOURCES ~/rpmbuild/
# rpmbuild -ba SPECS/collectl.spec
```


[collectl]:      https://collectl.sf.net
[lustre-plugin]: https://github.com/pcpiela/collectl-lustre

