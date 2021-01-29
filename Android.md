Does libusb support Android?
Yes. However, this will only work if your device has USB host support (also known as USB On-The-Go) and if you have sufficient privileges to run in host mode. Please check the android directory for more info.
https://github.com/libusb/libusb/blob/master/android/README

Currently there are also multiple issues reported by the user. Please check the existing tickets as well to see if you can sort out the issues from the hints in the tickets. Version 1.0.24 has made quite some improvements on Android side and you should use version 1.0.24 or later.

An important tip of using the API libusb_wrap_sys_device under Android is mentioned in Issue [#7171](https://github.com/libusb/libusb/issues/717) and [Pull Request #830](https://github.com/libusb/libusb/pull/830).

