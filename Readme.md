Libmacgpg-free
=========

Libmacgpg-free is a drop-in-replacement for [GPG Suite](https://gpgtools.org) Libmacgpg removing the paywall.


Build
-----

#### Clone the repository
```bash
git clone --recursive https://github.com/macgpg/libmacgpg-free
cd Libmacgpg-free
```

#### Build
```bash
make
```

#### Install
To replace the existing org.gpgtools.Libmacgpg:

```bash
sudo cp ./build/Release/org.gpgtools.Libmacgpg.xpc/Contents/MacOS/org.gpgtools.Libmacgpg /Library/Application\ Support/GPGTools/org.gpgtools.Libmacgpg.xpc/Contents/MacOS
```
