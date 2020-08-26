# Maintainer: JunYoung Gwak <aur@jgwak.com>
# Contributor: grimsock <lord.grimsock at gmail dot com>
# Contributor: James An <james@jamesan.ca>
# Contributor: lybin

pkgname=chromedriver
pkgver=85.0.4183.83
pkgrel=1
pkgdesc="Standalone server which implements WebDriver's wire protocol (for google-chrome)"
arch=('x86_64')
url="https://sites.google.com/a/chromium.org/chromedriver/"
license=('Apache')
conflicts=('chromium')
depends=('alsa-lib' 'gtk3' 'libcups' 'libxss' 'libxtst' 'nss' 'xdg-utils')
optdepends=('google-chrome')
md5sums=('c60433f136d588cb0534a68a7b5fc3c2')

source=("${pkgname}_${pkgver}_linux64.zip::https://chromedriver.storage.googleapis.com/${pkgver}/${pkgname}_linux64.zip")

package() {
  mkdir -p "$pkgdir/usr/bin/"
  install -D -m 755 "$srcdir/$pkgname" "$pkgdir/usr/bin/"
}
