# Does libusb support Android?
Yes. However, this will only work if your device has USB host support (including USB On-The-Go dual role) and if the correct permissions are obtained from the user or system image. Please check the android directory for more info.
https://github.com/libusb/libusb/blob/master/android/README

Currently there are also multiple issues reported by the user. Please check the existing tickets as well to see if you can sort out the issues from the hints in the tickets. Version 1.0.24 has made quite some improvements on Android side and you should use version 1.0.24 or later.

An important tip of using the API libusb_wrap_sys_device under Android is mentioned in Issue [#717](https://github.com/libusb/libusb/issues/717) and [Pull Request #830](https://github.com/libusb/libusb/pull/830). As of June 2021, you should be able to use libusb under Android using the approach mentioned in [Pull Request #830](https://github.com/libusb/libusb/pull/830).

Please also look at [Pullrequest #874](https://github.com/libusb/libusb/pull/874) for future improvement.

# Alternative ways
https://github.com/mcuee/libusb-1.0.23-android-helper-service-patch (used by AnotherTerm)

# Termux Android
Please check here to see if it works for you or not.

https://wiki.termux.com/wiki/Termux-usb

https://github.com/green-green-avk/LibUsbManager

https://github.com/normanr/termux-libusb-bridge
