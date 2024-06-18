# C++ Project Template with CMake

Welcome to the C++ Project Template! This repository provides a basic setup for a C++ project using CMake. It includes scripts for both PowerShell (Windows) and Bash (Linux) to streamline the build process.

## Directory Structure

```bash
C++-Project-Template/
├── build/ # Directory where build artifacts will be generated
├── src/ # Directory containing the source code
├── scripts/
│ ├── build.ps1 # PowerShell script for building on Windows
│ └── build.sh # Bash script for building on Linux
├── CMakeLists.txt # CMake configuration file
└── README.md # This file
```

## Prerequisites

- **CMake**: Make sure CMake is installed on your system. You can download it from [here](https://cmake.org/download/).

## Building the Project

### On Windows

1. Open PowerShell.
2. Navigate to the project directory.
3. Run the PowerShell build script:
    ```powershell
    ./scripts/build.ps1
    ```
4. Navigate to the build directory:
    ```powershell
    cd build
    ```
5. Run `make` to build the project:
    ```powershell
    mingw32-make
    ```
6. Run the output binary:
    ```powershell
    ./output_binary.exe
    ```

### On Linux

1. Open a terminal.
2. Navigate to the project directory.
3. Make the Bash script executable (only required once):
    ```bash
    chmod +x scripts/build.sh
    ```
4. Run the Bash build script:
    ```bash
    ./scripts/build.sh
    ```
5. Navigate to the build directory:
    ```bash
    cd build
    ```
6. Run `make` to build the project:
    ```bash
    make
    ```
7. Run the output binary:
    ```bash
    ./output_binary
    ```

## Customizing the Project

- Add your C++ source files to the `src` directory.
- Modify the `CMakeLists.txt` file to include your source files and any necessary libraries or dependencies.

## Troubleshooting

- Ensure CMake is installed and added to your system's PATH.
- Check the output of the build scripts for any errors or warnings.
- Make sure you have the necessary build tools installed (`mingw32-make` for Windows and `make` for Linux).
