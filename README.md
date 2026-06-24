# Thymine
An tether A7 downgrader for some devices.

Supports MacOS and Ubuntu.

This tool now only supports "iPhone6,2!"

# Compatible devices and versions

# iPhone6,2 (iPhone 5s Global)

iOS 7.0.6 and 7.1.2

# iPhone6,1 (soon) (iPhone 5s GSM)

iOS 7.1.2

# Usage and Guide

Do not forget to put your device into Recovery Mode,
This tool cannot put your device into Recovery Mode
because some issues that we cannot fix.

Firstly install the dependencies.

For MacOS:

`brew install libimobiledevice`
`sudo port install idevicerestore`

For Ubuntu:

`sudo apt install usbmuxd libimobiledevice6 libimobiledevice-utils`

To put your device into DFU before pwned DFU and restore your device into desired version, type :

`./thymine.sh --restore < 7.0.6 or 7.1.2 >:`

 For example: `./thymine.sh --restore 7.0.6`

When the device restored into desired version, it will boot into Recovery Mode.

You will need any iOS version of SHSH blobs. For example you can use 12.5.8 blob or 10.3.3 blob.
You can fetch the SHSH blobs via the Legacy-iOS-Kit

For patching the boot files and put your device into DFU before pwned DFU and boot the desired version, type :

`./thymine.sh --boot < 7.0.6 or 7.1.2 >`

 For example: `./thymine.sh --boot 7.1.2`

And your device is will boot in iOS 7.0.6! (or 7.1.2)

# Thank you very much:

xerub, libimobiledevice team and tihmstar. (for the binaries)

heliX (special thanks)
