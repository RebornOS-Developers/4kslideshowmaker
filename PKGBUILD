# Maintainer: Rafael <rafael@rebornos.org>
# v2.0.1.1055

pkgname=4kslideshowmaker
pkgver=2.0.1
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('fd249d3934eac8490ac287d4a52c3d453966283e295d419b2ee6db3dd788269a5033ef4d64b9902b538d4abd6ff091182b94e3f6243c5ce72c82b68cb1c49382')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

