pkgname=gloriousctl-2ms
pkgver=1.0
pkgrel=1
pkgdesc="Command-line tool to control Glorious Model O/D mouse settings, modified to support 2ms debounce"
arch=('x86_64')
url="https://github.com/TheRealTrip/gloriousctl-2ms"
license=('MIT')
depends=('hidapi')
makedepends=('git')
source=("git+https://github.com/TheRealTrip/gloriousctl-2ms.git")
md5sums=('SKIP')

build() {
  cd "$srcdir/gloriousctl-2ms"
  make
}

package() {
  cd "$srcdir/gloriousctl-2ms"
  install -Dm755 gloriousctl "$pkgdir/usr/bin/gloriousctl"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
