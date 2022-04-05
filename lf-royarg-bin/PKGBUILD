# Maintainer: Anurag Roy <anuragr9847@gmail.com>
_pkgname='lf'
pkgname="$_pkgname-royarg-bin"
pkgver=27
pkgrel=1
pkgdesc='A terminal file manager inspired by ranger(precompiled binary)'
arch=('i686' 'x86_64' 'armv7h')
url="https://github.com/gokcehan/$_pkgname"
license=('MIT')
provides=('lf')
conflicts=("$_pkgname" "$_pkgname-bin")
source=("$url/raw/r$pkgver/lf.1"
        "$url/raw/r$pkgver/lf.desktop"
        "$url/raw/r$pkgver/LICENSE")
source_i686=("$_pkgname-$pkgver-linux-386.tar.gz::${url}/releases/download/r${pkgver}/lf-linux-386.tar.gz")
source_x86_64=("$_pkgname-$pkgver-linux-amd64.tar.gz::${url}/releases/download/r${pkgver}/lf-linux-amd64.tar.gz")
source_armv7h=("$_pkgname-$pkgver.linux-arm.tar.gz::${url}/releases/download/r${pkgver}/lf-linux-arm.tar.gz")
sha256sums=('936175e2cca41b95a94649c43138ce956165b16f46d193202ace85f610bbccab'
            '8435d4ac067dc81aedacc2cbc67d72449e39027ff3ec55d2b3910f3712dd1f74'
            '077f3c8aa73a4886221438f9df5c1551baab43c6a0f2e7cddf56f436e8b63480')
sha256sums_i686=('7735a1a203c58891bafdc6869f72606142694179eb5798b6674ef9e7b02dbd71')
sha256sums_x86_64=('b8f9431dc63f7b2cff8e4306cff4c075adbe9f0900b563f91a6b742a41290d7f')
sha256sums_armv7h=('e3dfc49ff95aacae1f44be882f8b36960182e200bad10f1afad3a63df37b0927')

package() {
  install -Dm755 -t "$pkgdir/usr/bin" "lf"
  install -Dm644 -t "$pkgdir/usr/share/man/man1" "lf.1"
  install -Dm644 -t "$pkgdir/usr/share/applications" "lf.desktop"
  install -Dm644 -t "${pkgdir}/usr/share/licenses/${pkgname}" "LICENSE"
}
