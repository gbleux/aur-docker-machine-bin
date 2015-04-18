# Maintainer: Gordon Bleux <gordon.bleux+aurdmb@gmail.com>
pkgname=docker-machine-bin
_pkgname=docker-machine
pkgver=0.2.0
pkgrel=1
pkgdesc="Machine management for a container-centric world"
arch=('i686' 'x86_64')
_os=linux
url="https://github.com/docker/machine"
license=('Apache')
depends=('docker')
provides=("${_pkgname}")
conflicts=("${_pkgname}")
source_i686=("docker-machine::https://github.com/docker/machine/releases/download/v${pkgver//_/-}/${_pkgname}_${_os}-386")
source_x86_64=("docker-machine::https://github.com/docker/machine/releases/download/v${pkgver//_/-}/${_pkgname}_${_os}-amd64")
noextract=('docker-machine')
sha256sums_i686=('e047e71c544b32751dbb9e9796fdf4e540cd9177d22699862775a4b09267578e')
sha256sums_x86_64=('24a95d55524e6db84ac9db1cef0eba6ca764989d92dbcb8e28f778b7e1c6a0dd')

package() {
    install -Dm755 'docker-machine' "$pkgdir/usr/bin/docker-machine"
}
