# Maintainer: Damjan Georgievski <gdamjan@gmail.com>
pkgname=systemd-suspend-modules
pkgver=1.0
pkgrel=2
pkgdesc="Reload modules on suspend/hibernate with systemd"
arch=('any')
url="https://aur.archlinux.org/packages/systemd-suspend-modules/"
license=('GPL')
depends=('systemd')
backup=('etc/suspend-modules.conf')
source=("suspend-modules")

package() {
    # Install files
    install -Dm755 "${srcdir}/suspend-modules" "${pkgdir}/usr/lib/systemd/system-sleep/suspend-modules"
    mkdir ${pkgdir}/etc/
    touch ${pkgdir}/etc/suspend-modules.conf
}
md5sums=('464a8347df5c492d48815145af1a3ee3')
