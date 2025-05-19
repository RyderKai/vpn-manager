# Maintainer: Ryd3rK41 <the1337lonewolf@gmail.com>
pkgname=vpn-manager
pkgver=1.0.0
pkgrel=1
pkgdesc="A Zenity-based OpenVPN GUI Manager"
arch=('any')
url="https://github.com/RyderKai/vpn-manager"
license=('MIT')
depends=('zenity' 'openvpn' 'sudo')
source=('vpn-gui'
        'vpn-manager.desktop'
        'vpn-icon.svg')
sha256sums=('184d60c263926c0a5789fac3d39d428bdfd23c3a855489cae64f19c52bd31111'
         'e38f6f8d2ea6b77472f8f23a893c159b9eafa775687dabc26b2829dd50983c02'
         '7d99f3470bf101a3acd5aae4f3ba1d2e380ef97aac1c2c299306d770bbd82d62')

package() {
  install -Dm755 vpn-gui "$pkgdir/usr/bin/vpn-gui"
  install -Dm644 vpn-manager.desktop "$pkgdir/usr/share/applications/vpn-manager.desktop"
  install -Dm644 vpn-icon.svg "$pkgdir/usr/share/icons/hicolor/scalable/apps/vpn-icon.svg"
}
