# Maintainer: Vladislav Nepogodin <nepogodin.vlad@gmail.com>

pkgname=cachyos-openbox-settings
pkgdesc='CachyOS openbox settings'
pkgver=1.0.0
pkgrel=1
arch=('any')
url="https://github.com/cachyos/$pkgname"
license=('GPL')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/archive/$pkgver.tar.gz")
sha512sums=('3c8d3e5bb0220a7e352673e3166305f934dee54fc6b4afd3271bca1c862494fd884983627099916d20e282e58142b1a3925ecb577b383d1f88f7d05143577046')
depends=('cachyos-zsh-config'
         'picom-ibhagwan-git'
         'nerd-fonts-fantasque-sans-mono'
         'noto-fonts' 'noto-fonts-emoji'
         'ttf-fira-sans'
         'char-white'
         'dunst' 'nitrogen' 'openbox' 'rofi' 'rxvt-unicode-truecolor-wide-glyphs' 'tint2' 'obmenu-generator' 'perl-gtk3'
         'mpd' 'mpc' 'ncmpcpp'
         'alsa-utils' 'brightnessctl' 'imagemagick' 'scrot' 'w3m' 'wireless_tools' 'xclip' 'xsettingsd' 'xss-lock'
         'thunar' 'thunar-archive-plugin' 'thunar-volman' 'ffmpegthumbnailer' 'tumbler'
         'gsimplecal' 'mpv' 'parcellite' 'pavucontrol' 'viewnior' 'xfce4-power-manager'
         'capitaine-cursors'
         'polkit-gnome'
         'cachyos-wallpapers'
         'cachyos-nord-gtk-theme-git')
install=$pkgname.install
provides=('cachyos-desktop-settings')
conflicts=('cachyos-desktop-settings' 'cachyos-picom-config')

package() {
    install -d $pkgdir/etc
    install -d $pkgdir/usr
    cp -rf $srcdir/$pkgname-$pkgver/etc $pkgdir
    cp -rf $srcdir/$pkgname-$pkgver/usr $pkgdir
}
