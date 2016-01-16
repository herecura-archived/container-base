# $Id$
# Maintainer: BlackEagle <ike DOT devolder AT gmail DOT com>

pkgname=container-base
pkgver=1
pkgrel=1
pkgdesc="busybox linked base for containers"
arch=('any')
url="http://herecura.eu/"
license=('GPL')
depends=('busybox')
provides=('sh' 'bash' 'acpid' 'shadow' 'binutils' 'net-tools' 'iputils' 'gawk' 'coreutils' 'util-linux' 'bootchart' 'bridge-utils' 'bzip2' 'e2fsprogs' 'kbd' 'ncurses' 'diffutils' 'cpio' 'cron' 'kmod' 'inetutils' 'dos2unix' 'ed' 'grep' 'fbset' 'psmisc' 'gzip' 'hdparm' 'i2c-tools' 'net-tools' 'ifenslave' 'ifplugd' 'findutils' 'procps-ng' 'iproute2' 'ipcalc' 'less' 'lsof' 'pciutils' 'usbutils' 'xz' 'man-db' 'dosfstools' 'sysstat' 'dnsutils' 'patch' 'powertop' 'rfkill' 'rpmextract' 'run-parts' 'sed' 'smem' 'syslog-ng' 'tar' 'traceroute' 'unzip' 'sharutils' 'wget' 'which' 'whois'
'runit' 'fatattr' 'fbsplash' 'microcom' 'sha3sum')

package() {
    install -dm755 "$pkgdir/usr/bin"

    # sh and bash
    ln -s busybox "$pkgdir/usr/bin/sh"
    printf "#!/bin/sh\n/bin/sh \"\$@\"" > "$pkgdir/usr/bin/bash"
    chmod +x "$pkgdir/usr/bin/bash"

    # groupadd and useradd links
    ln -s addgroup "$pkgdir/usr/bin/groupadd"
    ln -s adduser "$pkgdir/usr/bin/useradd"
    ln -s delgroup "$pkgdir/usr/bin/groupdel"
    ln -s deluser "$pkgdir/usr/bin/userdel"
}
