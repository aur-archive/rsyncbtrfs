# Maintainer: Adrien Ferrand <h 4 d r i e n @ g m a i l . c o m>

pkgname=rsyncbtrfs
pkgver=1.0.3
pkgrel=1
pkgdesc="Simple incremental backup tool which uses the incremental snapshot capability of Btrfs subvolumes."

arch=('any')
url="http://github.com/fullm3tal/rsyncbtrfs"

license=('GPL')
depends=('python' 'btrfs-progs' 'rsync')
makedepends=('git')
provides=('rsyncbtrfs')
md5sums=('SKIP')

source=('rsyncbtrfs::git+http://github.com/fullm3tal/rsyncbtrfs')

build() {
	cd ${srcdir}
}

package(){
	cd "$srcdir/$pkgname"

	install -D -m755 rsyncbtrfs ${pkgdir}/usr/bin/rsyncbtrfs || return 1
	install -D -m644 COPYING ${pkgdir}/usr/share/licenses/rsyncbtrfs/COPYING
}
