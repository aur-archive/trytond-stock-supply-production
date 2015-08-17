# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-stock-supply-production
_pkgname=trytond_stock_supply_production
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The stock_supply_production module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-product>=3.4' 'trytond-production>=3.4' 'trytond-stock>=3.4' 'trytond-stock-supply>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("daf71e25a10657638c0d1c8cdc821b8f")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}