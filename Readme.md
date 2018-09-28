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
* Install the [GPG Suite](https://gpgtools.org).
* Build this library or [download it](https://github.com/macgpg/libmacgpg-free/releases).
* Make sure the version of your downloaded GPGTools match the version of this library (see [releases](https://github.com/macgpg/libmacgpg-free/releases))
* To replace the existing org.gpgtools.Libmacgpg:

```bash
sudo cp ./build/Release/org.gpgtools.Libmacgpg.xpc/Contents/MacOS/org.gpgtools.Libmacgpg /Library/Application\ Support/GPGTools/org.gpgtools.Libmacgpg.xpc/Contents/MacOS
```
