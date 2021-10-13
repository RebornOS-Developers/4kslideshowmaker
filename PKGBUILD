# Maintainer: Rafael <rafael@rebornos.org>
# 2.0.0.1054

pkgname=4kslideshowmaker
pkgver=2.0.0
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('00094cd161f296b20e7db9cc07ce584203b4db93478a392cf110949f2ba91ae9c0599f5d3e1f79c41764c19770ca589e19ecab23b255ac70c4c26a2c034f718a')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

