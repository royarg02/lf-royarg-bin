# Maintainer: Anurag Roy <anuragr9847@gmail.com>
_pkgname='lf'
pkgname="$_pkgname-royarg-bin"
pkgver=26
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
sha256sums=('85278c32e05b47dc2b610e638ca3bd881d343da80f62d7f4c71d6a6344679588'
            '8435d4ac067dc81aedacc2cbc67d72449e39027ff3ec55d2b3910f3712dd1f74'
            '077f3c8aa73a4886221438f9df5c1551baab43c6a0f2e7cddf56f436e8b63480')
sha256sums_i686=('09eabddcf198395171392cb82b4f5834f9e54509b99b35e883022ca41d95352c')
sha256sums_x86_64=('0a07b8cbceadac4fea003f55f6ba5afa03cbb87261b1f6d2c8933286996ded75')
sha256sums_armv7h=('8a94ef07d35e41095bf8b218ab2cc2f71cb9f15eb91b2aa684f24693ab9a6886')

package() {
  install -Dm755 -t "$pkgdir/usr/bin" "lf"
  install -Dm644 -t "$pkgdir/usr/share/man/man1" "lf.1"
  install -Dm644 -t "$pkgdir/usr/share/applications" "lf.desktop"
  install -Dm644 -t "${pkgdir}/usr/share/licenses/${pkgname}" "LICENSE"
}
