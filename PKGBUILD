# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Sudip Datta <sudipdatta2002@gmail.com>
pkgname="freedownloadmanager"
pkgver=0.1.alpha
pkgrel=1
pkgdesc="free downlaod manager"
arch=("x86_64")
url="https://github.com/Github-2lu/fdm-arch"
license=("GPL3")
depends=('gtk3')
makedepends=("git")
source=("$pkgname.deb::$url/releases/download/v$pkgver/$pkgname.deb")
md5sums=("SKIP")

prepare(){
    unzstd $srcdir/data.tar.zst
    tar -xvf data.tar -C $srcdir
}

package() {
 	cp -r $srcdir/opt $srcdir/usr $pkgdir
}
