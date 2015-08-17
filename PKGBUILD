pkgname=otf-goudy
pkgver=3.1
pkgrel=3
pkgdesc="MIT licensed opentype fonts based on Goudy Old Style (Sorts Mill Goudy)"
arch=('any')
url="https://bitbucket.org/sortsmill/sortsmill-fonts"
license=('MIT')
depends=('fontconfig' 'xorg-font-utils')
makedepends=('unzip')
source=(https://bitbucket.org/sortsmill/sortsmill-fonts/downloads/goudy-3.1.zip)
noextract=(goudy-3.1.zip)
install=$pkgname.install
md5sums=('d33eb55056c9cd51eed04254eccf2ca9')

package() {
  cd $srcdir/
  unzip goudy-3.1.zip GoudyStM-Italic.otf GoudyStM.otf
  mkdir -p $pkgdir/usr/share/fonts/OTF
  cp *.otf $pkgdir/usr/share/fonts/OTF
}

