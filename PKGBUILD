# Maintainer: imcb <irismessage@protonmail.com>
# Contributor: Victoria Mitchell <victoria@quietmisdreavus.net>

pkgname='git-htmldocs'
pkgver=2.55.0
pkgrel=1
pkgdesc='HTML documentation files for Git'
arch=('any')
url='https://git-scm.com/'
license=('GPL-2.0-only')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
source=("https://www.kernel.org/pub/software/scm/git/$pkgname-$pkgver.tar."{xz,sign})
sha256sums=('d1142c4e28b469d297d6df6519653e92a76c952f55202fde17a72a3b03d49437'
            'SKIP')
validpgpkeys=('96E07AF25771955980DAD10020D04E5A713660A7') # Junio C Hamano

package() {
    _dest="${pkgdir}/usr/share/doc/git-doc"
    install -Dm644 -t "${_dest}/" *.html
    install -Dm644 -t "${_dest}/howto" howto/*.html
    install -Dm644 -t "${_dest}/technical" technical/*.html
}
