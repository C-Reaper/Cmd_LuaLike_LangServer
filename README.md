## Overview
The project is a C/C++ application that uses Lua-like language scripts for custom scripting. The primary feature is the execution of Lua-like scripts.

## Features
- Execution of Lua-like language scripts (.ll files)
- Memory management for the script environment
- Basic printing functionality in Lua-like scripts

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed: X11, PNG, JPEG (for Linux)

### Build & Run
To build the project for Linux:
```bash
cd <Project>
make -f Makefile.linux all
```
To run the executable:
```bash
make -f Makefile.linux exe
```

To clean the build artifacts:
```bash
make -f Makefile.linux clean
```

For a debug build:
```bash
make -f Makefile.linux alldebug
```

To debug with GDB:
```bash
make -f Makefile.linux debug
```

The project is organized as follows:

<Project>/
├── build/              # .exe files produced by Main.c
├── bin/                # .so produced by *.c in libs
├── libs/               # *.c for bin
├── code/               # scripts from my custom languages for example .rex, .ll, .omml
├── src/                # source code
│   ├── Main.c          # Entry point
│   └── *.h             # stand alone Header-based C-files, without *.c files that implement it
├── Makefile.linux      # Linux Build configuration
├── README.md           # This file
└── LICENSE