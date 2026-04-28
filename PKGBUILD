# Maintainer: imcb <irismessage@protonmail.com>
# Contributor: Victoria Mitchell <victoria@quietmisdreavus.net>

pkgname='git-htmldocs'
pkgver=2.54.0
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
sha256sums=('7ff72bfdfed4f20563f34416cf27614fb9c35bfad590db0062f2a0a9636514e4'
            'SKIP')
validpgpkeys=('96E07AF25771955980DAD10020D04E5A713660A7') # Junio C Hamano

package() {
    _dest="${pkgdir}/usr/share/doc/git-doc"
    install -Dm644 -t "${_dest}/" *.html
    install -Dm644 -t "${_dest}/howto" howto/*.html
    install -Dm644 -t "${_dest}/technical" technical/*.html
}
