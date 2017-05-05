# Marlin 3D Printer Firmware
<img align="right" src="../../raw/1.1.x/buildroot/share/pixmaps/logo/marlin-250.png" />

## Marlin 1.1.0

Marlin 1.1 represents an evolutionary leap over Marlin 1.0.2. It is the result of over two years of effort by several volunteers around the world who have paid meticulous and sometimes obsessive attention to every detail. For this release we focused on code quality, performance, stability, and overall user experience. Several new features have also been added, many of which require no extra hardware.

Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).
Please test this firmware and inform us if it misbehaves in any way, volunteers are standing by!

## Bugfix Branch

__Not for production use. Use with caution!__

This branch is used to accumulate patches to the latest 1.1.x release version. Periodically this branch will form the basis for the next minor 1.1.x release.

Download earlier versions of Marlin on the [Releases page](https://github.com/MarlinFirmware/Marlin/releases). (The latest tagged release of Marlin is version 1.1.0.)

## Recent Changes
- 1.1.0 - 4 May 2017
  - See the [1.1.0 Release Notes](https://github.com/MarlinFirmware/Marlin/releases/tag/1.1.0) for a full list of changes.

- RC8 - 6 Dec 2016
  - Major performance improvement for Graphical LCDs
  - Simplified probe configuration
  - Enable Auto Bed Leveling by type
  - Reduce serial communication errors
  - Make Bilinear (Mesh) Grid Leveling available for non-delta
  - Support for Trinamic TMC2130 SilentStepStick SPI-based drivers
  - Add `M211` to Enable/Disable Software Endstops
  - Add `M355` to turn the case light on/off and set brightness
  - Improved I2C class with full master/slave support
  - Add `G38.2` `G38.3` command option for CNC style probing
  - Add `MINIMUM_STEPPER_PULSE` option to adjust step pulse duration
  - Add `R` parameter support for `G2`/`G3`
  - Add `M43` optional command (`PINS_DEBUGGING`)
  - Remove SCARA axis scaling
  - Improved sanity checking of configuration
  - Improved support for PlatformIO and command-line build
  - Usable `DELTA_CALIBRATION_MENU`
  - Support for Printrbot Rev.F
  - New and updated languages

Note that our "bugfix" branch will always contain the latest patches to the current release version. These patches may not be widely tested. As always, when using "nightly" builds of Marlin, proceed with full caution.

## Current Status: In Development

Marlin development has reached an important milestone with its first stable release in over 2 years. During this period we focused on cleaning up the code and making it more modern, consistent, readable, and sensible.

## Future Development

Marlin 1.1 is the last "flat" version of Marlin!

Arduino IDE now has support for folder hierarchies, so Marlin 1.2 will have a [hierarchical file structure](/MarlinFirmware/Marlin/tree/breakup-marlin-idea). Marlin's newly reorganized code will be easier to work with and form a stronger starting-point as we get into [32-bit CPU support](/MarlinFirmware/Marlin/tree/32-Bit-RCBugFix-new) and the Hardware Access Layer (HAL).

[![Coverity Scan Build Status](https://scan.coverity.com/projects/2224/badge.svg)](https://scan.coverity.com/projects/2224)
[![Travis Build Status](https://travis-ci.org/MarlinFirmware/Marlin.svg)](https://travis-ci.org/MarlinFirmware/Marlin)

## Submitting Patches

Proposed patches should be submitted as a Pull Request against this branch ([bugfix-1.1.x](https://github.com/MarlinFirmware/Marlin/tree/bugfix-1.1.x)).

- This branch is for fixing bugs and integrating any new features for the duration of the Marlin 1.1.x life-cycle. We've opted for a simplified branch structure while we work on the maintainability and encapsulation of code modules. Version 1.2 and beyond should improve on separation of bug fixes and cutting-edge development.
- Follow the proper coding style to gain points with the maintainers. See our [Coding Standards](http://marlinfw.org/docs/development/coding_standards.html) page for more information.
- Please submit your questions and concerns to the [Issue Queue](https://github.com/MarlinFirmware/Marlin/issues). The "naive" question is often the one we forget to ask.

### [RepRap.org Wiki Page](http://reprap.org/wiki/Marlin)

## Credits

The current Marlin dev team consists of:
 - Roxanne Neufeld [@Roxy-3D] - English
 - Scott Lahteine [@thinkyhead] - English
 - Bob Kuhn [@Bob-the-Kuhn] - English
 - Andreas Hardtung [@AnHardt] - Deutsch, English
 - Nico Tonnhofer [@Wurstnase] - Deutsch, English
 - Jochen Groppe [@CONSULitAS] - Deutsch, English
 - João Brazio [@jbrazio] - Portuguese, English
 - Bo Hermannsen [@boelle] - Danish, English
 - Bob Cousins [@bobc] - English
 - [@maverikou]
 - Chris Palmer [@nophead]
 - [@paclema]
 - Erik van der Zalm [@ErikZalm]
 - David Braam [@daid]
 - Bernhard Kubicek [@bkubicek]

More features have been added by:
 - Alberto Cotronei [@MagoKimbra] - English, Italian
 - Thomas Moore [@tcm0116]
 - Ernesto Martinez [@emartinez167]
 - Petr Zahradnik [@clexpert]
 - Kai [@Kaibob2]
 - Edward Patel [@epatel]
 - F. Malpartida [@fmalpartida] - English, Spanish
 - [@esenapaj] - English, Japanese
 - [@benlye]
 - [@Tannoo]
 - [@teemuatlut]
 - [@bgort]
 - [@LVD-AC]
 - [@paulusjacobus]
 - ...and many others

## License

Marlin is published under the [GPL license](/COPYING.md) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.

[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
