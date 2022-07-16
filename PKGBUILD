pkgname=holoiso-install-script
pkgver="snapshot$(date +%Y%m%d.%H%M)"
pkgdesc="HoloISO installer scripts"
pkgrel="1"
depends=('arch-install-scripts')
arch=("x86_64")

package() {
    mkdir -p "${pkgdir}/usr/bin"
    mkdir -p "${pkgdir}/etc/skel/Desktop"
    cp "${srcdir}/holoinstall" "${pkgdir}/usr/bin/holoinstall"
    cp "${srcdir}/desktopicons/holoiso-chroot.desktop" "${pkgdir}/etc/skel/Desktop/holoiso-chroot.desktop"
    cp "${srcdir}/desktopicons/holoiso-install.desktop" "${pkgdir}/etc/skel/Desktop/holoiso-install.desktop"
    cp "${srcdir}/holoiso-chroot" "${pkgdir}/usr/bin/holoiso-chroot"
    chmod +x "${pkgdir}/usr/bin/holoinstall"
    chmod +x "${pkgdir}/etc/skel/Desktop/holoiso-chroot.desktop"
    chmod +x "${pkgdir}/etc/skel/Desktop/holoiso-install.desktop"
    chmod +x "${pkgdir}/usr/bin/holoiso-chroot"
}