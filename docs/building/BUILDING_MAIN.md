
# 🚀 Build Guide - CaptureMoment

Welcome! This guide will help you build CaptureMoment from source.

## 🧰 Global Prerequisites

Before selecting your platform, ensure you have these tools:

1.  **CMake 4.2+**
2.  **C++23 Compiler**:
    * **Windows**: MSVC 2026.
    * **Linux**: GCC 16+
    * **macOS**: Apple Clang 16+ (Xcode 15+).
3. **Python 3+**

---
## ⚙️ Global Build Configuration

### CMake Build

| Component | Default Status | Necessary | CMake Variable (with Alias) | Description |
| --- | --- | --- | --- | --- |
| Desktop UI | OFF | Manual | \-BUILD\_DESKTOP\_UI <br> (-Ddesktop\_ui=on) | Builds the Qt Quick/QML desktop application. |
| Mobile UI | OFF | Not configured | BUILD\_MOBILE\_UI <br>(mobile\_ui) | Builds the mobile application (future phase). |
| Tests | OFF | Manual in Release / Automatic in Debug | BUILD\_TESTS <br>(-tests=on) | Builds unit and integration tests. |
| Diagnostics | OFF | Manual in Release / Automatic in Debug | BUILD\_DIAGNOSTICS <br> (-Ddiagnostics=on) | Builds with ASan (Windows & macOS), UBSan (macOS), Valgrind (Linux) |
| Benchmarks | OFF | Not configured | BUILD\_BENCHMARKS <br>(benchmarks) | Builds performance benchmarks. |

### Libraries

| Library     | Version      | Link                                                     |
|-------------|:------------------:|----------------------------------------------------------|
| OpenImageIO | 3.1.14.0             | https://github.com/AcademySoftwareFoundation/OpenImageIO |
| Halide      | >=22.1           | https://github.com/halide/Halide                         |
| spdlog      | 1.16.0      | https://github.com/gabime/spdlog                         |
| Exiv2         | 0.28.7| https://github.com/Exiv2/exiv2  |
| Magic Enum         |0.9.7| https://github.com/Neargye/magic_enum/ |
|  Qt6           | 6.10.x| https://doc.qt.io/qt-6/ |
|  GoogleTest           | 1.18.0 | https://github.com/google/googletest/ |

---
## 📦 How to build

### 1. Setup Qt (Optional - Required for UI only)
➡️ Read the Building Qt Guide

### 2. Setup Dependencies & Compile
git clone the project
```bash
# Clone from develop branch
git clone --branch develop --single-branch https://github.com/Capture-Moment/CaptureMoment.git
cd CaptureMoment

# Or from your Fork
```

### 4. Setup Dependencies & Compile
Click the link for your OS for detailed instructions:

* [🟦 **Windows**](BUILDING_WINDOWS.md).
* [🐧 **Linux**](BUILDING_LINUX.md) (Ubuntu, Fedora, Arch).
* [🍎 **macOS**](BUILDING_MACOS.md) (Homebrew and Xcode).
