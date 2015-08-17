# Maintainer: Igor Duarte Cardoso <igordcard@gmail.com>
pkgname=vmware-usbarbitrator
pkgver=9.0.2
pkgrel=2
pkgdesc="VMware USB Arbitrator script, including unit for systemd."
arch=('any')
url="https://wiki.archlinux.org/index.php/VMware"
license=('GPL')
depends=('systemd')
install=$pkgname.install
source=('vmware-USBArbitrator'
        'vmware-usbarbitrator.service'
        'vmware-usbarbitrator.install')

sha512sums=('66d1588b3a1637106e5d8469a8e38b9f61970a3954a8b41384a72b8b019cd52dddea56ab0d708fc23b043ac99cd472f8efeb0e28abcb6fe25b18aef774dd3944'
            '39f7b4d431a3ca7ee619a0686cdc63b6543a48947c87f8c988eae2066c83ef8e565e039f7eb275b32f6951b423917f916cc5900f502633d331dfe32d64453e0f'
            'c83978d2c5d6e8c1d1404935badd633b45cbebc00468d052aa4a53d391a760e1ce0b557a4304a7827a77290c0b518b15cb629906620342b1276a4d7e97773517')

package() {
    install -Dm755 "${srcdir}/vmware-USBArbitrator" "${pkgdir}/etc/init.d/vmware-USBArbitrator"
    install -Dm644 "${srcdir}/$pkgname.service" "${pkgdir}/usr/lib/systemd/system/$pkgname.service"
}