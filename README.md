# QtuneGX Android

QtuneGX Android is a  robust GPLv3 Mumble client for Android originally written by Andrew Comminos.
It uses the [Rimic](https://github.com/TommyTeaVee/rimic_android) protocol implementation
(forked from Comminos's [Jumble](https://github.com/acomminos/Jumble)).

QtuneGX Android should run on Android 4.0 (IceCreamSandwich, API 14) and later.


There is an instructions configuration and [WiMic Server/Client](https://github.com/hiro2233/wimic) installation on https://hiro2233.github.io/wimic/docs/.

## Building on GNU/Linux

TODO: rimic-spongycastle should be built as a sub-project of Rimic's Gradle,
but currently isn't.

    git submodule update --init --recursive

    pushd libraries/rimic/libs/rimic-spongycastle
    ../../gradlew jar
    popd

    ./gradlew assembleDebug

## License

WiMic's [LICENSE](LICENSE) is GNU GPL v3.
