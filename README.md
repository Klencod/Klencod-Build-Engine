Klencod Build Engine

Build Android applications directly on Android devices.

Klencod Build Engine is an independent build engine designed to compile Android applications and generate APK files directly on Android devices, without requiring an external Linux environment or applications such as Termux.

The engine operates as a standalone Android application and integrates with Klencod IDE through inter-app communication. This allows the IDE to send projects to the engine, execute build operations, and receive the results.

Key Features

1. Programming Language Support

- Compile Java projects using Eclipse Compiler for Java (ECJ).
- Compile Kotlin projects using Kotlin Compiler 2.4.0.
- Support projects combining Java and Kotlin within the currently supported compatibility scope.

2. Dependency and Library Management

- Resolve Maven dependencies.
- Download required libraries and manage transitive dependencies.
- Support local JAR libraries.
- Support local AAR libraries and Maven AAR dependencies.
- Preserve imported files and libraries in the application's internal storage.

3. Android Project Support

- Discover project files and source directories.
- Process AndroidManifest.xml.
- Process Android resources and library resources.
- Support multi-module projects within the currently supported compatibility scope.
- Process resource files and generate the required R files.

4. APK Generation

- Convert compiled code into DEX files using D8.
- Package application resources, compiled code, and libraries.
- Generate APK files.
- Support APK signing.

5. Background Build Execution

- Execute build operations through an Android Foreground Service.
- Monitor build stages and execution logs.
- Display build operation status.
- Allow ongoing build operations to be cancelled.
- Continue build execution when switching to another application, subject to Android system restrictions.

Klencod IDE Integration

Klencod Build Engine is a standalone application and is not embedded inside Klencod IDE.

Integration between the two applications is handled through inter-app communication. Klencod IDE manages the project and user interface, while Klencod Build Engine handles the build process and generates the APK file.

Compatibility

Currently supported architectures:

- ARM64 (arm64-v8a)
- ARM32 (armeabi-v7a)

Other architectures are not currently supported.

Current Release Information

Item| Value
Project| Klencod Build Engine
Version| 0.9.52
Build Number| 62
Release Channel| Beta
Platform| Android

Project Status

The engine is currently in the Beta stage. It has been tested with a range of Java and Kotlin projects, multi-module projects, JAR and AAR libraries, and Android resources.

These tests do not guarantee that every Android project will build successfully. Some projects or build configurations may encounter compatibility or stability issues.

Development is ongoing to improve reliability and expand compatibility with different project configurations.

Download

Get the latest release from the "Releases" (../../releases) page.

Project

Klencod Build Engine — Build Android Applications Directly on Your Device.
