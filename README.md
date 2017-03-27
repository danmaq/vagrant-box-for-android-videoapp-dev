# vagrant-box-for-android-videoapp-dev

Vagrant box for Android video-app develop environment using Qt.

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
