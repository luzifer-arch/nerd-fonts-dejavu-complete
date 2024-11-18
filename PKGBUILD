# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.3.0
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
sha512sums=('ec692a60f7f690e497dba62b84a564a50818ee5ac02352f94fa78cbaf7c854ab8747e6baf7cfe8ce2a18b1c91aff62f9021f3b3779f8cf480ae173e6dc078157'
            '8f0fbcdee8bfb593fe194f4c06241b31d6613e9af8031edb5f02c0016f70a1564b2ca0d3595c35124eb8d7ca6d96f1df9c22c8ccb55146acf7de246665515e1b'
            'f76b1c96409e64a2fc348aecf9dfe7a79a10dc810595df250baf2fe7ae46b3975db049750afdd2671ab9c1060c75ccf8087ae5ba0b01e0555575ad6263454a54'
            '8ff8a1963adbf4cba971b4416f0edec3c8e79d3e5e10ba35c23284de7902d873707360a18168312f4331307807aadd86edfe5d970ee2fb98545f8e04b0b53470'
            'b34a4154bfee8bda4ec5a10882a23c0540c306f9e4b9e9b47d905dd5bba4383a5dc40f3fc80536110085904af8ade9ad5d3dd127666e61033eb94201456eccf8'
            'aa37c5b3ad7f65b5e5ca6e82f147b2adfe7cd4ee8d6371219b9b2e63d86b8866a466bf47ef0e29928664f461e732e950c7e0a1cab57310479553a21d497eb878'
            '12175019fcc8dc51d38e8b0f9529442fb4729d57b959b654dfca92d0ff378d6a68441af0802231b7e9709b9238ff80065bf66566c5fc1923dd0736867db0e3ea'
            '0cf873f0ec9f3ade42812d1745253ddf0baa553414c8d871c96af859f5b217085c147eb353b8f3e8428deea9d2b66061ba7a238c72ee1b725606939cbba6c159'
            'd2b6862cb277d8eb02789e4715bdc6ec52bfa20390c5f0116f89843782c5685b29a0a16be7c3bf5b48d4b02e2cf4948a09eadd2acfd2cea0c9957fd39aeebd2a'
            '43d72a19c835205623cd0adce85ea2c50533ba2675a718b8569a1181d4d3203b902c7f206f9e6017d242b362fa3925e40a0919f83724048c70ada90d2f09184c'
            '76fcd5f4b585b7926d138faf0659ebe2e1eff502d44ad1904b2fce7427d216d2ae2c401fe7b2aeeeeabeb6d0143a5529e5a7ed1af4736c512a5eb94f2e5b3ce6'
            '2fa7fdf0f12053778adaa93d8a86ac10f7d9ee03405c7e19fb98d73cd411430a838b9f5d48bdb7ec57d04756036e129488a0acb2aeb8fa5a02cc0d1cb4b0fae2'
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
