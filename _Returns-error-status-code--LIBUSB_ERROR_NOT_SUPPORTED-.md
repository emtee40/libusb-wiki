Why at start <testlibusb> for some devices 
 ret = libusb_open (dev, &handle)
Returns error status code <LIBUSB_ERROR_NOT_SUPPORTED>?
 
Example:
static int print_device (libusb_device *dev, int level)
{
struct libusb_device_descriptor desc;
libusb_device_handle *handle = NULL;
char description [260], string [256];
int ret;
uint8_t i;

	ret = libusb_get_device_descriptor (dev, &desc);
	if (ret <0) {
		fprintf (stderr, "failed to get device descriptor");
		return-1;
	}

	ret = libusb_open (dev, &handle);
	if (LIBUSB_SUCCESS == ret) { // Ok!
	}
	else {//error!!!
		snprintf (description, sizeof (description), "Err: %04X - %04X", desc.idVendor, desc.idProduct);
	}
...................
}

I use Win7 x64. 