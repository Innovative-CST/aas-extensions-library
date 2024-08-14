# Extension Generator
This repository is a template which is used to generate the extension files for [Android App Studio](https://github.com/TS-Code-Editor/AndroidAppStudio)

> [!CAUTION]
> Do not make modifications in any files of library module.

# Entry point
The entry point for generating extension file is `extension/src/main/java/com/icst/android/appsstudio/ExtensionGenerator.java`.
When you will execute this project with task `generateExtensions` then gradle will execute `ExtensionGenerator.java`.
In `ExtensionGenerator.java` you will have to pass the object of `com.icst.android.appstudio.models.ExtensionBundle` so gradle can generate extension.

> [!NOTE]
> You can write your ExtensionBundle object in any file but remember you just have to pass object of `ExtensionBundle` in `ExtensionGenerator`.
> You can run this project in Android IDE also.
> For testing blocks please build android app studio on your device and set STORAGE property to a accessible directory in `gradle.properties` and then extract the extension file generated by this project to `$STORAGE/Extension`.