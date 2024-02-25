
this pretty not fun because some wrecked dependencies.


Need to install all dependencies and then compile and install yourself some libraries (palera1n doesnt document that).

Ubuntu 22.04:
```
sudo apt install -y build-essential pkg-config checkinstall git autoconf automake libtool-bin libreadline-dev libusb-1.0-0-dev gtk-doc-tools libkmod-dev
```

to build this libraries is pretty the same you just need to follow the next steps:
 
```
git clone http://github/{library}.git
cd {library}
./autogen.sh
make
sudo make install
```


After installing dependencies you should build this one first:
https://github.com/libimobiledevice/libplist.git


https://github.com/libimobiledevice/libusbmuxd.git

then:
https://github.com/libimobiledevice/libimobiledevice-glue.git

then:
https://github.com/libimobiledevice/libusbmuxd.git

then:
https://github.com/libimobiledevice/libirecovery.git

then:
https://github.com/libimobiledevice/libimobiledevice.git

then:
https://github.com/libimobiledevice/usbmuxd.git

finally:
https://github.com/palera1n/palera1n.git

so i got too many problems with compile that so i move to new script:

https://github.com/0rShemesh/palera1n/blob/main/deb_install.sh