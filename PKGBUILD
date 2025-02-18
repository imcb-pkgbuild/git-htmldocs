# Maintainer: imcb <irismessage@protonmail.com>
# Contributor: Victoria Mitchell <victoria@quietmisdreavus.net>

pkgname='git-htmldocs'
pkgver='2.48.1'
pkgrel=1
pkgdesc='HTML documentation files for Git'
arch=('any')
url='https://git-scm.com/'
license=('GPL2')
groups=()
depends=('git')
makedepends=()
checkdepends=()
optdepends=()
source=("https://www.kernel.org/pub/software/scm/git/$pkgname-$pkgver.tar."{xz,sign})
sha256sums=('5450321b7de6702f9ec0a41108dfac3626afeb8fdd575b3d9a78febfaa96315c'
            'SKIP')
validpgpkeys=('96E07AF25771955980DAD10020D04E5A713660A7') # Junio C Hamano

package() {
    _dest="${pkgdir}/usr/share/doc/git-doc"
    install -Dm644 -t "${_dest}/" *.html
    install -Dm644 -t "${_dest}/howto" howto/*.html
    install -Dm644 -t "${_dest}/technical" technical/*.html
}
