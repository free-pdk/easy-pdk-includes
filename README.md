# easy-pdk-includes
This repository contains Easy PDK Programmer specific include files for Padauk MCUs

### Warning: This is a work in progress and may change significantly before being considered stable.  Use at your own risk.

This repo is intended to be integrated into other projects either as a git Submodule or by manual file copy.

This repo should be installed into a easy-pdk/ subdirectory in the root include file directory of a parent project.

#### To install as a git Submodule:
- From the root include directory:
  - `git submodule add https://github.com/free-pdk/easy-pdk-includes.git easy-pdk`
- More info: https://git-scm.com/book/en/v2/Git-Tools-Submodules

#### These include files assume the use of:
- The open source SDCC C compiler: http://sdcc.sourceforge.net/
- The base pdk-includes repository: https://github.com/free-pdk/pdk-includes
- The open source Easy PDK Programmer: https://github.com/free-pdk/easy-pdk-programmer-software

#### File Layout:
- **easy-pdk/calibration.h** - Macros for calibration routines (IHRC, ILRC, and BG) performed during programming.
- **easy-pdk/serial_num.h** - Macro for writing a unique Serial Number during programming.

### Copyright and License:
- Copyright (C) 2019-2020 - Original version by freepdk (https://free-pdk.github.io)
- Copyright (C) 2020 - Split out and refactor by serisman (github@serisman.com)
- License: [GPL v2 (or later) + Linking Exception](LICENSE)
  - The linking exception allows this library to be linked (by SDCC) with proprietary (closed source) applications.
