# Maintainer: Knut Ahlers <knut at ahlers dot me>
# Contributor: Tiago Brait <tiagobrait AT gmail DOT com>

pkgname=nerd-fonts-dejavu-complete
pkgver=3.0.0
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
sha512sums=('37b006948fce7349e7f355f183e236d9b5603e7a6dfc4687afde56e58200e7aae5e23ba3e545eb713bc9f6f13686ca818aff8dad377b28836d8c2497f327c937'
            '5b81a6bca1ac54a21af94f98b90d86cd2e483ecae35111d4d03a4598368ecdc330831db2e84838c51809163fba76fd6626e26b2f2220da2217c36617f2071908'
            'e75d0b8b8e6d530f6db54b954561a999d8e3cb95178027aeb8537827bf148549a35c7d4e802ce33d09ee4a0006f6f631e16bdd81a280237072b715ebbae7c75d'
            '7f31c997c333badbf83f21266f80329bb6d174944d44f7a6ced618c85989b53b4d1499cd7d08872cd195c8d003ea571814f939b1b6c6fbb27df031b8ccad3f0c'
            'f5485d46ae6fd331a2dc22fb51f81f1d5c3c4122ad6e2bd040b3321caba3f34a4ac7a0b8e53e7794bcae163e141609faa6f2c10f9e76de0b173e9ad2649b0f80'
            'e6f9931eb16edc79530f9ba16a1393a13ac59ae521d914e27d33eeaa548bb0f7a408bb5f7fe1374c19f8188d3dd294626c05783c259164fdeaecb4b81d0b5a42'
            'fbdaadcf27ee4d733186536c6c754300ab436725a93b4ca05eaf2b98765674f92d29b08325aa601de2ed1f2fd30af8efd92174a262b3c6e54f147a71401e15c5'
            'e94d328e0ef1aaf443f8e2ae7a1eebce7df7e12cf347aac8cf1b9cbd08576279c36f4feb2b1121cd93540261534f197562d9b8a3eda9e992ce27e8b6fd5c3649'
            '871e7eed63a1e479c3d680e1c4d427a5bef5219a62e219f0c55062477117eba4c2049abe0ca4aefeb3eb741eb51b2eddf577a2d150383ac2312a7784e5853a1e'
            '8bbcd6fc857e790a2be2b02b6c65b9d58feeb4d8f68d8e42447344d5d7c3c185ea1ddd9b10df0a30311e573bcb2147f6d96ee84fa87f9f7033d235e6aa4c5131'
            'fe00828bea57333c23d3adf5532bca99378a3cf8f66d6101f7b20cf478fdc9a7f3de51b7afcfe717664e6f37a9b0198c498f50e8546738e399313d9677c468f9'
            'b1637164a7faf0369cf145d8817be470f66cb1f9ef293810cad482f1f0252461d83acf3243f1e42a3b5443fe32e88adcb8a0a473f8165aca0b98555e63da22ed'
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
