# Maintainer: pineappletoad

pkgname=open-cad-studio-bin
pkgver=2026.38
_pkgrel_src=1
pkgrel=1
pkgdesc="A CAD application built with Rust — 2D/3D drawing, DWG/DXF support, and GPU-accelerated rendering (precompiled)"
arch=('x86_64')
url="https://github.com/HakanSeven12/OpenCADStudio"
license=('GPL-3.0-only')
options=('!debug')
provides=('open-cad-studio')
conflicts=('open-cad-studio')
depends=(
    'xdg-desktop-portal'
    'glibc'
    'libgcc'
    'wayland'
)

source=("https://github.com/tubbywrestler/open-cad-studio-bin/releases/download/${pkgver}-${_pkgrel_src}/open-cad-studio-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst")
sha256sums=('ba888482d09b59ab1d0676f602552ec16442a80a2b5c21e84adb53191c54b6cc')

package() {
    bsdtar -xf "${srcdir}/open-cad-studio-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
