# Maintainer: felipe.facundes
# Contributor: Felipe Facundes
# Based on mixxx PKGBUILD by felipe.facundes

pkgname=mixxxold
pkgver=1.10
pkgrel=2
pkgdesc="Old mixxx DJ for gpu chipset i915."
arch=('i686')
depends=('portmidi' 'protobuf' 'vamp-plugin-sdk' 'fftw' 'libid3tag' 'libmad' 'libogg' 'libshout' 'libsndfile' 'portaudio' 'taglib' 'qtwebkit' 'libusbx')
makedepends=('mesa' 'libshout' 'glu')
optdepends=('java-runtime: for using pmdefaults')
conflicts=('mixxx' 'mixxx-git')
url="https://sites.google.com/site/felipefacundes/"
license=('GPL')
source=(
https://dl.dropboxusercontent.com/s/6o0l120h2n4si06/mixxxold.tar.gz)

build()
{
 cd "$srcdir"
 install -d "${pkgdir}/"
 cp -rf "usr" "${pkgdir}/" || return 1
 echo run command: ln -s /usr/lib/libshout.so /usr/lib/libshout2.so.3
}

sha512sums=('831fcee6316c20d2aafe90320ba0a160714c26ed5ecb66f266317a52df5e3f3a3177f2e6508c5e4d85ae3552dd45686143a98d6fa131c574fdf66cae36632b44')
