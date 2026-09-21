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
            '32a59621f5e074dbca32c3300c93ae9e49f243da39b1986f645a59d4c0c89352')

package() {
    install -Dm755 "$srcdir/poop" "$pkgdir/usr/bin/poopascii"
    install -Dm644 "$srcdir/poop.txt" "$pkgdir/usr/share/poopascii/poop.txt"
    install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
