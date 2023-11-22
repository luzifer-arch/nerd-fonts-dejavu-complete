# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.1.0
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

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-ObliqueBold.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFont-ObliqueBold.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-ObliqueBold.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFontMono-ObliqueBold.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-ObliqueBold.ttf::${_raw_font_url}/Bold-Italic/DejaVuSansMNerdFontPropo-ObliqueBold.ttf"

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFont-Oblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFontMono-Oblique.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-Oblique.ttf::${_raw_font_url}/Italic/DejaVuSansMNerdFontPropo-Oblique.ttf"

  "${pkgname}-${pkgver}_DejaVuSansMNerdFont-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFont-Regular.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontMono-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFontMono-Regular.ttf"
  "${pkgname}-${pkgver}_DejaVuSansMNerdFontPropo-Regular.ttf::${_raw_font_url}/Regular/DejaVuSansMNerdFontPropo-Regular.ttf"

  "${pkgname}-${pkgver}_LICENSE::${_raw_base_url}/LICENSE"
)
sha512sums=('1d1c44be336f8d37b0550843a3149a27fc90e8022d5fe2e2a0b3fe09b0d298919c7c76a49acd59c9b2c495e8ca1d8e4b5bcced5aab05c7f0c9f094ac79e34d49'
            '6da1cedb2b3980def1c4ce47c1145cd183825046c7309e303d0a0bd8fa2d27bb3523d605279068bbd4bc3d6bbdbec7932866da8a1433cce280e68753a985cd37'
            'b82161a7e4b8e903c2ce16d8b5732e14d3f3489eaaf96807c14c52b277bb05a72596561400518a62adfb843acb69139c84383fa45fc03f05e200de498abb0a85'
            'd4c6ea2f5f7e85eb2a2171f0f149110ca03b46c92d80281a5ce8554df95bd942d225cadc37addf249838d6a8c7e9ff8f71530331b6e32801dc5f560e568076eb'
            '38f854c4da5cb39d90e87ff8eb344835f306930a0c6df3f401a179faf2cafd1b45af416e663305b22dad0189132b8dd2c3c6a3f5fa9a988e3a55ff857202bc79'
            '7292b8aca1ecdbd23910a8e914b8b157fb6c44992cfe35b2dfaf4395533b84cd5828334efa453ecd1d692ec88a52a33a6afe34a161a734979954b5afa13af468'
            '31ecc2064245b3cb3e1c8958e99d7b6f2ebf209ba51e7dedd374e2f850190ca2ce22af2a6a98fba30bce6ad4d7ccd73b7f40537e31a96a3aa1c66cedec7e8685'
            '7da542fac493d95e920cdbd7611d7ae0ea3ec0015d80b6422bb82061a8c3e46eec45bf402f6b7df8e467c273b5a55933908ac10d0c01596e8505cfd671fae4b9'
            'ef8954329de1fbda2cc11b26942a103048ef2a9ce5b0d8426cefd14481cf085496e6582a688d96bb9d24678714251596c57a2babc07f15d6a0dbd78a562c89e6'
            'c803984d8a1eacbadbe915bcf7e95c234ee508ef10fb40fec0c769705e965f3c327a5af0008c66f9403c6dc03abe719d57aedd174e453375f05049e589fef600'
            '055ab598414feaa3659327d34ec5cb32671316c5deea9c4c2566b39d317f7aa764d2486895ea12a641999f276152525e7f3a0123f453db48547208d080034211'
            'e9188ae3511a8bb10f999518809f1d0a72c7d0059b5e74e3ccb90ae23010dd6e4c26f8562b0dc21a9268912919f78a6d43d98efdcf54b3562aae6308f0ebc723'
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
