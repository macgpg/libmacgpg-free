Libmacgpg-free
=========

Libmacgpg-free is a drop-in-replacement for [GPG Suite](https://gpgtools.org) Libmacgpg removing the paywall.

Tested with GPG-Suite **2019.1**, 2018.5 and 2018.4

Build
-----

#### Clone the repository
```bash
git clone --recursive https://github.com/macgpg/libmacgpg-free
cd Libmacgpg-free
```

#### Build (newest version 2019.1)
```bash
make
```
*Checkout an older tag if you wish to build for older versions*

#### Install
* Install the [GPG Suite](https://gpgtools.org).
* Build this library or [download it](https://github.com/macgpg/libmacgpg-free/releases).
* Make sure the version of your downloaded GPGTools match the version of this library (see [releases](https://github.com/macgpg/libmacgpg-free/releases))
* To replace the existing org.gpgtools.Libmacgpg:

```bash
sudo cp ./build/Release/org.gpgtools.Libmacgpg.xpc/Contents/MacOS/org.gpgtools.Libmacgpg /Library/Application\ Support/GPGTools/org.gpgtools.Libmacgpg.xpc/Contents/MacOS
sudo chmod 755 /Library/Application\ Support/GPGTools/org.gpgtools.Libmacgpg.xpc/Contents/MacOS/org.gpgtools.Libmacgpg
```

Restart your computer or at least restart the XPC `org.gpgtools.Libmacgpg.xpc`:
```bash
sudo launchctl stop org.gpgtools.Libmacgpg.xpc
sudo launchctl start org.gpgtools.Libmacgpg.xpc
```

...or eventully kill the org.gpgtools.Libmacgpg.xpc process.
