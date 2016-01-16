# $Id$
# Maintainer: BlackEagle <ike DOT devolder AT gmail DOT com>

pkgname=container-base
pkgver=5
pkgrel=1
pkgdesc="busybox linked base for containers"
arch=('any')
url="http://herecura.eu/"
license=('GPL')
depends=('busybox')
provides=('findutils' 'sed' 'grep' 'tar' 'lsof' 'wget' 'which' 'whois' 'traceroute' 'ed' 'dos2unix' 'cron' 'diffutils'
    'texinfo' # cheat
)
#provides=('acpid' 'binutils' 'net-tools' 'iputils' 'gawk' 'bridge-utils' 'e2fsprogs' 'kbd' 'ncurses' 'diffutils' 'cron' 'kmod' 'inetutils' 'dos2unix' 'ed' 'grep' 'fbset' 'psmisc' 'hdparm' 'i2c-tools' 'net-tools' 'ifenslave' 'ifplugd' 'findutils' 'procps-ng' 'iproute2' 'ipcalc' 'less' 'lsof' 'pciutils' 'usbutils' 'man-db' 'dosfstools' 'sysstat' 'dnsutils' 'patch' 'powertop' 'rfkill' 'rpmextract' 'run-parts' 'sed' 'smem' 'syslog-ng' 'tar' 'traceroute' 'unzip' 'sharutils' 'wget' 'which' 'whois'
#'runit' 'fatattr' 'fbsplash' 'microcom' 'sha3sum')

package() {
    install -dm755 "$pkgdir/usr/bin"

    # sh and bash
    #ln -s busybox "$pkgdir/usr/bin/sh"
    #printf "#!/bin/sh\n/bin/sh \"\$@\"" > "$pkgdir/usr/bin/bash"
    #chmod +x "$pkgdir/usr/bin/bash"

    # groupadd and useradd links
    #ln -s addgroup "$pkgdir/usr/bin/groupadd"
    #ln -s adduser "$pkgdir/usr/bin/useradd"
    #ln -s delgroup "$pkgdir/usr/bin/groupdel"
    #ln -s deluser "$pkgdir/usr/bin/userdel"

    # findutils
    ln -s busybox "$pkgdir/usr/bin/find" 
    ln -s busybox "$pkgdir/usr/bin/xargs" 

    # sed
    ln -s busybox "$pkgdir/usr/bin/sed"

    # grep
    ln -s busybox "$pkgdir/usr/bin/grep"
    ln -s busybox "$pkgdir/usr/bin/egrep"
    ln -s busybox "$pkgdir/usr/bin/fgrep"

    # tar
    ln -s busybox "$pkgdir/usr/bin/tar"

    # lsof
    ln -s busybox "$pkgdir/usr/bin/lsof"

    # wget
    ln -s busybox "$pkgdir/usr/bin/wget"

    # which
    ln -s busybox "$pkgdir/usr/bin/which"

    # whois
    ln -s busybox "$pkgdir/usr/bin/whois"

    # traceroute
    ln -s busybox "$pkgdir/usr/bin/traceroute"

    # procps-ng # missing slabtop, tload, vmstat, w
    ln -s busybox "$pkgdir/usr/bin/free"
    ln -s busybox "$pkgdir/usr/bin/pgrep"
    ln -s busybox "$pkgdir/usr/bin/pidof"
    ln -s busybox "$pkgdir/usr/bin/pkill"
    ln -s busybox "$pkgdir/usr/bin/pmap"
    ln -s busybox "$pkgdir/usr/bin/ps"
    ln -s busybox "$pkgdir/usr/bin/pwdx"
    ln -s busybox "$pkgdir/usr/bin/sysctl"
    ln -s busybox "$pkgdir/usr/bin/top"
    ln -s busybox "$pkgdir/usr/bin/uptime"
    ln -s busybox "$pkgdir/usr/bin/watch"

    # ed
    ln -s busybox "$pkgdir/usr/bin/ed"

    # dos2unix
    ln -s busybox "$pkgdir/usr/bin/dos2unix"
    ln -s busybox "$pkgdir/usr/bin/unix2dos"

    # cron
    ln -s busybox "$pkgdir/usr/bin/crond"
    ln -s busybox "$pkgdir/usr/bin/crontab"

    # diffutils
    ln -s busybox "$pkgdir/usr/bin/cmp"
    ln -s busybox "$pkgdir/usr/bin/diff"
}
