# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf.com>
pkgname=ramallahos-dotx-config
pkgver=1
pkgrel=1
pkgdesc="Xresources, xinitrc and xmodmap config for RamallahOS"
arch=('any')
url="https://github.com/ramallahos/$pkgname"
license=('GPL3')
depends=('starship')
makedepends=('coreutils')
source=("$pkgname::git+$url.git")
sha256sums=('SKIP')

package() {
    cd "$pkgname"
    install -d "${pkgdir}/etc/skel/.config/X11/"
    install -d "${pkgdir}/etc/skel/.Xresources.d"
    install -Dm 644 ".Xresources" "${pkgdir}/etc/skel/.Xresources"
    install -Dm 644 ".Xmodmap" "${pkgdir}/etc/skel/.Xmodmap"
    install -Dm 644 ".xinitrc" "${pkgdir}/etc/skel/.xinitrc"
    install -Dm 644 ".xprofile" "${pkgdir}/etc/skel/.xprofile"
    cp -rf ".Xresources.d" "${pkgdir}/etc/skel/

}
