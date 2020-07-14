# easy-pdk-includes
This repository contains Easy PDK Programmer specific include files for Padauk MCUs

### Warning: This is a work in progress and may change significantly before being considered stable.  Use at your own risk.

This repo is intended to be integrated into other projects either as a git Submodule or by manual file copy.

This repo should be installed into a easy-pdk/ subdirectory in the root includes directory of a parent project.

#### To install as a git Submodule:
- From the root includes directory:
  - `git submodule add https://github.com/free-pdk/easy-pdk-includes.git easy-pdk`
- More info: https://git-scm.com/book/en/v2/Git-Tools-Submodules

#### These include files assume the use of:
- The open-source SDCC C Compiler: http://sdcc.sourceforge.net/ (requires 3.9.0 or newer, 4.0.0+ preferred)
- The base pdk-includes repository: https://github.com/free-pdk/pdk-includes
- The open source Easy PDK Programmer: https://github.com/free-pdk/easy-pdk-programmer-software (requires 1.3 or newer)

### File Layout:
- [**calibrate.h**](calibrate.h) - Macros for calibration routines (IHRC, ILRC, and BG) performed during programming.
- [**serial_num.h**](serial_num.h) - Macro for writing a unique Serial Number during programming.
