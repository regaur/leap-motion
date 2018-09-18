# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='leap-motion'
pkgver=1.0
pkgrel=1
pkgdesc='Add auto-login and local-admin to plugdev group, configure leapd'
packager='Jan Boelsche'
arch=('any')
license=('GPL')
groups=()
depends=(
  'leap-motion-driver'
  'leap-motion-sdk'
)
makedepends=()
checkdepends=()
optdepends=()
install=${pkgname}.install

source=(
  'config.json'
)

sha256sums=('1a283396cd260626b94dd8f7449e45839cdb3c8db5df28e652d418c33c91d899')

package() {
  install -Dm 644 -t "${pkgdir}/var/.Leap Motion" config.json
}

