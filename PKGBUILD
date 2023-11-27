# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.1.1
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
sha512sums=('6ec6ed890450216448f8b856f99a2893f4e2e44a50f34b3ca60f06fd79b4abda9443e54e93c321f3904ecb70a843aa515acb46ed34281b89be241eec560c125e'
            'ed2246464d19c48e2a0dd776cebd9dbe3958c37d9981d4fc3e4cd8c50e8b59c30183d2052e9f88aa827d36fdf3c24f00a0b3e83eb47330090105adcab9e03ed3'
            'f43ed5922aacea41aee532117576e97d1f75683fd5425bdaceef302500c911b2f9bf14a420eedeb5f11070e1e70cc8dbbc19f7c0506bb4eae05dea12e636b4fc'
            'e226efff877eeaf48a01690e2ea215024f0835c333831e3e8371f49e3a2ac59df9086d2f5634f7d471e39a79085027901202790083293cc3273615abfe9571af'
            '0863718d1cfd8a3157174190b26b04720afc45f6272cc149dbda91697bbccba63f087f1e7b5976a443ce8de3ffc2ff24eb741ccbd28fab95f1c157a83c78ca99'
            'e7c853b3ce7c378fbee4dfaa215684cb1af0edcfbb509473a541c32e54159ddab95f623e1b18bcc2065617d465588e9d61425b363b584a3b3f2fa220de5e440c'
            '680613b2220bab54672ebd41bdfb8bca944b5f6cca785d5960f4c3591dc3530c1a259746d520dd81866b54616c37313fe57fa3fc1a586dc7d5954bfd22acf655'
            'd33c70ed3d06c3757120f2a080eb81da968436bd6b8b6f5e99c27dd26e1f55efe9da896c4cec4196d0a94f5b77091f3faa4d34d20029d5bea42e0ad9a9555dbb'
            'f7aa217c3575c093bd876dc0782cc924a909c990d5e731901302a45c40a9d9a685354f6b0f00296af925c69597ebe6df817454098ff5a2acea7ab114774a2ff5'
            'c07544b41fa48af8c9c7ec0984c211a28a33af63b5b5d2cd841d1263f7d1228df010e3674f816ae75f59f3f96d77c1aafd94b96210e8b493d7dc951c0cc955dd'
            '4dd8c1c80167abf0e485a7087c299551dd99cb626dc22dcf09361216024f19c216826f02252c85da0223bf14068063b929e01e87b393a3b93217171de7088dec'
            '9c30219bb2c69da64e206b9aa987ed312c72e4f665cb1fedf6f475f5106f3798db4879e59dd421c72f9e4668975f7ba8d33ac189cf2dabdc74e87df61d8f29cc'
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
