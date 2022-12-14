# Maintainer: Onur Ankut <onurankut123@gmail.com> 
# Contributor: Rob McCathie <korrode at gmail>
# Contributor: Giovanni Scafora <giovanni@archlinux.org>
# Contributor: Sarah Hay <sarahhay@mb.sympatico.ca>
# Contributor: Martin Sandsmark <martin.sandsmark@kde.org>
# Contributor: heaven <aheaven87 at gmail dot com>
# Contributor: graysky <graysky at archlinux dot us>
# Contributor: Arkham <arkham at archlinux dot us>
# Contributor: MacWolf <macwolf at archlinux dot de>
# Contributor: Andrew Crerar <crerar@archlinux.org>

pkgname=vlc-git
pkgver=4.0.0.r20473.g3a08825c8a
pkgrel=1
pkgdesc="A multi-platform MPEG, VCD/DVD, and DivX player (GIT Version)"
url='https://www.videolan.org/vlc/'
arch=('i686' 'x86_64')
license=('LGPL2.1' 'GPL2')
depends=('a52dec' 'libdvbpsi' 'libxpm' 'libdca' 'libproxy' 'lua'
         'libmatroska' 'taglib' 'libmpcdec' 'ffmpeg' 'faad2' 'libupnp' 'libmad'
         'libmpeg2' 'xcb-util-keysyms' 'libtar' 'libxinerama' 'libsecret'
         'libarchive' 'qt5-base' 'qt5-x11extras' 'qt5-svg' 'freetype2'
         'fribidi' 'harfbuzz' 'fontconfig' 'libxml2' 'gnutls' 'wayland-protocols'
         'libidn' 'aribb24' 'qt5-quickcontrols2' 'qt5-graphicaleffects' 'libmicrodns>=0.1.2'
         'libplacebo' 'libixml.so')
makedepends=('gst-plugins-base-libs' 'live-media' 'libnotify' 'libbluray'
             'flac' 'libdc1394' 'libavc1394' 'libcaca' 'gtk3'
             'librsvg' 'libgme' 'twolame' 'aalib' 'avahi' 'systemd-libs'
             'libmtp' 'libupnp' 'libmicrodns' 'libdvdcss' 'smbclient'
             'vcdimager' 'libssh2' 'mesa' 'protobuf' 'libnfs' 'mpg123'
             'libdvdread' 'libdvdnav' 'libogg' 'libshout' 'libmodplug' 'libvpx'
             'libvorbis' 'speex' 'opus' 'libtheora' 'libpng' 'libjpeg-turbo'
             'libx265.so' 'libx264.so' 'zvbi' 'libass' 'libkate' 'libtiger'
             'sdl_image' 'libpulse' 'alsa-lib' 'jack' 'libsamplerate' 'libsoxr'
             'lirc' 'libgoom2' 'projectm' 'git' 'aom' 'srt'
             'vulkan-headers' 'dav1d' 'flex' 'bison' 'xosd' 'aribb25' 'pcsclite'
             'libebur128')
optdepends=('avahi: service discovery using bonjour protocol'
            'gst-plugins-base-libs: for libgst plugins'
            'libdvdcss: decoding encrypted DVDs'
            'libavc1394: devices using the 1394ta AV/C'
            'libdc1394: IEEE 1394 access plugin'
            'kwallet: kwallet keystore'
            'libva-vdpau-driver: vdpau backend nvidia'
            'libva-intel-driver: video backend intel'
            'libbluray: Blu-Ray video input'
            'flac: Free Lossless Audio Codec plugin'
            'twolame: TwoLAME mpeg2 encoder plugin'
            'libgme: Game Music Emu plugin'
            'vcdimager: navigate VCD with libvcdinfo'
            'libmtp: MTP devices discovery'
            'systemd-libs: udev services discovery'
            'smbclient: SMB access plugin'
            'libcdio: audio CD playback'
            'ttf-freefont: subtitle font '
            'ttf-dejavu: subtitle font'
            'libssh2: sftp access'
            'libnfs: NFS access'
            'mpg123: mpg123 codec'
            'protobuf: chromecast streaming'
            'lua-socket: http interface'
            'live-media: RTSP input'
            'libdvdread: DVD input module'
            'libdvdnav: DVD with navigation input module'
            'libogg: Ogg and OggSpots codec'
            'libshout: shoutcast/icecast output plugin'
            'libmodplug: MOD output plugin'
            'libvpx: VP8 and VP9 codec'
            'libvorbis: Vorbis decoder/encoder'
            'speex: Speex codec'
            'opus: opus codec'
            'libtheora: theora codec'
            'libpng: PNG support'
            'libjpeg-turbo: JPEG support'
            'librsvg: SVG plugin'
            'x264: H264 encoding'
            'x265: HEVC/H.265 encoder'
            'zvbi: VBI/Teletext decoding'
            'libass: Subtitle support'
            'libkate: Kate codec'
            'libtiger: Tiger rendering for Kate streams'
            'sdl_image: SDL image support'
            'aalib: ASCII art video output'
            'libcaca: colored ASCII art video output'
            'libpulse: PulseAudio audio output'
            'alsa-lib: ALSA audio output'
            'jack: jack audio server'
            'libsamplerate: audio Resampler'
            'libsoxr: SoX audio Resampler'
            'chromaprint: Chromaprint audio fingerprinter'
            'lirc: lirc control'
            'libgoom2: Goom visualization'
            'projectm: ProjectM visualisation'
            'ncurses: ncurses interface'
            'libnotify: notification plugin'
            'gtk3: notification plugin'
            'aom: AOM AV1 codec'
            'srt: SRT input/output plugin'
            'dav1d: dav1d AV1 decoder')

