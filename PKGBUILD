pkgname=bred-skel-default
_pkgname=bredos-cinnamon-theming
pkgver=1.1.0
pkgrel=0
pkgdesc="Pre user creation things for theming in BredOS"
arch=('any')
url="https://github.com/BredOS/bredos-cinnamon-theming"
license=('GPL-3.0-or-later')
source=("https://github.com/BredGang/bredos-cinnamon-theming/archive/refs/tags/v$pkgver.tar.gz")
md5sums=('SKIP')
depends=('mint-y-icons' 'mint-themes' 'glib2')
makedepends=('git')
package() {
    PREFIX=/etc/skel
    cd "$_pkgname-$pkgver"
    mkdir -p "${pkgdir}${PREFIX}/.config/"
    mkdir -p "${pkgdir}${PREFIX}/.config/dconf"
    mkdir -p "${pkgdir}${PREFIX}/.config/fish"
    cp -R "./user" "${pkgdir}${PREFIX}/.config/dconf/user"
    cp -R "./config.fish" "${pkgdir}${PREFIX}/.config/fish/config.fish"
}
