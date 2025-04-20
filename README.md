# AugerXenith EFI

This repository contains a simple EFI (Extensible Firmware Interface) application written in C.

## Prerequisites

### AugerXenith is made to run on a linux system. Instructions for building it on windows will be here soon.

Before building, you need the following tools and dependencies:

- `clang` for compiling C.
- `lld` for linking the executable.
- `mkfs.vfat` for creating the file system.
- `make` for building it.
- `qemu-system` for running it.

## Installing prerequisites

Install all the packages needed (Debian, Ubuntu):
```bash
sudo apt install make clang dosfstools qemu-system lld
```

## Building

To build it:

1. **Clone the repository:**
```bash
git clone https://github.com/Xaristrike/AugerXenithEFI.git
```
```bash
cd AugerXenithEFI
```
2. **Compile:**
```bash
make
```

## Running
To run it using QEMU:
```bash
make qemu
```

To run it in text mode, QEMU will use the terminal window as the output:
```bash
make qemunographic
```

## Cleaning Up
To clean up build files and other temporary files:
```bash
make clean
```
