# Maintainer: spider-mario <spidermario@free.fr>
# Contributor: Zachary P. Landau <zlandau@jellofund.net>
pkgname=submux-dvd
pkgver=0.5.1
pkgrel=1
pkgdesc="A subtitle multiplexer for DVD .VOB files"
arch=('i686' 'x86_64')
url=ftp://sunsite.unc.edu/pub/linux/apps/video/
license=('GPL2')
source=(ftp://sunsite.unc.edu/pub/linux/apps/video/$pkgname-$pkgver.tgz)
noextract=()
md5sums=('95445a2b79737c83eb0ca38f22c8b7eb')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  install -D -m755 submux-dvd "$pkgdir/usr/bin/submux-dvd"
  install    -m755 vob2sub    "$pkgdir/usr/bin/"
}


# vim:set ts=2 sw=2 et:
