# EarthBound Android - Edzito Edition 3.6.4

An experimental fan-made Android adaptation, based on Brian Pugh and
contributors' EarthBound C implementation and Herringway/ebsrc's disassembly
and research. See [Community credits](CREDITS.md) and the original notices
in [licenses](licenses). This repository contains a packaged Android release
and documentation; the underlying projects are linked in the credits.

## Installation

Android 8.0+ with a 64-bit ARM processor is required. Install the APK, then
select your own unmodified EarthBound (USA) ROM using the app's file picker.
No ROM is included. Updating with the same package/signing identity should
preserve private app data; uninstalling removes that data.

## Touch controls

- Drag from your initial touch point to walk; drag farther to run.
- Tap native menu choices directly. Hold during dialogue to speed up text.
- Double tap or use two fingers for the personal menu / Back.
- Pinch to zoom. Mr. Saturn opens options; the portrait menu scrolls.
- Black phone: choose a quicksave to save. Red phone: choose one to load.
- Optional OK/Back buttons default off. Speed/rewind buttons are optional.
- Button visibility, size and opacity are configurable in Touch.
- Credits are available in the options menu. The optional God Menu includes
  a hitkill-button toggle; cheats and co-op remain experimental.

## Testing status

The APK's signature, archive, ARM64 libraries and 16 KiB alignment are checked.
Touch/portrait-menu behavior is tested through SDL simulations on Windows.
The latest release has not been validated on a physical Android device.
The smaller internal render canvas reduces pixel work; device FPS improvements
have not been measured. The output still fills the phone display.

## Original authors and this edition

EarthBound was created by Nintendo, Shigesato Itoi, APE, HAL Laboratory and
the original teams. The C foundation and inherited disassembly belong to
their respective authors. Edzito's edition adds the menus, co-op and other
modifications, with Codex assistance. Library authors, translators, researchers,
testers and preservation communities are credited in CREDITS.md.
