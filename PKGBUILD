# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.2.1
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
sha512sums=('4cd8d85ea55ece45bf2b47710a92b21b228a8e09d460c6b646074b40cc52333dbac73c5e3753b9b730463bf588b349a82cb408c1f600b5a2820de68de81715ed'
            '8053dfbb893ff491b3d2bf8e8ac98a6495cdd0eaabd9d172ef155a5e0009d832fcf3c3035524e74b38104fdc935a7ff2352169128b5abf8de440646de3e6ecf5'
            'a96e241b6a08ad3ea19f5d7163ee2b642246c63f40eb0956c4a17a24d6231941180c256611db38e5c705d1d76a5ece554f7a7c474f093fe21bfcb0d5ee247ca1'
            '1b7effd53287053ff5c6a126ba00488bf8fca5cafb92bc99e2929d41c083f6c4caaf47dbeb04ac863e66da8a95322eec0adad4172a2c1040464a50fe5506f98b'
            '8fc91e9a6cca88061aa1e5ef2ca0fb41cb59fd67b9122262bfda52a879cee905cae707c082f4a9f4ee9d7d4b678b307d27f1a90ec9a6e310966f45a25c7cd445'
            'a99aff77acdb8cf703c7cc9c1afbc40cc3009407cf726e0a8fe8c5b363a201cc5105c4a1c3e26f0a969d6fa6d77fa1e64e37f17063199e969907be62e6d17c25'
            'c474a3490d38e64855079be899727063523f6e14625b89afbb30bb93e498dc1bc3c24d81618bbcd5988703c3b5967e6ee9bddbf3d2af9f21a5aa742541116651'
            '1925ebdc72bd562d6da0093acab3f15b41e68a643c8012f23261da7260aa341b2600596bea2881b8a5706439c3c09cb15021290ec15a30117efdf404f8ab6461'
            'e39c239e2a41f01db1d4051e44455376863d80e9532bbd683e5cdf9534b4d9440db2780ad9d7d070cb100ce218674cf6f14f2b62c036c83fa530c425a5c1e686'
            'bf914e09fb0bb5598c8c90dd8297187d3600464945c5dfaf6beffe3a47c40f878aad41a4a2b409ce0cd8a758831e37ffe932702b4e8b702d5658ece4cbe50fbe'
            'a12deb102de163f87dda8398fe3512ce3b36ed20a54836b58479f9fd5e4e1685eabba70e52bdf195b0ebcd58486be1bbc863833c4e6475703aa831b786007ab7'
            'c6504ec5c007c27f342789a2d4be1ef2365d67bc8f20b317167e2352fab68667f1682fb89f375928c4c20a0e23cb7e4e841f7f437f486a090576436c124e333f'
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
