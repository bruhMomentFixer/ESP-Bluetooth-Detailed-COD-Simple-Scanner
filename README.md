# ESP-WROOM-32-Detailed-COD-Simple-Scanner
Scans a maximum of devices and then prints the devices addresses, RSSI and a detailed description of the class of device (COD).

Modify the #define SCAN_DEV_MAX to scan a maximum number of devices.

The detailed COD description is based in the https://www.ampedrftech.com/datasheets/cod_definition.pdf which defines the class of device for format 00 devices.

You can check a COD specifications in https://www.ampedrftech.com/cod.htm (insert hexadecimal values).

I also include (commented) functionality to print binary values of the gathered COD so that you can manually check the COD with the pdf guide mentioned before.

Print example:
```
Scanning BT devices.
+1
+1
------------------------------------
# 1: XX:XX:XX:XX:XX:XX
Name: HUAWEI WATCH GT 2e-7F4
RSSI: -77
Class of device: 280704 
Format: 00
MAJOR Service Class:
 - Audio (Speaker, Microphone, Headset Service, ...)
 - Capturing (Scanner, Microphone, ...)
MAJOR Device Class: Wearable
minor Device Class: Wrist Watch
------------------------------------
# 2: XX:XX:XX:XX:XX:XX
Name: S89Pro
RSSI: -31
Class of device: 5A020C 
Format: 00
MAJOR Service Class:
 - Telephony (Cordless Telephony, Modem, Headset Service, ...)
 - Object Transfer (v-Inbox, v-Folder, ...)
 - Capturing (Scanner, Microphone, ...)
 - Networking (AN, Ad hoc, ...)
MAJOR Device Class: Phone (cellular, cordless, payphone, modem, ...)
minor Device Class: Smart Phone
------------------------------------
Scan finished.
```
