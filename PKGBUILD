# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.0.2
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
sha512sums=('e073dc9eb1e39ad49569f9e561d4b0b79e548545ae8c91bf41f50ac90d8dadd66269d43dda43fde4bcd74c171852a204614ff907fcee22ff2173dc4e27943aa3'
            '024a96741fa21f6725af9f3c5211c5d6cb6905dce65bbae47d0539c7f70de80eecc2f08cfc534bc943760e7247f84818c258cb20235c392e3c90f07c8a8041d3'
            'dbc2a68557d38ffa051d40d1cbc09142e46dfd5338eb4fae3254248217b6fbd0cd01840f5d07c28eb9665e7f43b0271f53f50d014b111f1a560eb725de1911c0'
            '9407958a6418553a1cc65205b3e3c9dda038d2480fc717a634da8577c386f6f751ebf9813f2f8745bc16d333ed7991f432b5ec5709fee6087e2c6c51a706ec8c'
            '71a17680210efa7e56f48d46d32b2f676978a4f51deef4850408f9c10ae3b56d958bc245333500160092a083e65f556f8a6c66bf76817f7927781a42c3219bf0'
            '105d7691d2b986a606c2625603341687ec24356d4414d3a9bcc67c8e57c11a3dc444302c77ff190d534cc8b2ecc1bee3346ce7eb499bfbb4c1b9b566da53e0e4'
            '5478a0ceedf860f0bf3410f5e2b926bbe4710cb9ef095315e67230a868914e3508b65d793717596105dc7f79097b830164ff05a703a6b0b159c5f302b69a7125'
            '34a69f218d08df128f5de46c76a0b114f843c9e5d7ea128fa1315849895c39c60b0c60c55ab89d9b6ec83a0c76c1275e56445ae24b99ed34b9a6ed8b9f6749a4'
            'e8323f55c089ae2e5139da5f875d906be296c4c9a1a4e2f98b5cddd0d366b696d5ca2fdc1f8b4b11015292187eb0637bf9357e5407859418aceb4990789f7ed5'
            'd3153992ea85c1cbc1e8f6b92ebcffe8ee7b57b6979420be2a69483a5741fc5033922a94b0dc7cb18c98c70bb80e574174e5b42a73389dd63b5236b7067a3bf9'
            'b3334db5da5bb49d9be5338b4ca4644f8d746a951cef9dbae3c0171d5179a3f99ced6ed8644be09860d2219668d0cf2874d27c9182cde0a036a177ec05144e1b'
            'bb7f7686d0230aa8f01350c803d175395cd6351105ce628220cc9d6998f0052e488d45bfe771c3a674b794c858b69326154817469e5b6a7b2bebe448c6b51303'
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
