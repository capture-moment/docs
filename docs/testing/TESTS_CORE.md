# How to run Tests
This guide for running the tests.

```bash
The followings arguments are enabled by default in debug mode -Ddiagnostics="on" -Dtests="on"
```

### Windows MSVC
### Example in Debug mode
```bash
cmake --preset debug-vcpkg-msvc
cmake --build --preset debug-vcpkg-msvc
ctest --preset debug-vcpkg-msvc
```

### Example in Release
```bash
cmake --preset release-vcpkg-msvc -Dtests="on" -Ddiagnostics="on"
cmake --build --preset release-vcpkg-msvc
ctest --preset release-vcpkg-msvc
```

## Linux Ninja
### Example in Debug
```bash
cmake --preset debug-ninja
cmake --build --preset debug-ninja
ctest --preset debug-ninja
```
### Example release
```bash
cmake --preset release-ninja -Dtests="on" -Ddiagnostics="on"
cmake --build --preset release-ninja
ctest --preset release-ninja
```

## macOS Ninja
### Example in Debug
```bash
cmake --preset debug-ninja
cmake --build --preset debug-ninja
ctest --preset debug-ninja
```
### Example release
```bash
cmake --preset release-ninja -Dtests="on" -Ddiagnostics="on"
cmake --build --preset release-ninja
ctest --preset release-ninja
```
