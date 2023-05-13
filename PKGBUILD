# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.0.1
pkgrel=1
pkgdesc="All variants of Nerd-Font-patched DejaVu Sans Mono"
arch=('any')
url="https://github.com/ryanoasis/nerd-fonts"
_raw_base_url="https://raw.githubusercontent.com/ryanoasis/nerd-fonts/v${pkgver}"
_raw_font_url="${_raw_base_url}/patched-fonts/DejaVuSansMono"
license=(MIT)
provides=(ttf-font)
source=(
  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-Bold.ttf::${_raw_font_url}/Bold/DejaVuSansMNerdFont-Bold.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-Bold.ttf::${_raw_font_url}/Bold/DejaVuSansMNerdFontMono-Bold.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-Bold.ttf::${_raw_font_url}/Bold/DejaVuSansMNerdFontPropo-Bold.ttf"

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-BoldOblique.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFont-BoldOblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-BoldOblique.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFontMono-BoldOblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-BoldOblique.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFontPropo-BoldOblique.ttf"

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFont-Oblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFontMono-Oblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFontPropo-Oblique.ttf"

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFont-Regular.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFontMono-Regular.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFontPropo-Regular.ttf"

  "${pkgname}-${pkgver}_LICENSE::${_raw_base_url}/LICENSE"
)
sha512sums=('56eef74b3946701eb91585547c2a2679114297247b5d02c9745db1fe95c2006108649e50367f9189fc0e65bb2d06cb10a618cd989d1ec02175d00dac2c42e902'
            '541ca08417cf2b8414e527f085970b5879d318228c4083fd9e37447dd33b3ed9e366664946bddda739981513a792605b950780d9c61b50a9adb019376ce4e7f7'
            '81967f655a45b30ff44d858573d9322c312d69462449f69bd1e7ba44beb7c8bc5a2f5c484e3a67a0e9a5f46d573c8de2a4dfad6d5f6cdf79f5a0354ec5d329a3'
            '03f07ff3a95f5f84f91df8f3651b3d74c0b3225ce4b4aec7de2d4f10e233d28a8abd8668ad0bba9db53554745d6a65d275306fbefa04c33184ffbeb318b730f0'
            '1d60ebbb8c8512780b37c084c3d6426218e3ae5d4fc0a838c7113b29e795e2e9ec7f4fc64a5976117a265244fd445f0d27849b81a293bcca56b9214818d506f3'
            '3651c3ac0a1aaa816053810ec62ab7edf21aab7be037cce6f28954fe4b9c3a5e96e3cea9bc0fde9d13f625820ae453433239857e378a551eba9a2f69916269cd'
            '877e94632d6a3d49342c2341486aeea8fcdf54f59a719eba11542eff149ad24c6c8cb083e3160a5647fd8f460d0f92ae2bba5554c4a79b671bcc890234170f49'
            'a03fdf3e417990f85467e940c89526861d53ca334699ee0152e3100995e842c28c97c7229bd64563208bbf40ff068311d670c68713ca050b9891ae6b03a8a003'
            '2e1f06645ec29b65dbf29c56e6c137bcb28fe8606dc3baec4079869484d303c4f0a1c2fa32aca064b8e0498ee2f7a9803a61cf4e3d821e05f30fb0973787b126'
            '105cd8a77d977968610e6b5c9ea9c86dc1583a2a4f8bc4c195bd78290e3db1b1855b5d0c6fd3b26d481fda29a870990c906d13e3679a07d7137644f43a9698b6'
            'c3ca69fb8fa1d99a56ba28bff79e3a3f0e45528d1ecf54958ccbbf0212f905ea628c3307e63be063a799cb81bee14ce2a2cf48d335999101c5450315f566c765'
            'e430851172e91a43dead98c4ee97d19b772dd002f42eb5e93092a9771f3fff7bded3ffacc8dfbd3627db17ad6da97a01609334b38b4e3a6e57ba777247c1d4b5'
            '54b3d670b99a1128b32e61078165ddf9823a43dd51ef4f523b58a4d5638180ee57a22d90ce76e8955f50b6b556bc0f7ee32231d6abbb95575ceef7376e61215a')

prepare() {
  mkdir "${srcdir}/${pkgname}-${pkgver}"
  for srcfile in "${srcdir}/${pkgname}-${pkgver}_"*; do
    ln "${srcfile}" "${srcdir}/${pkgname}-${pkgver}/${srcfile#${srcdir}/${pkgname}-${pkgver}_}"
  done
}

package() {
  install -dm0755 "${pkgdir}/usr/share/fonts/TTF"
  install -Dm0644 -t "${pkgdir}/usr/share/fonts/TTF" ${srcdir}/${pkgname}-${pkgver}/*.ttf
  install -Dm0644 -t "${pkgdir}/usr/share/licenses/${pkgname}" ${srcdir}/${pkgname}-${pkgver}/LICENSE
}
