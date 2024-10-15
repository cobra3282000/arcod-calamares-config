pkgname=arcod-calamares-config
_destname1="/etc"
pkgver=4.0.1
pkgrel=2
pkgdesc="Calamares Config"
arch=('any')
url="https://github.com/cobra3282000"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-net-config')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
