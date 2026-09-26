pkgname=workfolio
pkgver=0.1.54
pkgrel=1
pkgdesc="Workfolio desktop application"
arch=('x86_64')
url="https://www.getworkfolio.com/"
license=('custom')

options=('!strip' '!debug')

depends=(
  'gtk3'
  'libx11'
  'libxcb'
)

source=("https://workfolio-public.s3.ap-south-1.amazonaws.com/Workfolio+Setup.deb")
sha256sums=('SKIP')

package() {
  bsdtar -xf "$srcdir/Workfolio+Setup.deb" \
    -C "$srcdir"

  bsdtar -xf "$srcdir/data.tar.xz" \
    -C "$pkgdir"

  install -d "$pkgdir/usr/bin"
  ln -s /opt/Workfolio/workfolio "$pkgdir/usr/bin/workfolio"
}
