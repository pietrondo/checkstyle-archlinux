# Maintainer: Jaime Gil de Sagredo <jaimegildesagredo@gmail.com

pkgname='checkstyle'
pkgver='6.3'
pkgrel=1
pkgdesc='Checkstyle is a development tool to help programmers write Java code that adheres to a coding standard'
depends=('java-environment')
arch=('i686' 'x86_64')
license=('LGPL2')
url='http://checkstyle.sourceforge.net'
source=(
    "http://downloads.sourceforge.net/project/checkstyle/checkstyle/${pkgver}/${pkgname}-${pkgver}-bin.tar.gz"
    'checkstyle')


    md5sums=('0e1a704cc956be3b56732a214d819a4d'
             '8326c63991962d738fa9c55d0dd8d64d')


function package() {
    local destdir="${pkgdir}/opt/${pkgname}"
    local bindir="${pkgdir}/usr/bin"

    mkdir -pv ${destdir}
    mkdir -pv ${bindir}

    cp -r "${srcdir}/${pkgname}-${pkgver}"/* ${destdir}

    install -m755 "${srcdir}/${pkgname}" ${bindir}
}
