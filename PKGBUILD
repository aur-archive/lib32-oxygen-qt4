pkgname=lib32-oxygen-qt4
pkgver=4.11.15 # Version taken from i686 kdebase-workspace
pkgrel=1
pkgdesc='Libs needed for lib32-compiled Qt4 apps to use Oxygen KDE Style (such as Skype)'
arch=('x86_64')
license=('GPL' 'LGPL' 'FDL')
url='https://projects.kde.org/projects/kde/kde-workspace'
depends=('lib32-acl' 'lib32-libxml2' 'lib32-libdbusmenu-qt')
source=('https://www.archlinux.org/packages/extra/i686/kdebase-workspace/download/#kdebase-workspace-i686.pkg.tar.xz' 
	'https://www.archlinux.org/packages/extra/i686/kdelibs/download/#kdelibs-i686.pkg.tar.xz'
	'https://www.archlinux.org/packages/extra/i686/attica-qt4/download/#attica-qt4-i686.pkg.tar.xz'
	'https://www.archlinux.org/packages/extra/i686/strigi/download/#strigi-i686.pkg.tar.xz')

md5sums=('SKIP'
         'SKIP'
         'SKIP'
         'SKIP')
         
install="${pkgname}.install"

build() {
  true
}

package() {
  mkdir -p $pkgdir/usr/lib32/kde4/plugins/styles/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/kde4/plugins/styles/oxygen.so $pkgdir/usr/lib32/kde4/plugins/styles/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libkdeui.so.5* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libkio.so.5* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/liboxygenstyle.so.4* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libkdecore.so.5* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libattica.so.0.4* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libstreamanalyzer.so.0* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libsolid.so.4* $pkgdir/usr/lib32/
  cp --preserve=mode,ownership,timestamps,links $srcdir/usr/lib/libstreams.so.0* $pkgdir/usr/lib32/
}
