pkgname=holoiso-install-script
pkgver="snapshot$(date +%Y%m%d.%H%M)"
pkgdesc="HoloISO installer scripts"
pkgrel="1"
depends=('arch-install-scripts')
arch=("x86_64")

package() {
    mkdir -p "${pkgdir}/usr/bin"
    cp "${srcdir}/holoinstall" "${pkgdir}/usr/bin/holoinstall"
    cp "${srcdir}/holoiso-chroot" "${pkgdir}/usr/bin/holoiso-chroot"
    chmod +x "${pkgdir}/usr/bin/holoinstall"
    chmod +x "${pkgdir}/usr/bin/holoiso-chroot"
}
