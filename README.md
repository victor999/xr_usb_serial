# xr_usb_serial
Exar USB Serial Driver with RS485 support

This driver should work with any USB UART function in these Exar devices:
	XR21V1410/1412/1414
	XR21B1411
	XR21B1420/1422/1424
	XR22801/802/804

The source code has been tested on Linux kernel 6.6 on Raspberry Pi.  
This may also work with other kernels as well.  


Installation
------------
* Install kernel headers
    # sudo apt-get install raspberrypi-kernel-headers

* Compile and install the common usb serial driver module
	# make
	# make install

* Plug the device into the USB host.  You should see up to four devices created,
  typically /dev/ttyXRUSB[0-3].

