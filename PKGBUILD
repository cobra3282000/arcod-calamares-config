# Maintainer: Erik Dubois <erik.dubois@gmail.com>
pkgname=arcod-calamares-config
_pkgname=arcod-calamares-config
_destname="/etc/calamares"
_licensedir="/usr/share/arcolinux/licenses/"
pkgver=1.0
pkgrel=1
pkgdesc="calamares config for arcopro"
arch=('any')
url="https://github.com/cobra3282000/${_pkgname}"
license=('GPL3')
makedepends=('git')
depends=()
# conflicts=('arcoplasma-calamares-config' 'arconet-calamares-config')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+$url")
sha256sums=('SKIP')
# install='readme.install'
package() {
    mkdir -p "${pkgdir}${_licensedir}${_pkgname}"
    mv "${srcdir}/${_pkgname}/"LICENSE "${pkgdir}${_licensedir}${_pkgname}/LICENSE"
    mkdir -p "${pkgdir}${_destname}"
    cp -r "${srcdir}/${_pkgname}/calamares/"* "${pkgdir}${_destname}"
}
