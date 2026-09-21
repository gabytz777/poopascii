# Maintainer: gab <gab@example.com>

pkgname=poopascii
pkgver=1.0
pkgrel=1
pkgdesc="Print beautiful terminal ASCII art"
arch=('any')
url="https://aur.archlinux.org/poopascii"
license=('MIT')
source=('poop' 'poop.txt' 'LICENSE')
sha256sums=('5af288c7cbd2fe0148e7ad147ff903b7e0d3c4aa993f08e07965202963a83c6b'
            '3fd2e3a6359486fa883faf06ba6675dcfbeaea01e359d6a68daef2408ccc861f'
            'c4401fdd8e3a1113ad7f1059ba2d3743a5b5ada25ba2dac9f85320d2e821e877')

package() {
    install -Dm755 "$srcdir/poop" "$pkgdir/usr/bin/poopascii"
    install -Dm644 "$srcdir/poop.txt" "$pkgdir/usr/share/poopascii/poop.txt"
    install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
