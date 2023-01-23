# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=2.3.2
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
sha512sums=('c63371545166e9f42982afda6e1301bf6ff44edc11653f6cc58fc5f8d0aa50079a123bc647666855899d9e4604299c4b0c4d551aebcfd4e57b0ff37c00c05853'
            '17856fb0f3067205b604c013148afbae72a1a5592127df100c81d221d4317e6b5a0df7d6ed05abd8e353713a8bef79f92036143756f2ba4ba239f383c5c8ee90'
            '8a1f189da0ff0e3280534247a16db21fd0231341a1fc51bb373dbee8c7cca212391d278f84b80540dc089aa708e57d9f568972556b1b3601a28e9f5db0194152'
            'b6b68d1bf3f971acabc4e16744af83ef706e975b919547e9aa754df14cb35ecef488c977defce4e2993d2a36b91201bec09de7e5d1d3fafabe258a440437190e'
            '908db3712eb76167c1406ef9cea8d6fb54ffe2cefa492e912e225744a798d3aef3d9507321de6f57d30dd9f5ab2596b82b64ba11cd1b5c378dfdd8986fffcd85'
            'c2e26cba9d48df77970667063e743bb262cb6391e2d7bbca862d90c44712ff3e0251c2047f2ed29fd93abade20eba0abc12662a839ef43c7f8ea88c89e88553d'
            'd94b58e31427e328fd42afff9379583753cee83945acd4280c5f0c37295ba7c0252833d5c1e6302b662ff00089d4b8f1b15c036fb3eeb10e9cbe202e69c7481f'
            'e38be542f911bd643c674e13c6ff17f0699b972c1caf5799fb4cdbc9f8779893c4fa42e8e7af48686cef1b9ae435f3ca4ce3e61a601da2748c1d46a739ba634f'
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
