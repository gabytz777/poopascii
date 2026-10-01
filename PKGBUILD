# Maintainer: gab <gab@example.com>

pkgname=poopascii
pkgver=1.1
pkgrel=1
pkgdesc="Print beautiful terminal ASCII art"
arch=('any')
url="https://aur.archlinux.org/poopascii"
license=('MIT')
source=('poopascii' 'CREDITS' 'LICENSE')
sha256sums=('4470b50a42db76fb011ea5dced03298b05e5be97dab15e6d6e5e8dd57475fca1'
            'a08e9e8544179c6fe9099c82183a2b2ddc6559569cae659da37d2d96e37883d5'
            '32a59621f5e074dbca32c3300c93ae9e49f243da39b1986f645a59d4c0c89352')

package() {
    install -Dm755 "$srcdir/poopascii" "$pkgdir/usr/bin/poopascii"

    # art/ is not a VCS checkout, so makepkg never populates $srcdir/art.
    # Install straight from the package tree instead. See CREDITS for the
    # origin of the individual pieces.
    install -d "$pkgdir/usr/share/poopascii/art"
    install -m644 "$startdir"/art/*.txt "$pkgdir/usr/share/poopascii/art/"

    install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 "$srcdir/CREDITS" "$pkgdir/usr/share/licenses/$pkgname/CREDITS"
}
