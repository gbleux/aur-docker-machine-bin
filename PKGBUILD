# Maintainer: Gordon Bleux <gordon.bleux+aurdmb@gmail.com>
pkgname=docker-machine-bin
_pkgname=docker-machine
pkgver=0.2.0_rc3
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
sha256sums_i686=('20dfeceb11f0989d824ee778195bd930c4d45075c7eea25e3e7ebb5dbab3f0fc')
sha256sums_x86_64=('7d3a5499481e95f9fdacc400f5457cd084ad9e6a90d205ec1d416452c0ca1f77')

package() {
    install -Dm755 'docker-machine' "$pkgdir/usr/bin/docker-machine"
}
