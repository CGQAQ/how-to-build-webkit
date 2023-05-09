# how-to-build-webkit


## on ubuntu 22.04
1. clone the repo 
```console
git clone https://github.com/WebKit/WebKit.git
```
2. Install prerequisit deps
```shell
cd WebKit
Tools/gtk/install-dependencies

# optionally
Tools/Scripts/update-webkitgtk-libs

# build for debug
# Tools/Scripts/build-webkit --gtk --debug
```
3. build
```console
cmake -DPORT=GTK -DCMAKE_BUILD_TYPE=RelWithDebInfo -GNinja
ninja
```
for more go [https://github.com/WebKit/WebKit#building-the-gtk-port]
