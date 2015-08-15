# Maintainer: Lucas Tanure <tanure@linux.com>

pkgname=gcc-linaro-aarch64-linux-gnu
_relver=4.9
_reldate=2014.09
_relverdate=${_relver}-${_reldate}
pkgver=${_relver}_${_reldate}
pkgrel=4
pkgdesc="Linux binaries for the ARMv7 Linux cross-toolchain (Compiled by Linaro)"
arch=('i686' 'x86_64')
url="https://wiki.linaro.org/WorkingGroups/ToolChain"
license=('GPL' 'LGPL')
depends=()
optdepends=()
provides=(${pkgname})
options=(!strip staticlibs)
install=$pkgname.install
source=("http://releases.linaro.org/14.11/components/toolchain/binaries/${pkgname}-${_relverdate}_linux.tar.xz")
md5sums=('2ea94e329933f20a4cdf4cdc08e5d64d')

package () {
	mkdir -p "$pkgdir/opt"
	mv "$srcdir/${pkgname}-${_relverdate}_linux" "$pkgdir/opt/${pkgname}"
}
