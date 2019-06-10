# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='leap-motion'
pkgver=1.2
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
            'c63904945e2a6b97b021034030d085df49a9214d4d9565548887396db7e58907')

package() {
  install -Dm 644 -t "${pkgdir}/var/.Leap Motion" config.json
  install -Dm 644 -t "${pkgdir}/var/.Leap Motion" leapd.service
}

