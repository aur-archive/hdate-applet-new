# Maintainer: Assaf Sapir <meijin07 AT gmail.com>
# Contributor: Jack <nim901@gmail.com>
pkgname=hdate-applet-new
libname=hdate-applet
pkgver=0.15.11
pkgrel=1
arch=('i686' 'x86_64')
license=('GPL')
provides=('hdate-applet')
conflict=('hdate-applet')
pkgdesc="Is an applet to show the hebrew date (calendar) using the libhdate library and the gnome-2.0 graphics library"
depends=('gtk2' 'libhdate-ik' 'gnome-panel-bonobo')
optdepends=('python: for python bynding')
url="http://hdateapplet.sourceforge.net/"
source=(http://downloads.sourceforge.net/sourceforge/hdateapplet/hdateapplet/$libname-$pkgver.tar.bz2)
md5sums=(8cfda134941b4d656df30d45e8fccf4e)

build() {
cd $srcdir/$libname-$pkgver
./configure --prefix=/usr
make
make DESTDIR=$pkgdir install
}
