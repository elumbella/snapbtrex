# Maintainer: Robert Goßmann <robert@gossmann.xyz>
pkgname=snapbtrex-python3-git
pkgver=0.1
pkgrel=1
pkgdesc="A python3 fork of yoshtec/snapbtrex"
arch=(any)
url="https://github.com/elumbella/$pkgname"
makedepends=(git)
depends=(python3 btrfs-progs)
source=("git+https://github.com/elumbella/snapbtrex")
md5sums=('SKIP')

package() {
	cd "snapbtrex"
	chmod +x snapbtrex.py
	sudo cp snapbtrex.py /usr/bin/snapbtrex
	sudo adduser snapbtr
	sudo cp 90_snapbtrsnd /etc/sudoers.d/
}

