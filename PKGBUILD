# Maintainer: Pavel Horniak <gouster4@gmail.com>
pkgname=technic-launcher
pkgver=v4.666
pkgrel=1
pkgdesc='The Technic Launcher will get you playing your favorite minecraft modpacks in no time. Choose from thousands of modpacks and install them with a single click.

Offline (LAN) version'
arch=('x86_64')
license=('GPL3')
url="https://www.technicpack.net/"
depends=('jre8-openjdk')
source=("technic-launcher"
"technic.desktop"
"technic.jar"
"technic.png")
md5sums=('SKIP' 'SKIP' 'SKIP' 'SKIP')
build() {
   echo "copyring files..."
}

package(){
  # Moving everything to pkg/.
  mkdir "$pkgdir"/usr "$pkgdir"/usr/lib "$pkgdir"/usr/bin "$pkgdir"/usr/share
   "$pkgdir"/usr/share/applications "$pkgdir"/usr/share/icons
  mv technic-launcher "$pkgdir"/usr/bin/technic-launcher
  chmod +x "$pkgdir"/usr/bin/technic-launcher
  mv technic.jar "$pkgdir"/usr/lib/technic.jar
  mv technic.desktop "$pkgdir"/usr/share/applications/technic.desktop
  mv technic.png "$pkgdir"/usr/share/icons/technic.png
}

