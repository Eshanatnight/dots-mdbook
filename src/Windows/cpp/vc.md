# Vcpkg & CMake

---

## Vcpkg

### Installation

To install ***vcpkg*** you can run the [script](../scripts/install-vcpkg.ps1). It's a
Poweshell Script that will clone the repository from the
[official page](https://github.com/microsoft/vcpkg.git) in the location `D:\tools\vcpkg`
and then bootstrapping vcpkg.

> Note: You would need to add the executable to env PATH, if you want to use it globally in the terminal

### Using

Navigate to the project repository. Create a build directory `build`, or whatever you want to name.
Navigate to the build Directory.

```terminal
mkdir build

cd build
```

```terminal
cmake .. -DCMAKE_TOOLCHAIN_FILE=<path-to-vcpkg>/scripts/buildsystems/vcpkg.cmake
```

```terminal
cmake --build .
```

> Note: if you are using the Visual Studio cl compiler.
> Then to get the release build of the project.
> You need to pass `--release` flag in the build command. Like so

```terminal
cmake --build . --release
```

### VCPKG in Manifest Mode

vcpkg has now a mainfest mode. To use it, you need a manifest file `vcpkg.json` in the
place where the top level `CMakelists.txt` file is.

#### Format for `vcpkg.json`

`filename: vcpkg.json`

```json
{
    "name": "Project_Name",
    "version-string": "0.0.1",
    "description": "Project_Description",

    "dependencies":
    [
        "name_of_package",
        {
            "name": "name_of_package",
            "features": [ "feature_name" ]
        }
    ]
}
```

---

## CMake

### VSCode Settings

To use CMake and vcpkg in Manifest Mode. Add the following to the vscode `settings.json` file.

```json
"cmake.configureSettings": {
     "CMAKE_TOOLCHAIN_FILE": "path/to/vcpkg/scripts/buildsystems/vcpkg.cmake"
}
"cmake.configureOnOpen": true
```

### CMAKE Common Settings

```cmake
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
```