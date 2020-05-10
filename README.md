# APK Lab

APK Lab extension provides an automated and easy-to-use workflow for reverse engineering of Android apps (APK) by integrating popular CLI tools such as `Apktool` with the excellent VS Code so you can spend more time on app analysis not tooling.

## Features

1. DeAssemble/Decode an APK file using [**`Apktool`**](https://github.com/ibotpeaches/apktool/)

    ![decode.gif](assets/decode.gif)

## Requirements

1. **JDK 8** or higher should be in your PATH
2. **Apktool**: Download the latest [`apktool.jar`](https://github.com/ibotpeaches/apktool/releases/) and update its location in VS Code settings under (**`Apklab: Apktool Path`**)

> [**Smalise**](https://marketplace.visualstudio.com/items?itemName=LoyieKing.smalise) extension is highly recommended as it makes working with `smali` files a breeze.

## Extension Settings

This extension contributes the following settings:

* **`apklab.javaPath`**: Path of `java` executable. Please update this if JDK is not in the PATH. For example:

  ```json
    {
        "apklab.javaPath": "/usr/bin/java"
    }
  ```

* **`apklab.apktoolPath`**: Path of `apktool.jar`. Please update this with absolute location(full path). For example:

  ```json
    {
        "apklab.apktoolPath": "/home/oozer/downloads/apktool_2.4.1.jar"
    }
  ```

## Known Issues

1. When decoding an APK, save your workspace first as decoded dir opens up in same window and closes all previous editor tabs & workspace.

## Release Notes