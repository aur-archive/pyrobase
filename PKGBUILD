pkgname=pyrobase
pkgver=0.2
pkgrel=2
pkgdesc="pyrobase assembles general Python helper functions and classes"
arch=(any)
license=(GPL)
url=http://pypi.python.org/pypi/pyrobase
depends=(python2 python2-distribute)
source=("http://pypi.python.org/packages/source/p/${pkgname}/${pkgname}-${pkgver}.zip")
md5sums=('71c3d183988a7cddb8c28c4a9fe598f2')

package()
{
  cd ${pkgname}-${pkgver}
  python2 setup.py install --root="${pkgdir}" --optimize=1
  mkdir -p "${pkgdir}/usr/share/${pkgname}"
  mv "${pkgdir}/usr/EGG-INFO" "${pkgdir}/usr/share/${pkgname}"
} 
