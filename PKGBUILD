# Contributor: damir <damir@archlinux.org>

pkgname=biogrep
pkgver=1.0
pkgrel=2
pkgdesc="match large sets of patterns against biosequence databases"
arch=(i686 x86_64)
license=('GPL')
url="http://web.mit.edu/bamel/biogrep.shtml"
depends=('glibc')
source=(http://web.mit.edu/bamel/biogrep-$pkgver.tar.gz)
md5sums=('90fb4987301b4c84f16e36e82c679e16')

build() {
  cd $srcdir/$pkgname-$pkgver
  ./configure --prefix=/usr || return 1
  make || return 1
  make DESTDIR=$pkgdir install || return 1
}
