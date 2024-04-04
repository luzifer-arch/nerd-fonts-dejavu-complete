# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.2.0
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
sha512sums=('33c8956283a5766b1288a1e4617b894ced589f1c4fefc51023a45698a3b8e4d9cf69cdfacb5de1b36d5a6927eb510d67b8413913b33217b106a934475ae26581'
            'fda7ff9d24e0e49232ff5ce4a60315a3876159dab7864e4efaef4a39c771a511548157d0d175000badb9d6de8f1aa33b6b93eb13cbec58bfc4124a8a126abcab'
            '071f6e70c76afa5651a0c3cefb8da52449f5f1e45b18063ed13f0bcc4a7cea4779dfd261d3c81c5840b68d90a4bb526755d5ce8e7afe5668ebf19d9966007fd6'
            'a54fb632cbec3fc0c79d16981f8037de4f7efc5ead22408d72ae9d63f994ab1a2040c3d3f4547c99a0c0b9bdf48ae559c310e63d27f27c148f6af4bd087c5d52'
            'eaf2ccad975a96d7d806121ede0e973398d3c2fdd0123ca2651946f86abe5f12a3df891bf41c4a33144197d32a1cb14e8550bc59a6e5a81b8c2667f4c6cc40bb'
            'a7c169bca66c7657782cd63162cd5702a32f5b040a13fc28e0e7922319f6649da67d3b567a19ed9e2d015f3b0fd91779833970f3479002881461fad5bb584c0a'
            '0ad069c00f0a187c935ac6bd3c7cf86d3bdb8a654d928fc7f77f08a5058847b150284df7b82afc06d716edff26050946843fd8cf35d257ef78716693986c7b83'
            'f5703e501e532c018e044e2c27b27c9645335435b06b13c4a1e7a5e3c873b73d006aa88b4f3bbfd5d3c670e711ad2f8b45825e2dac8fa3a2cda12351565e50e0'
            'ae59c9684feecfb2fb735d9bb0141f2853218961e59fd03560296508dc8979612593611c6fa650b08b6443e5e612b9dcf1c288b06a0b144bc931f17204f43409'
            'ad2382bf9c4815313087db7a22f7ef5e3e1dcb58a4330ba676b78784cd992fa89d642171e5139fa7ba48abef7b66c68f21b95049920c5cd2c16d17fd2362a4d9'
            'd9d6b08a18db24bf00094b10862ae9bd04786c6b6da4efdd8e01e8215eda42c7202305010fded6d7bbbb6d21a13d80f334257a69a50b9fe82502e28aa2992198'
            '27ed7e4dbb4c01cdbba2537baba83a5c57bd89e1997b2aa84747e83fadeea3f513d3d01d6388bd9d40e661175b0d202ea5b069dc3c615869490c4b17e72b4d86'
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
