mira_installer
==============

This shall install all required MIRA packages


## create debian using fpm

First run `./mira-installer-binary.sh ubuntu-1804lts-x64`

Then:

```
fpm -m "marc@hanheide.net" -n mira-scitos -t deb -v 0.21.2~bionic -s dir -d libboost-all-dev -d libogre-1.9-dev -d libqwt5-qt4 -d libsqlite3-dev -d libssl-dev -d libxml2-dev -d libxrandr-dev -d pyqt4-dev-tools -d libopencv-dev -d libsvn-dev /opt/mira-release
```