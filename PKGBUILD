# Maintainer: pineappletoad

pkgname=open-cad-studio-bin
pkgver=2026.37
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
sha256sums=('3b676cabc7660b1a3640a4fe7a8b5a31d8be2d9e6d16fc684836dc3e51616dbc')

package() {
    bsdtar -xf "${srcdir}/open-cad-studio-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
