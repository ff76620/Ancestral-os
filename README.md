# Ancestral-os

Kernel Project
A modern C++ kernel implementation.

Overview
This project aims to create a modern, efficient, and extensible kernel written in C++. It leverages modern C++ features to provide a robust and maintainable codebase. The kernel is designed with modularity in mind, allowing for easy addition of new features and drivers.

Features
Memory Management: Advanced memory management system including virtual memory, paging, and a custom page allocator.
Process Management: Process creation, scheduling, and inter-process communication (IPC).
Device Drivers: Support for various hardware devices through modular device drivers.
File System: Virtual file system (VFS) with support for multiple file systems.
Networking: Basic networking stack implementation.
Compatibility: Partial Windows 11 compatibility layer (Win32 API wrappers).
Multimedia: Audio and Video playback capabilities
Security: Security manager for handling security policies and user privileges.
Project Status
Currently, the project is in the alpha stage. Core functionalities such as memory management and process scheduling are implemented. Device driver support is still under development. The Windows 11 compatibility layer is partially implemented, with ongoing efforts to expand its coverage.

Building the Kernel
Prerequisites
A modern C++ compiler (e.g., GCC, Clang) supporting C++17 or later
Make or a similar build system
QEMU or another virtualization platform for testing
Build Instructions
Clone the repository: git clone [repository_url]
Navigate to the project directory: cd [project_directory]
Create a build directory: mkdir build && cd build
Configure the build: cmake .. (or your preferred CMake configuration)
Build the kernel: make
Testing
The kernel includes a suite of unit and integration tests. To run the tests:

Build the tests: make tests
Run the tests: ./tests/kernel_tests (or the appropriate path to the test executable)
Performance Benchmarks
Performance benchmarks are crucial for evaluating the kernel's efficiency. Key areas include:

Process Creation: Time taken to create and destroy processes.
Memory Allocation: Speed of memory allocation and deallocation.
I/O Operations: Performance of disk and network I/O.
Context Switching: Time required for context switching between processes.
Running Benchmarks
Specific benchmarks are located in the /kernel/tests/performance directory. Execute these benchmarks after building to assess performance metrics.

Comparing with Windows 11
When comparing benchmark results with Windows 11, consider the following:

Hardware Differences: Ensure both systems are running on comparable hardware.
System Configuration: Match system configurations (e.g., memory size, CPU cores) as closely as possible.
Benchmark Tools: Use equivalent benchmark tools and methodologies.
Due to the kernel's early stage, significant performance differences are expected. The goal is to progressively optimize the kernel to approach the performance of established operating systems like Windows 11.

Contributing
Contributions are welcome! Please follow these guidelines:

Fork the repository and create a branch for your feature or bug fix.
Write clear and concise commit messages.
Submit a pull request with a detailed description of your changes.
© 2024 Kernel Project. All rights reserved.
