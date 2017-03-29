# [danmaq/openSUSE-42.1-x86_64-Android-Qt-videoapp-dev-env](https://atlas.hashicorp.com/danmaq/boxes/openSUSE-42.1-x86_64-Android-Qt-videoapp-dev-env)

Vagrant box for Android video-app develop environment using Qt.

* openSUSE Leap 42.1 (from opensuse/openSUSE-42.1-x86_64 1.0.1)
* patterns-openSUSE-devel_C_C++
* Qt 5.6
* Android SDK (API 21)
* Android NDK r10e
* FFmpeg
* faad2
* libmad
* x264
* libSDL2-devel
* others (see Process overview)

## base box

see: [danmaq/openSUSE-42.1-x86_64-Android-Qt-dev-env](https://github.com/danmaq/box-devenv.android-qt) box.

* openSUSE
* KDE Desktop
* AndroidSDK/NDK
* Qt

## Added

* via Zypper
    * git
    * ant
    * yasm
    * libSDL2-devel
* maked libraries
    * faad2 (for Android/Linux Desktop)
    * libmad (for Android/Linux Desktop)
    * ffmpeg (for Android/Linux Desktop)
    * x264 (for Linux Desktop)
