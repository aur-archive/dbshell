# Maintainer: Edgar Kalkowski <eMail@edgar-kalkowski.de>
pkgname=dbshell
pkgver=0.1.1
pkgrel=1
epoch=
pkgdesc="Database CLI for PostgreSQL and Virtuoso"
arch=('i686' 'x86_64')
url="https://github.com/ErkiDerLoony/dbshell"
license=('GPL')
groups=()
depends=('postgresql-libs' 'readline' 'libiodbc')
makedepends=('postgresql' 'cmake')
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(https://github.com/ErkiDerLoony/dbshell/archive/$pkgver.tar.gz)
noextract=()

build() {
  cd "$srcdir/$pkgname-$pkgver"
  mkdir -p build
  cd build
  cmake -DCMAKE_INSTALL_PREFIX="$pkgdir/" ..
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver/build"
  make install
}
md5sums=('9491b5cf54a77629462a69fd5cf1aca1')
