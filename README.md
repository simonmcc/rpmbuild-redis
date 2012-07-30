# rpmbuild-redis
**Simple rpmdev setup for building redis RPMs**

Original spec file from Redis EPEL RPM (http://rpmfind.net//linux/RPM/epel/5/x86_64/redis-2.4.10-1.el5.x86_64.html)

RPM dev setup from http://fedoraproject.org/wiki/A_Short_RPM_Tutorial

One off tool setup
```shell
# yum install @development-tools
# yum install fedora-packager
# usermod -a -G mock <your username>
```

Building RPM as non-root
```shell
$ rpmbuild -ba SPECS/redis.spec
```
