# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='leap-motion'
pkgver=1.1
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
  'leapd.service'
)

sha256sums=('9e8077591c058f5564d40a4e4cdb8cdc0dbc62cf473bafcb2bb3b58cb1ab0a9e'
            '949fe9e0e65366a80cb4e22676e96e3886090db9486f9444cdfdc7da9ff9a385')

package() {
  install -Dm 644 -t "${pkgdir}/var/.Leap Motion" config.json
  install -Dm 644 -t "${pkgdir}/var/.Leap Motion" leapd.service
}

