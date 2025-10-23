# TT-Metalium C++ Project Template

A comprehensive template for kickstarting TT-Metalium C++ projects using CMake. This template demonstrates how to consume TT-Metalium using CMake's `add_subdirectory` and provides a working example of compute kernel development.

## 🚀 Quick Start

### Prerequisites

- CMake 3.22 or higher
- Compatible compiler (Clang 17+ recommended)

### Building the Template

```bash
# Configure the build
cmake -B build -S . -DCMAKE_BUILD_TYPE=Release

# Build the project
cmake --build build
```

### Running the Example

```bash
# Set environment variable to see kernel output
export TT_METAL_DPRINT_CORES=0,0

# Run the hello world example
./build/hello_world_compute_kernel
```

## 📁 Project Structure

```
cpp-tt-metalium-project-template/
├── CMakeLists.txt              # Main CMake configuration
├── src/                        # Host application source code
│   └── hello_world_compute_kernel.cpp
├── kernel/                     # Device kernel source code
│   └── compute/
│       └── void_compute_kernel.cpp
├── build/                      # Build directory (generated)
└── README.md                   # This file
```
