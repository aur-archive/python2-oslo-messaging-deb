# Maintainer: James Bulmer <nekinie@gmail.com>

pkgname='python2-oslo-messaging-deb'
pkgver=1.3.0
pkgrel=1
pkgdesc='Openstack oslo messaging api'
arch=('i686' 'x86_64')
url='http://packages.ubuntu.com/saucy/all/python-oslo.messaging'
license=('Apache')

depends=(
  'python2'
  'python2-six'
  'python2-iso8601'
  'python2-oslo-config'
  'python2-babel'
  'python2-stevedore'
  'python2-eventlet'
  'python2-yaml'
)
source=('http://archive.ubuntu.com/ubuntu/pool/main/o/oslo.messaging/python-oslo.messaging_1.3.0~a7-0ubuntu1_all.deb')
md5sums=('ff5b0cb1afc8927d051cc682f8e421dc')

package() {
  cd ${srcdir}
  tar -xJf ${startdir}/src/data.tar.xz
  mv ${srcdir}/usr/lib/python2.7/dist-packages/ ${srcdir}/usr/lib/python2.7/site-packages/
  cp -r ${srcdir}/usr/ ${pkgdir}
}