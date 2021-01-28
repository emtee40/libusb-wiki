There is some existing android support in the main tree.  Information on this support is available at https://github.com/libusb/libusb/blob/master/android/README .

The support in the main tree currently relies on access to the usb device files being enabled via other means.  It is also possible to reliably access USB without root on Android by using the JNI.

These forks also have implemented some android support:

- https://github.com/SpecLad/libusb-android (uses Java interface, not updated since 2012)
- https://github.com/kuldeepdhaka/libusb/tree/android-open2
- https://gitlab.com/madresistor/libusb/tree/android