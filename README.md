# QT Application example for Gradle QT Plugin
This example based on [QT Application Example](https://doc.qt.io/qt-5/qtwidgets-mainwindows-application-example.html),
with [QT Application Example Sources](https://code.qt.io/cgit/qt/qtbase.git/tree/examples/widgets/mainwindows/application?h=5.15)

Base sources use qmake while this example repository contains configuration for [Gradle Build Tool](https://gradle.org/)
using [Gradle QT Plugin](https://github.com/axmetishe/gradle-qt-plugin)
and [Gradle C++ Application plugin](https://docs.gradle.org/current/userguide/cpp_application_plugin.html)

## Prerequisites
- QT SDK
- Clang or GCC toolchain

## Build
```shell
./gradlew build
```
This operation will generate QT Meta-Objects, QT Resource Bundle and then will compile and link cpp application
with 'Debug' flavor by default.
Build results will be stored in `build` directory, where `exe` will contain the linked app only, `install` directory
will have generated wrapper script and `lib` folder with app.