_name=vlc
conflicts=("${_name}" 'vlc-dev' 'vlc-plugin' 'vlc-stable-git')
provides=("${_name}=${pkgver}")
options=(debug !emptydirs)
source=('git+https://github.com/videolan/vlc.git'
        'vlc-live-media-2021.patch'
        'update-vlc-plugin-cache.hook')
b2sums=('SKIP'
        '76103422a1eaad40d33bfb7897bf25c1b5748729270974bec13f642f2861c4458f0dc07b5fb68d9ba4fae6e44d4a6c8e4d67af7ec10e0c117f1b804dd06868e3'
        'fe3849f45fb91d3697573a9c23b90b78ff0bef5f94c42bc6e7c14427637f45f2fc86786803fb9b36c657ac2c50f6bf3c860cd763248711308ceab2bfcf7be49a')

pkgver() {
  cd "${srcdir}/${_name}"
  printf "%s.r%s.g%s" "$(grep 'AC_INIT' configure.ac | sed 's/[^0-9\.]*//g')" "$(git describe --tags --long | cut -d '-' -f 3)" "$(git rev-parse --short HEAD)"
}

prepare() {
  cd "${srcdir}/${_name}"

  ./bootstrap

  sed -e 's:truetype/ttf-dejavu:TTF:g' -i modules/visualization/projectm.cpp
  sed -e 's|-Werror-implicit-function-declaration||g' -i configure
  patch -Np1 < "${srcdir}"/vlc-live-media-2021.patch
  sed 's|whoami|echo builduser|g' -i configure
  sed 's|hostname -f|echo arch|g' -i configure
  autoreconf -vf
}

build() {
  cd "${srcdir}/${_name}"

  export CFLAGS+=" -I/usr/include/samba-4.0 -ffat-lto-objects"
  export CPPFLAGS+=" -I/usr/include/samba-4.0"
  export CXXFLAGS+=" -std=c++11"
  export LUAC=/usr/bin/luac
  export LUA_LIBS="$(pkg-config --libs lua)"
  export RCC=/usr/bin/rcc-qt5
  export PKG_CONFIG_PATH="/usr/lib/pkgconfig/:$PKG_CONFIG_PATH"

  ./configure --prefix=/usr \
              --sysconfdir=/etc \
              --libexecdir=/usr/lib \
              --with-kde-solid=/usr/share/solid/actions/ \
              --disable-rpath \
              --enable-nls \
              --enable-archive \
              --enable-live555 \
              --enable-dc1394 \
              --enable-dv1394 \
              --enable-dvdread \
              --enable-dvdnav \
              --enable-bluray \
              --disable-opencv \
              --enable-smbclient \
              --enable-sftp \
              --enable-nfs \
              --enable-realrtsp \
              --enable-dvbpsi \
              --enable-gme \
              --enable-ogg \
              --enable-shout \
              --enable-matroska \
              --enable-mod \
              --enable-mpc \
              --enable-mad \
              --enable-mpg123 \
              --enable-gst-decode \
              --enable-avcodec \
              --enable-libva \
              --enable-avformat \
              --enable-postproc \
              --enable-faad \
              --enable-vpx \
              --enable-twolame \
              --disable-fdkaac \
              --enable-a52 \
              --enable-dca \
              --enable-flac \
              --enable-libmpeg2 \
              --enable-vorbis \
              --enable-speex \
              --enable-opus \
              --enable-oggspots \
              --disable-schroedinger \
              --enable-png \
              --enable-jpeg \
              --enable-x264 \
              --enable-x265 \
              --enable-zvbi \
              --enable-libass \
              --enable-kate \
              --enable-tiger \
              --enable-vdpau \
              --enable-wayland \
              --enable-sdl-image \
              --enable-freetype \
              --enable-fribidi \
              --enable-harfbuzz \
              --enable-fontconfig \
              --enable-svg \
              --enable-svgdec \
              --enable-aa \
              --enable-caca \
              --enable-pulse \
              --enable-alsa \
              --enable-jack \
              --enable-samplerate \
              --enable-soxr \
              --disable-chromaprint \
              --disable-chromecast \
              --enable-qt \
              --enable-skins2 \
              --enable-libtar \
              --enable-ncurses \
              --enable-lirc \
              --enable-goom \
              --enable-projectm \
              --enable-avahi \
              --enable-mtp \
              --enable-upnp \
              --enable-microdns \
              --enable-libxml2 \
              --disable-libgcrypt \
              --enable-gnutls \
              --enable-taglib \
              --enable-secret \
              --enable-kwallet \
              --disable-update-check \
              --enable-notify \
              --enable-libplacebo \
              --enable-vlc \
              --enable-aribsub \
              --enable-aribcam \
              --enable-aom \
              --enable-srt \
              --enable-dav1d

  # prevent excessive overlinking due to libtool
  sed -i -e 's/ -shared / -Wl,-O1,--as-needed\0/g' libtool

  make
}

package() {
  cd "${srcdir}/${_name}"

  make DESTDIR="${pkgdir}" install

  for res in 16 32 48 128 256; do
    install -Dm 644 "${srcdir}"/"${_name}"/share/icons/"${res}"x"${res}"/vlc.png \
                     "${pkgdir}"/usr/share/icons/hicolor/"${res}"x"${res}"/apps/vlc.png
  done

  install -Dm 644 "${srcdir}"/update-vlc-plugin-cache.hook -t "${pkgdir}"/usr/share/libalpm/hooks
}
