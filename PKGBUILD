# Maintainer: Rafael <rafael@rebornos.org>
# v1.8.2.1041

pkgname=4kslideshowmaker
pkgver=1.8.2
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('d2d073523661a5009e93d7a86537e5539bb533c4429862897bfc15571e42fa2bc7b16f7fe0fda8193bb9905762130d7b0fa14562be5fa013217d3723323ddd3e')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

