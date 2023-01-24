# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=2.3.3
pkgrel=1
pkgdesc="All variants of Nerd-Font-patched DejaVu Sans Mono"
arch=('any')
url="https://github.com/ryanoasis/nerd-fonts"
_raw_base_url="https://raw.githubusercontent.com/ryanoasis/nerd-fonts/v${pkgver}"
_raw_font_url="${_raw_base_url}/patched-fonts/DejaVuSansMono"
license=(MIT)
provides=(ttf-font)
source=(
  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Bold-Nerd-Font-Complete.ttf::${_raw_font_url}/Bold/complete/DejaVu%20Sans%20Mono%20Bold%20Nerd%20Font%20Complete.ttf"
  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Bold-Nerd-Font-Complete-Mono.ttf::${_raw_font_url}/Bold/complete/DejaVu%20Sans%20Mono%20Bold%20Nerd%20Font%20Complete%20Mono.ttf"

  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Bold-Oblique-Nerd-Font-Complete-Mono.ttf::${_raw_font_url}/Bold-Italic/complete/DejaVu%20Sans%20Mono%20Bold%20Oblique%20Nerd%20Font%20Complete%20Mono.ttf"
  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Bold-Oblique-Nerd-Font-Complete.ttf::${_raw_font_url}/Bold-Italic/complete/DejaVu%20Sans%20Mono%20Bold%20Oblique%20Nerd%20Font%20Complete.ttf"

  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Oblique-Nerd-Font-Complete.ttf::${_raw_font_url}/Italic/complete/DejaVu%20Sans%20Mono%20Oblique%20Nerd%20Font%20Complete.ttf"
  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Oblique-Nerd-Font-Complete-Mono.ttf::${_raw_font_url}/Italic/complete/DejaVu%20Sans%20Mono%20Oblique%20Nerd%20Font%20Complete%20Mono.ttf"

  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Nerd-Font-Complete.ttf::${_raw_font_url}/Regular/complete/DejaVu%20Sans%20Mono%20Nerd%20Font%20Complete.ttf"
  "${pkgname}-${pkgver}_DejaVu-Sans-Mono-Nerd-Font-Complete-Mono.ttf::${_raw_font_url}/Regular/complete/DejaVu%20Sans%20Mono%20Nerd%20Font%20Complete%20Mono.ttf"

  "${pkgname}-${pkgver}_LICENSE::${_raw_base_url}/LICENSE"
)
sha512sums=('466ae169f648a7a1334ca0a303c5616c8c657c5cbcf5ddf653f8fb5c3cedd635dcc1d22ad4efc936b66dd410a20255f7f2d35c9527d52a9c936989b13a5c0d71'
            '850fb7c046e206bf67b7ca534aaec9d40c531b8a65fe3dcf03cac40d0d581b0cfdc1760b30d597e67355b72bd51276f65f2983ddf8b55bc957f31cabcd524eac'
            '574fb59493f063a9b705c2a738c11d185d904d678d76ddef56fb338f2fe1475a6df1fe3623c9e6ffae8a5673bea7020c7fb14b878057ca382b042012da9237a1'
            'f0cbe8e59cb1379a7bb15b824d2aa57b773913abdf22c9c3f0a22462ec51b973aa04236bf4bdff6ff38be4f11889bfdc71a550a212799b51cbc93da5ca87562f'
            '4bc7c892e7a19bad3c06700bbc5b51a3e9eaf499006cb8f9f2561e36dfc14800f28bbb833549af0a3f64b70869726790353aef9dc46e2f5c4d3ca839cfa39ddb'
            '72432fa5945b9e150bd7dfee1cb5d698831acc932b07edffa0d4737eab5b336a7a1c8951dc99dc74c6f53fd726e93dd811b1016da91f1d14522a75abb680e5b3'
            '16a189cac183791eee4ba8faac6a681e1dd8f8278b174435b35ad9466fcf2958c6fb13304771e6e51f82a347f45fbf29f8513c9835383537675242c40750075e'
            '18f39622670f08eb9ac681f3b099ab3c12574b288ce00af7f3ce8052fcb8db0adacc7afbaf71482cb84602b72762cd8eb1e53b377e1f27e60cd9c02052b637cc'
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
