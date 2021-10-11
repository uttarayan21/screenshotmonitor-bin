pkgname=screenshotmonitor-bin
pkgver=1.0
pkgrel=1
pkgdesc="Screenshot monitor tool (bin)"
arch=(x86_64)
url=https://screenshotmonitor.com
provides=(screenshotmonitor)
depends=('mono', 'gtk-sharp-2')
source=('https://screenshotmonitor-download.s3.amazonaws.com/linux/ScreenshotMonitor.deb')

sha256sums=('9b35e8722132d641e1938874495a625a53754215b3e1228860671050f7678d0a')

package() {
    tar -xf data.tar.xz -C "${pkgdir}"
    mkdir "${pkgdir}/usr/share/ssm/data"
    chmod -R a+rwx "${pkgdir}/usr/share/ssm/data"
}
