# NB-IoT Module

> NarrowBand IoT (NB-IoT) is a Low Power Wide Area Network ([LPWAN](https://en.wikipedia.org/wiki/LPWAN)) radio technology standard developed to enable a wide range of devices and services to be connected using cellular telecommunications bands. NB-IoT is a [narrowband radio](https://en.wikipedia.org/wiki/Narrowband) technology designed for the [Internet of Things](https://en.wikipedia.org/wiki/Internet_of_Things) (IoT) and is one of a range of Mobile IoT (MIoT) technologies standardized by the 3rd Generation Partnership Project ([3GPP](https://en.wikipedia.org/wiki/3GPP)). Other 3GPP IoT technologies include eMTC (enhanced Machine-Type Communication) and EC-GSM-IoT. The NB-IoT specification was frozen at Release 13 of the 3GPP specification (LTE-Advanced Pro), in June 2016.

Wikipedia: [NB-IoT](https://en.wikipedia.org/wiki/NarrowBand_IOT)

## Quectel: BC95 NB-IoT Module

![Quectel BC95 NB-IoT Module](http://www.quectel.com/UploadImage/Product/20170412154839662.png)  
Source: [Quectel BC95 product page](http://www.quectel.com/product/gsmevb.htm)

> BC95 is a high-performance NB-IoT module with extremely low power consumption. The ultra-compact 19.9 × 23.6 × 2.2mm profile makes it a perfect choice for size sensitive applications. Designed to be compatible with Quectel GSM/GPRS M95 module in the compact and unified form factor, it provides a flexible and scalable platform for migrating from GSM/GPRS to NB-IoT networks.

Quectel: [BC95](http://www.quectel.com/product/bc95.htm)

If you need more specifications for the BC95 module you can check out the [specifications](http://www.quectel.com/UploadFile/Product/Quectel_GSM_EVB_User_Guide_V3.4.pdf)

## Connection between Calliope and NB-IoT Board

The BC95 development board is connected via uart to the calliope board. The devcelopment board need a higher voltage (+5V) than the calliope is capable (+3.3V), thats the reason why you need an additional power supply exclusivly for the NB-IoT board.

And example and the wiring of the module can be found in the [official calliope repo](https://github.com/calliope-mini/pxt-calliope-bc95)
**Note:** Dont connect the VCC of the NB-IoT development board to the calliope board. Otherwise the calliope board will brick.

## Control the NB-IoT Board
For further information about the functions and API's for the board check out the examples in the [bc95 calliope repo](https://github.com/calliope-mini/pxt-calliope-bc95)
* [Visual Editor](https://raw.githubusercontent.com/calliope-mini/pxt-calliope-bc95/master/example.png)
* [JavaScript](https://github.com/calliope-mini/pxt-calliope-bc95/blob/master/example.ts)
* [C++](https://github.com/calliope-mini/pxt-calliope-bc95/blob/master/ext_serial.cpp)