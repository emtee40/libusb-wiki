Does libusb support Android?
Yes. However, this will only work if your device has USB host support (including USB On-The-Go dual role) and if the correct permissions are obtained from the user or system image. Please check the android directory for more info.
https://github.com/libusb/libusb/blob/master/android/README

Currently there are also multiple issues reported by the user. Please check the existing tickets as well to see if you can sort out the issues from the hints in the tickets. Version 1.0.24 has made quite some improvements on Android side and you should use version 1.0.24 or later.

An important tip of using the API libusb_wrap_sys_device under Android is mentioned in Issue [#171](https://github.com/libusb/libusb/issues/717) and [Pull Request #830](https://github.com/libusb/libusb/pull/830).

It is possible for the android java bootstrapping work to be done inside the android code of libusb, fully automating use of libusb on android, but nobody has implemented this yet.  A few unsupported forks in the edit history of this article and elsewhere may have some code towards this, but please put the most up-to-date information here.

