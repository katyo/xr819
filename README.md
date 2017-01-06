# Allwinner XR819 linux support

Linux wireless driver and firmware for [xr819].

Source code obtained from [armbian].

## Device info

Device | Interface | Bus ID    | Module name
------ | --------- | --------- | -----------
XR819  | SDIO      | 0020:2281 | xradio_wlan

For [XR819][cert] BSP driver can found [here][origsrc] and
firmware blobs can be found [there][origfw1] or [here][origfw2].

May be related to ST cw1**0 [[1]].

Initial comparison between cw1200 (drivers/net/wireless/st/cw1200)
and xradio driver shows that the source code for two drivers are
really similar and the st1200 driver can be improved to support
both devices.

[xr819]: http://linux-sunxi.org/Wifi#Allwinner
[armbian]: https://github.com/igorpecovnik/lib
[cert]: http://certifications.prod.wi-fi.org/pdf/certificate/public/download?cid=WFA61880
[origsrc]: http://filez.zoobab.com/allwinner/h2/201609022/lichee/linux-3.4/drivers/net/wireless/xradio/
[origfw1]: http://filez.zoobab.com/allwinner/h2/201609022/android/hardware/broadcom/wlan/bcmdhd/firmware/xr819/
[origfw2]: https://github.com/igorpecovnik/lib/tree/master/bin/firmware-overlay/xr819
[1]: https://irclog.whitequark.org/linux-sunxi/2016-12-27
