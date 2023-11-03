# 1. OpenCTD Build Notes

Key website documentation: 
    https://github.com/OceanographyforEveryone/OpenCTD/tree/main
    
        (26.10.2023) 
        Trying to print the base parts:
OpenCTD_14Bar_Baseplate.3mf
OpenCTD_ElectronicsChassis_Bottom.3mf
OpenCTD_ElectronicsChassis_Top.3mf
Printing using standard high resolution settings (0.1mm)



#### The [manual](https://github.com/OceanographyforEveryone/OpenCTD/blob/main/Documentation/Manual/OpenCTD_ConstructionOperation.pdf) contain the full list to for the system.
https://github.com/OceanographyforEveryone/OpenCTD/blob/main/Documentation/Manual/OpenCTD_ConstructionOperation.pdf


## Table List of Parts Needed

| | Item | Description | Link | Price (€) | Comments |
|---:|:---|:------|:----|:----|:---|
| 4 | Custom Carrier Board | Custom PCB for M0-based OpenCTD | [https://a.co/d/hlJF9NW](https://a.co/d/hlJF9NW)  | 12.99 | *probably not the right link* |
| 5 | Adafruit Feather M0 Adalogger | Microcontroller | [https://www.adafruit.com/product/2796](https://www.adafruit.com/product/2796) | 19.95 | [Amazon.de](https://www.amazon.de/-/en/Adafruit-Feather-M0-Adalogger-ADA2796/dp/B01BMRDBXW) for 28 euro 
| 7 | Adafruit DS3231 Precision RTC Breakout | Real-time clock | [https://www.adafruit.com/product/3013](https://www.adafruit.com/product/3013) | 17.5 | [Amazon.de](https://www.amazon.de/-/en/Adafruit-DS3231-Precision-RTC-Breakout-ADA3013/dp/B01CAOG8IG/ref=sr_1_1?keywords=Adafruit+DS3231+Precision+RTC+Breakout&qid=1698599966&sr=8-1) for 25 euro 
| 8 | CR1220 3V Coin Cell Battery | To power RTC | [https://amzn.eu/d/gCg9msD](https://amzn.eu/d/gCg9msD)  | 6.64 | link good
| 9 | Atlas Scientific EZO Conductivity Circuit | Measures conductivity | [https://www.atlas-scientific.com/product_pages/circuits/ezo_ec.html](https://www.atlas-scientific.com/product_pages/circuits/ezo_ec.html) | 64.34 | guess we need this circuit ..
| 16 | Adafruit DS3231 Precision RTC FeatherWing | Real-time clock | [https://amzn.eu/d/ilk9QE7](https://amzn.eu/d/ilk9QE7)  | 21.99 | is this the same as item 7 which is also a RTC clock 
| 17 | Adafruit Stacking Headers | For connecting RTC | [https://amzn.eu/d/4mRsWOw](https://amzn.eu/d/4mRsWOw)  | 2.8 |
| 18 | Adafruit Perma-Proto Small Breadboard PCB | For protoboard version | [https://www.adafruit.com/product/1214](https://www.adafruit.com/product/1214) | 7.52 | can we find it elsewhere .. is  it needed?
| 21 | DS18B20 Temperature Sensor in Stainless Steel Housing | Measures temperature | [https://a.co/d/24QHySY](https://a.co/d/24QHySY) | 7.99 | okay .. Martin was commenting on this yesterday ..
| 22 | Atlas Scientific K 1.0 Mini Conductivity Probe | Measures conductivity | [https://www.atlas-scientific.com/product_pages/probes/ec_k1-0-mini.html](https://www.atlas-scientific.com/product_pages/probes/ec_k1-0-mini.html) | 123.99 | need to check if we need both the normal *and* mini probe
| 23 | Atlas Scientific K 1.0 Conductivity Probe | Measures conductivity | [https://www.atlas-scientific.com/product_pages/probes/ec_k1-0.html](https://www.atlas-scientific.com/product_pages/probes/ec_k1-0.html)  | 157.99 | probably need this ..
| 24 | MS5803-14BA Pressure Sensor Breakout | Measures pressure | [https://amzn.eu/d/5gxiEdw](https://amzn.eu/d/5gxiEdw)  | 79.23 | hmm .. expensive !!
| 25 | MS5803-14BA Pressure Sensor SMC | Pressure sensor chip | [https://www.digikey.de/en/products/detail/te-connectivity-measurement-specialties/MS580314BA01-00/5277631](https://www.digikey.de/en/products/detail/te-connectivity-measurement-specialties/MS580314BA01-00/5277631) | 23.63 |okay ..
| 26 | SOIC to DIP Adapter | For pressure sensor | [https://amzn.eu/d/af9ZiLB](https://amzn.eu/d/af9ZiLB)  | 8.9 | okay ..
| 28 | Lithium Ion Battery Pack 3.7V 2000 mAh | Battery for OpenCTD | [https://amzn.eu/d/fCoCx4s](https://amzn.eu/d/fCoCx4s)  | 17.09 | okay ..
| 29 | Board-mounted switch | Internal power switch | [https://amzn.eu/d/fWvyRN0](https://amzn.eu/d/fWvyRN0)  | 1.39 | yes ..
| 33 | Half-size breadboard | For testing circuits | [https://amzn.eu/d/2MireJq](https://amzn.eu/d/2MireJq)  | 11.99 | okay ..
| 34 | Screw Terminal Block Extra Long Pins for Breadboarding (3) | For connecting sensors during testing | [https://amzn.eu/d/iAapgTb](https://amzn.eu/d/iAapgTb)  | 8.15 | need to checkl with Martin
| 64 | Conductivity calibration solution | For calibrating conductivity probe | [https://atlas-scientific.com/calibration-solutions/conductivity-calibration-k-1-0-set/](https://atlas-scientific.com/calibration-solutions/conductivity-calibration-k-1-0-set/) | 15.89 |
| 65 | openrov 30bar IMU | Waterproof IMU Link not found yet |   | 10.99 | *please check !!*
| 66 | 10 DOF IMU Sensor | Possible Waterproof IMU | [https://www.waveshare.com/10-dof-imu-sensor-b.htm](https://www.waveshare.com/10-dof-imu-sensor-b.htm)  | 10.99 | Alternative to openrov 30bar IMU



- - -


## Screenshots of all the Parts and tools

![Web-capture_27-10-2023_141725_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_141725_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_141826_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_141826_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_141850_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_141850_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_141929_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_141929_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142032_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142032_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142053_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142053_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_14209_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_14209_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142254_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142254_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142313_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142313_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142349_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142349_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142415_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142415_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)
![Web-capture_27-10-2023_142455_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg](OpenCTD/Documentation/Manual/tools/Web-capture_27-10-2023_142455_gfdkcfdhglbbcnllmbgkfkfbmnfkncio.jpeg)



- - -


## Some Tools Available
![IMG-20231027-WA0003.jpg](OpenCTD/Documentation/Manual/available/IMG-20231027-WA0003.jpg)
![IMG-20231027-WA0005.jpg](OpenCTD/Documentation/Manual/available/IMG-20231027-WA0005.jpg)
![IMG-20231027-WA0006.jpg](OpenCTD/Documentation/Manual/available/IMG-20231027-WA0006.jpg)
![WhatsApp-Image-2023-10-27-at-14.33.26_f75f182d.jpg](OpenCTD/Documentation/Manual/available/WhatsApp-Image-2023-10-27-at-14.33.26_f75f182d.jpg)
![WhatsApp-Image-2023-10-27-at-14.33.27_2111816d.jpg](OpenCTD/Documentation/Manual/available/WhatsApp-Image-2023-10-27-at-14.33.27_2111816d.jpg)
![WhatsApp-Image-2023-10-27-at-14.33.27_f802645e.jpg](OpenCTD/Documentation/Manual/available/WhatsApp-Image-2023-10-27-at-14.33.27_f802645e.jpg)

