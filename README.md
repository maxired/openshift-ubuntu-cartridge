#Openshift-ubuntu-cartridge

This (DIY) cartridge allow to run a Ubuntu (12.04) inside a Gears.

This is done with proot.
Thanks to the '-0' option of proot (similar to fakeroot), the Ubuntu behave just as if you were root.
This mean that you can install package with 'apt-get' and so more.

https://github.com/maxired/openshift-ubuntu-cartridge

#Installation
After the first push, everything should be ready.
After this , you can connect to the gears and go inside your container

```
cd diy;
./proot-x86_64 -r ubuntu -0 -b /dev -b /etc/resolv.conf -b /proc bash
```
